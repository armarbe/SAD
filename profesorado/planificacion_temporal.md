# 📅 Planificación temporal del proyecto "De la oficina al hogar inteligente: asegurando el acceso remoto, la domótica y la continuidad del negocio en una PYME"

## ⏰ Distribución general

- **Duración total:** 12 semanas
- **Carga horaria:** 5 horas/semana (60 horas totales)
- **Modalidad:** 2 sesiones por semana (2.5h + 2.5h)

---

## 📋 Calendario detallado por semanas

### **SEMANA 1**

**Fase 1: Análisis empresarial y configuración base**

- **Sesión 1 (2.5h):** presentación del proyecto y análisis DAFO empresarial
- **Sesión 2 (2.5h):** instalación segura de DietPi y configuración SSH
- **RA trabajados:** RA1, RA7
- **🎯 Hito:** entrega análisis de vulnerabilidades (viernes 7/02)


### **SEMANA 2**

**Fase 1: Políticas de seguridad**

- **Sesión 1 (2.5h):** Configuración de políticas de contraseñas y usuarios
- **Sesión 2 (2.5h):** Documentación de procedimientos de seguridad inicial
- **RA trabajados:** RA1, RA7
- **🎯 Hito:** entrega documentación de políticas


### **SEMANA 3**

**Fase 2: Seguridad activa**

- **Sesión 1 (2.5h):** instalación y configuración de Fail2ban
- **Sesión 2 (2.5h):** configuración de sistemas de detección de intrusiones
- **RA trabajados:** RA2
- **🎯 Hito:** pruebas de funcionamiento Fail2ban


### **SEMANA 4**

**Fase 2: Cortafuegos perimetral**

- **Sesión 1 (2.5h):** configuración básica de iptables
- **Sesión 2 (2.5h):** implementación de reglas avanzadas de filtrado
- **RA trabajados:** RA4
- **🎯 Hito:** entrega documentación de reglas de cortafuegos


### **SEMANA 5**

**Fase 2: Filtrado DNS**

- **Sesión 1 (2.5h):** instalación y configuración de Pi-hole
- **Sesión 2 (2.5h):** integración Pi-hole con reglas de cortafuegos
- **RA trabajados:** RA4
- **🎯 Hito:** **EVALUACIÓN PARCIAL 1** - Seguridad perimetral


### **SEMANA 6**

**Fase 3: Contenedores y alta disponibilidad**

- **Sesión 1 (2.5h):** instalación Docker y Docker Compose
- **Sesión 2 (2.5h):** configuración Cloudflare DDNS en contenedor
- **RA trabajados:** RA6
- **🎯 Hito:** servicios críticos en contenedores


### **SEMANA 7**

**Fase 3: Proxy inverso**

- **Sesión 1 (2.5h):** instalación y configuración de Nginx Proxy Manager
- **Sesión 2 (2.5h):** configuración de balanceo de carga y SSL
- **RA trabajados:** RA5
- **🎯 Hito:** proxy inverso funcional con certificados


### **SEMANA 8**

**Fase 4: VPN - OpenVPN**

- **Sesión 1 (2.5h):** instalación y configuración básica de OpenVPN
- **Sesión 2 (2.5h):** configuración de certificados y autenticación
- **RA trabajados:** RA3
- **🎯 Hito:** conexión exitosa cliente OpenVPN


### **SEMANA 9**

**Fase 4: VPN - WireGuard**

- **Sesión 1 (2.5h):** instalación y configuración de WireGuard
- **Sesión 2 (2.5h):** comparativa OpenVPN vs WireGuard - Optimización
- **RA trabajados:** RA3
- **🎯 Hito:** entrega comparativa técnica VPN


### **SEMANA 10**

**Fase 4: Autenticación robusta**

- **Sesión 1 (2.5h):** configuración de métodos de autenticación multifactor
- **Sesión 2 (2.5h):** pruebas de conectividad y rendimiento VPN
- **RA trabajados:** RA3
- **🎯 Hito:** **EVALUACIÓN PARCIAL 2** - Acceso remoto seguro


### **SEMANA 11**

**Fase 5: Domótica empresarial**

- **Sesión 1 (2.5h):** instalación y configuración de Home Assistant
- **Sesión 2 (2.5h):** integración con protocolos Zigbee/Tasmota
- **RA trabajados:** RA6
- **🎯 Hito:** dashboard domótico funcional


