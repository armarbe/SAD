# Plantilla de Plan de Contingencias
---

*Nota: este plan debe ser revisado mensualmente y actualizado tras cada incidente mayor. En fase de construcción.*


---

## Información del documento

| Campo | Información |
|-------|-------------|
| **Equipo** | [Nombres del equipo] |
| **Fecha** | [DD/MM/AAAA] |
| **Versión** | [v1.0] |
| **Sistemas** | [Lista de sistemas cubiertos] |

---

## 1. Objetivos de recuperación

- **RTO (Recovery Time Objective):** [Tiempo máximo de caída aceptable]
- **RPO (Recovery Point Objective):** [Pérdida máxima de datos aceptable]
- **Disponibilidad objetivo:** [Porcentaje de uptime]

---

## 2. Clasificación de incidentes

### 🔴 Nivel 1 - CRÍTICO
- **Criterios:** Servicio completamente caído, compromiso grave de seguridad
- **Respuesta:** < 15 minutos
- **Ejemplos:** Servidor principal inaccesible, ataque exitoso, pérdida total de conectividad

### 🟡 Nivel 2 - ALTO  
- **Criterios:** Degradación significativa del servicio
- **Respuesta:** < 30 minutos
- **Ejemplos:** VPN lenta, servicios parcialmente caídos, intentos de intrusión

### 🟢 Nivel 3 - MEDIO
- **Criterios:** Impacto menor, problemas de rendimiento
- **Respuesta:** < 2 horas
- **Ejemplos:** Alertas de monitorización, errores en logs

### 🔵 Nivel 4 - BAJO
- **Criterios:** Sin impacto operativo, consultas
- **Respuesta:** < 8 horas laborales
- **Ejemplos:** Mantenimiento programado, optimizaciones

---

## 3. Inventario de sistemas críticos

| Sistema | Criticidad | RTO | RPO | Procedimiento |
|---------|------------|-----|-----|---------------|
| **Servidor principal** | Crítico | 30 min | 15 min | Sección 5.1 |
| **VPN** | Alto | 1 hora | 1 hora | Sección 5.2 |
| **Firewall** | Crítico | 15 min | N/A | Sección 5.3 |
| **Home Assistant** | Medio | 2 horas | 1 hora | Sección 5.4 |
| **Proxy inverso** | Alto | 1 hora | N/A | Sección 5.5 |

---

## 4. Equipo de respuesta

### Roles y contactos

| Rol | Responsable | Teléfono | Email | Responsabilidades |
|-----|-------------|----------|-------|-------------------|
| **Coordinador** | [Nombre] | [Tel] | [Email] | Coordinar respuesta, comunicar |
| **Técnico Principal** | [Nombre] | [Tel] | [Email] | Diagnóstico y solución técnica |
| **Técnico Backup** | [Nombre] | [Tel] | [Email] | Soporte técnico secundario |

### Escalado
1. **Detección** → Técnico de guardia (15 min)
2. **No resuelto** → Técnico Principal (30 min)
3. **Nivel 1 o >1 hora** → Coordinador (inmediato)

---

## 5. Procedimientos de recuperación

### 5.1 Servidor principal caído

**Diagnóstico:**
```

ping [IP_SERVIDOR]
ssh [USER]@[IP_SERVIDOR]

```

**Acciones:**
1. Verificar alimentación y conexiones físicas
2. Reinicio suave: `sudo reboot`
3. Reinicio físico si es necesario
4. Restaurar desde backup si falla hardware

**Verificación:**
- [ ] Ping responde
- [ ] SSH accesible
- [ ] Servicios principales activos

### 5.2 VPN no funciona

**Diagnóstico:**
```

sudo systemctl status openvpn@servidor
sudo systemctl status wg-quick@wg0
sudo journalctl -u openvpn@servidor -f

```

**Acciones:**
```


# Reiniciar servicio

sudo systemctl restart openvpn@servidor
sudo systemctl restart wg-quick@wg0

# Verificar configuración

sudo iptables -L -n
sudo ip route show

```

### 5.3 Compromiso de seguridad

**Respuesta inmediata (15 min):**
1. **Aislar sistema:**
```

sudo iptables -A INPUT -j DROP
sudo iptables -A OUTPUT -j DROP

```

2. **Preservar evidencias:**
```

sudo cp /var/log/* /backup/incident-logs/
sudo netstat -tulpn > /backup/conexiones-$(date +%Y%m%d-%H%M).txt
sudo ps aux > /backup/procesos-$(date +%Y%m%d-%H%M).txt

```

3. **Análisis:**
```

sudo grep -i "failed\|attack" /var/log/auth.log
sudo fail2ban-client status

```