### **SEMANA 12**

**Fase 6: Integración y cumplimiento normativo**

- **Sesión 1 (2.5h):** auditoría de cumplimiento RGPD/LOPDGDD/ISO 27001
- **Sesión 2 (2.5h):** **PRESENTACIONES FINALES** y documentación
- **RA trabajados:** RA7, todos los anteriores
- **🎯 Hito:** **ENTREGA FINAL DEL PROYECTO**

---

## 🎯 Hitos y entregas principales

### **Entregas menores (25% de la nota)**

| Semana | Entregable | Peso |
| :-- | :-- | :-- |
| 1 | Análisis de vulnerabilidades empresariales | 5% |
| 2 | Documentación de políticas de seguridad | 5% |
| 4 | Documentación de reglas de cortafuegos | 5% |
| 7 | Comparativa técnica OpenVPN vs WireGuard | 5% |
| 11 | Dashboard domótico funcional | 5% |

### **Evaluaciones parciales (50% de la nota)**

| Semana | Evaluación | Peso | RA evaluados |
| :-- | :-- | :-- | :-- |
| 5 | **Evaluación Parcial 1:** Seguridad perimetral | 25% | RA1, RA2, RA4 |
| 10 | **Evaluación Parcial 2:** Acceso remoto seguro | 25% | RA3 |

### **Entrega final (25% de la nota)**

| Semana | Entregable | Peso | RA evaluados |
| :-- | :-- | :-- | :-- |
| 12 | **Proyecto completo + Presentación** | 25% | RA5, RA6, RA7 + integración |


---

## 📊 Distribución de RA por semanas

```
Semanas  1  2  3  4  5  6  7  8  9 10 11 12
RA1      ██ ██ ░░ ░░ ░░ ░░ ░░ ░░ ░░ ░░ ░░ ░░
RA2      ░░ ░░ ██ ░░ ░░ ░░ ░░ ░░ ░░ ░░ ░░ ░░
RA3      ░░ ░░ ░░ ░░ ░░ ░░ ░░ ██ ██ ██ ░░ ░░
RA4      ░░ ░░ ░░ ██ ██ ░░ ░░ ░░ ░░ ░░ ░░ ░░
RA5      ░░ ░░ ░░ ░░ ░░ ░░ ░░ ░░ ░░ ░░ ██ ░░
RA6      ░░ ░░ ░░ ░░ ░░ ██ ██ ░░ ░░ ░░ ░░ ░░
RA7      ██ ██ ░░ ░░ ░░ ░░ ░░ ░░ ░░ ░░ ░░ ██
```


---

## 🎓 Metodología por semanas

### **Semanas 1-2:** Método expositivo + ABP

- Contextualización empresarial
- Análisis de casos reales
- Trabajo individual y grupal


### **Semanas 3-5:** Aprendizaje práctico guiado

- Laboratorio con seguimiento docente
- Resolución colaborativa de problemas
- Documentación técnica


### **Semanas 6-8:** ABP autónomo

- Trabajo por equipos
- Investigación y experimentación
- Presentaciones intermedias


### **Semanas 9-11:** Integración y síntesis

- Proyecto integrador
- Trabajo colaborativo avanzado
- Mentorización personalizada


### **Semana 12:** Evaluación y reflexión

- Presentaciones finales
- Coevaluación entre equipos
- Reflexión metacognitiva

---

## 📝 Instrumentos de evaluación distribuidos

| Instrumento | Semanas de aplicación | Peso total |
| :-- | :-- | :-- |
| **Rúbricas de actividades prácticas** | 1-11 | 25% |
| **Pruebas de configuración funcional** | 5, 8 | 50% |
| **Portfolio digital del proyecto** | 1-12 | 15% |
| **Presentación final + coevaluación** | 12 | 10% |


---

## ⚠️ Consideraciones especiales

**Flexibilidad curricular:**

- Las semanas 6-7 pueden intercambiarse según el nivel del grupo
- La semana 11 permite adaptación de contenidos según intereses
- Las evaluaciones parciales incluyen recuperación automática

**Recursos críticos:**

- Hardware disponible desde semana 1
- Acceso a laboratorio garantizado 5h/semana
- Conectividad a internet estable para VPN y DDNS