---

## 6. Copias de seguridad

### Backup automático diario
```

\#!/bin/bash

# backup-diario.sh

DATE=\$(date +%Y%m%d-%H%M)
BACKUP_DIR="/backup/daily"

# Configuraciones críticas

tar -czf "$BACKUP_DIR/config-$DATE.tar.gz" \
/etc/openvpn/ \
/etc/nginx/ \
/etc/fail2ban/ \
/home/dietpi/.homeassistant/

# Limpiar backups >7 días

find "\$BACKUP_DIR" -name "*.tar.gz" -mtime +7 -delete

```

### Restauración
```


# Restaurar configuraciones

tar -xzf /backup/daily/config-YYYYMMDD-HHMM.tar.gz -C /

# Reiniciar servicios

sudo systemctl restart openvpn@servidor nginx fail2ban

```

---

## 7. Comunicación

### Canales
- **Primario:** Slack #incidentes
- **Backup:** WhatsApp grupal
- **Email:** lista-incidentes@proyecto.local

### Plantilla de notificación
```

ASUNTO: [INCIDENTE NIVEL X] - [Descripción breve]

Detectado incidente en [sistema] a las [HH:MM]

IMPACTO: [Descripción]
ESTADO: [En investigación/En resolución]
ETA RESOLUCIÓN: [X horas]

Próxima actualización: [HH:MM]

```

---

## 8. Monitorización

### Script básico de monitorización
```

\#!/bin/bash

# monitor.sh - Ejecutar cada 5 minutos

# Servicios críticos

services=("ssh" "openvpn@servidor" "nginx" "fail2ban")
for service in "${services[@]}"; do
  if ! systemctl is-active --quiet "$service"; then
echo "ALERTA: \$service caído" | mail -s "Servicio caído" admin@proyecto.local
fi
done

# Espacio en disco

DISK_USAGE=\$(df / | awk 'NR==2 {print $5}' | sed 's/%//')
if [ "$DISK_USAGE" -gt 85 ]; then
echo "ALERTA: Disco al \$DISK_USAGE%" | mail -s "Espacio crítico" admin@proyecto.local
fi

```

### KPIs de seguimiento
| Métrica | Normal | Alerta | Acción |
|---------|--------|--------|--------|
| CPU Load | < 1.0 | > 2.0 | Investigar procesos |
| RAM | < 80% | > 90% | Liberar memoria |
| Disco | < 80% | > 85% | Limpiar logs |
| VPN conexiones | Variable | 0 | Verificar servicio |

---

## 9. Post-incidente

### Informe básico
```


## Informe de Incidente [INC-YYYYMMDD-001]

**Resumen:** [Descripción breve]
**Duración:** [X horas]
**Causa:** [Causa raíz identificada]
**Impacto:** [Sistemas y usuarios afectados]

**Cronología:**

- HH:MM - Detección
- HH:MM - Inicio acciones
- HH:MM - Resolución

**Acciones preventivas:**

- [ ] [Acción 1] - Responsable: [Nombre] - Fecha: [DD/MM]
- [ ] [Acción 2] - Responsable: [Nombre] - Fecha: [DD/MM]

```

---

## 10. Comandos útiles

### Diagnóstico básico
```


# Conectividad

ping [host]
traceroute [host]

# Servicios

systemctl status [servicio]
journalctl -u [servicio] -f

# Recursos

htop
df -h
free -h

# Red

netstat -tulpn
ss -ant
sudo iptables -L -n

```

### Backup rápido
```


# Configuración actual

sudo tar -czf backup-emergency-\$(date +%Y%m%d).tar.gz /etc/

# Base de datos (si aplica)

sudo mysqldump -u root -p [database] > db-backup-\$(date +%Y%m%d).sql

```

---

## 11. Lista de verificación

### Durante el incidente
- [ ] Incidente clasificado
- [ ] Equipo notificado
- [ ] Usuarios informados
- [ ] Acciones de contención aplicadas
- [ ] Diagnóstico completado
- [ ] Solución implementada
- [ ] Funcionamiento verificado
- [ ] Resolución comunicada

### Post-incidente
- [ ] Informe de incidente completado
- [ ] Reunión de revisión realizada
- [ ] Lecciones aprendidas documentadas
- [ ] Acciones preventivas planificadas
- [ ] Plan actualizado si es necesario

---

## 12. Contactos de emergencia

- **Proveedor Internet:** [Teléfono]
- **Soporte hardware:** [Teléfono]
- **Profesor responsable:** [Teléfono/Email]

---

**Última actualización:** [DD/MM/AAAA]
**Próxima revisión:** [DD/MM/AAAA]
