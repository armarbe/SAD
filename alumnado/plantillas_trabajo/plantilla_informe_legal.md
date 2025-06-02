# Plantilla de Informe Legal - Auditoría de Cumplimiento Normativo

---

## Metadatos del documento

| Campo | Información |
|-------|-------------|
| **Título del informe** | Auditoría Legal - Proyecto SyAD |
| **Autor(es)** | [Nombres del equipo] |
| **Fecha de elaboración** | [DD/MM/AAAA] |
| **Última revisión** | [DD/MM/AAAA] |
| **Versión** | [v1.0] |
| **Empresa simulada** | [Nombre de la PYME] |
| **Actividad empresarial** | [Sector de la empresa] |

---

## 1. Resumen ejecutivo

### 1.1 Objeto del informe
> Descripción breve del propósito de esta auditoría legal en el contexto del proyecto de infraestructura segura para la PYME.

### 1.2 Alcance de la auditoría
- **Sistemas analizados:** [Lista de sistemas desplegados]
- **Normativas aplicadas:** RGPD, LOPDGDD, LSSI-CE, ISO 27001
- **Periodo de análisis:** [Fechas del proyecto]
- **Metodología:** [Análisis documental, técnico y normativo]

### 1.3 Conclusiones principales
- **Estado de cumplimiento general:** [Completo/Parcial/Deficiente]
- **Riesgos legales identificados:** [Número y severidad]
- **Medidas correctivas requeridas:** [Número de acciones necesarias]
- **Plazo de implementación:** [Estimación temporal]

---

## 2. Marco normativo de referencia

### 2.1 Reglamento General de Protección de Datos (RGPD)

**Referencia legal:** Reglamento (UE) 2016/679 del Parlamento Europeo y del Consejo, de 27 de abril de 2016
**Enlace oficial:** [https://eur-lex.europa.eu/legal-content/ES/TXT/?uri=CELEX%3A32016R0679](https://eur-lex.europa.eu/legal-content/ES/TXT/?uri=CELEX%3A32016R0679)

**Aplicabilidad al proyecto:**
- [X] Tratamiento de datos personales de empleados (acceso VPN)
- [X] Logs de sistemas con información personal
- [X] Datos de dispositivos IoT/domóticos
- [ ] Otros: [Especificar si aplica]

**Artículos clave aplicables:**
- **Art. 5** - Principios relativos al tratamiento
- **Art. 6** - Licitud del tratamiento
- **Art. 25** - Protección de datos desde el diseño y por defecto
- **Art. 32** - Seguridad del tratamiento
- **Art. 33** - Notificación de violaciones de seguridad
- **Art. 35** - Evaluación de impacto relativa a la protección de datos

### 2.2 Ley Orgánica de Protección de Datos y garantía de los derechos digitales (LOPDGDD)

**Referencia legal:** Ley Orgánica 3/2018, de 5 de diciembre
**BOE:** [https://www.boe.es/eli/es/lo/2018/12/05/3](https://www.boe.es/eli/es/lo/2018/12/05/3)

**Aplicabilidad al proyecto:**
- [X] Complementa y adapta el RGPD al derecho español
- [X] Derechos digitales de trabajadores (Art. 87-91)
- [X] Videovigilancia (si aplica)
- [X] Sistemas de información crediticia (si aplica)

**Artículos clave aplicables:**
- **Art. 25** - Análisis de riesgos
- **Art. 87** - Derecho a la intimidad y uso de dispositivos digitales
- **Art. 88** - Derecho a la desconexión digital
- **Art. 89** - Derecho a la intimidad frente al uso de dispositivos de videovigilancia

### 2.3 Ley de Servicios de la Sociedad de la Información y Comercio Electrónico (LSSI-CE)

**Referencia legal:** Ley 34/2002, de 11 de julio
**BOE:** [https://www.boe.es/eli/es/l/2002/07/11/34](https://www.boe.es/eli/es/l/2002/07/11/34)

**Aplicabilidad al proyecto:**
- [X] Servicios web empresariales
- [X] Comunicaciones comerciales electrónicas
- [X] Conservación de datos de tráfico
- [ ] Comercio electrónico (si la empresa vende online)

### 2.4 Normas técnicas de referencia

**ISO/IEC 27001:2013** - Sistemas de gestión de la seguridad de la información
**Esquema Nacional de Seguridad (ENS)** - Real Decreto 3/2010, de 8 de enero
**CCN-STIC** - Guías de seguridad del Centro Criptológico Nacional

---

## 3. Análisis de tratamientos de datos personales

### 3.1 Inventario de tratamientos identificados

#### Tratamiento 1: Acceso remoto VPN
| Campo | Información |
|-------|-------------|
| **Finalidad** | Acceso seguro de empleados en teletrabajo |
| **Base legal (Art. 6 RGPD)** | Interés legítimo / Ejecución de contrato laboral |
| **Categorías de datos** | Identificadores de usuario, direcciones IP, logs de conexión |
| **Categorías de interesados** | Empleados de la empresa |
| **Cesiones/transferencias** | No aplica |
| **Plazo de conservación** | [Especificar plazo] |
| **Medidas de seguridad** | Cifrado, autenticación, logs auditables |

#### Tratamiento 2: Videovigilancia (si aplica)
| Campo | Información |
|-------|-------------|
| **Finalidad** | Seguridad de las instalaciones |
| **Base legal (Art. 6 RGPD)** | Interés legítimo |
| **Categorías de datos** | Imágenes de personas |
| **Categorías de interesados** | Empleados, visitantes |
| **Cesiones/transferencias** | Fuerzas de seguridad (si es necesario) |
| **Plazo de conservación** | [Máximo 30 días según normativa] |
| **Medidas de seguridad** | Acceso restringido, cifrado de almacenamiento |

#### Tratamiento 3: Logs de sistemas
| Campo | Información |
|-------|-------------|
| **Finalidad** | Seguridad informática y auditoría |
| **Base legal (Art. 6 RGPD)** | Interés legítimo |
| **Categorías de datos** | IPs, usuarios, marcas temporales, acciones |
| **Categorías de interesados** | Empleados, usuarios de sistemas |
| **Cesiones/transferencias** | No aplica |
| **Plazo de conservación** | [Especificar plazo] |
| **Medidas de seguridad** | Control de acceso, integridad, backup |

### 3.2 Análisis de licitud (Art. 6 RGPD)

**Justificación de las bases legales utilizadas:**
- **Interés legítimo (Art. 6.1.f):** [Describir el test de proporcionalidad realizado]
- **Ejecución de contrato (Art. 6.1.b):** [Justificar la necesidad para el contrato laboral]
- **Cumplimiento de obligación legal (Art. 6.1.c):** [Si aplica, especificar normativa]

---

## 4. Identificación de figuras legales

### 4.1 Responsable del tratamiento

**Identificación:**
- **Denominación:** [Nombre de la empresa]
- **NIF/CIF:** [Número de identificación]
- **Dirección:** [Dirección completa]
- **Representante legal:** [Nombre y cargo]
- **Contacto DPO:** [Si aplica, datos del DPO]

**Responsabilidades principales:**
- [ ] Determinar los fines y medios del tratamiento
- [ ] Garantizar el cumplimiento del RGPD
- [ ] Implementar medidas técnicas y organizativas
- [ ] Notificar violaciones de seguridad
- [ ] Realizar evaluaciones de impacto si es necesario

### 4.2 Encargado del tratamiento (si aplica)

**Proveedores de servicios externos:**
| Proveedor | Servicio | Datos tratados | Ubicación | Contrato RGPD |
|-----------|----------|----------------|-----------|---------------|
| [Proveedor cloud] | Backup externo | [Tipo de datos] | [País] | [Sí/No] |
| [Proveedor ISP] | Conectividad | Logs de tráfico | España | [Sí/No] |

### 4.3 Interesados (data subjects)

**Categorías identificadas:**
- **Empleados:** [Número aproximado]
- **Visitantes:** [Si videovigilancia]
- **Usuarios externos:** [Si servicios web públicos]

**Derechos aplicables:**
- [ ] Derecho de acceso (Art. 15)
- [ ] Derecho de rectificación (Art. 16)
- [ ] Derecho de supresión (Art. 17)
- [ ] Derecho de limitación (Art. 18)
- [ ] Derecho de portabilidad (Art. 20)
- [ ] Derecho de oposición (Art. 21)

---

## 5. Evaluación de medidas técnicas y organizativas

### 5.1 Medidas técnicas implementadas

#### Cifrado
- [ ] **Datos en tránsito:** TLS/SSL para comunicaciones web, VPN cifrada
- [ ] **Datos en reposo:** Cifrado de discos/particiones sensibles
- [ ] **Copias de seguridad:** Backup cifrado

#### Control de acceso
- [ ] **Autenticación fuerte:** Certificados, claves SSH, 2FA
- [ ] **Autorización:** Permisos mínimos necesarios
- [ ] **Auditoría:** Logs de acceso y actividades

#### Seguridad de red
- [ ] **Firewall:** Reglas restrictivas, denegación por defecto
- [ ] **Segmentación:** VLANs, separación de redes
- [ ] **Monitorización:** IDS/IPS, detección de anomalías

#### Gestión de vulnerabilidades
- [ ] **Actualizaciones:** Parches de seguridad automáticos
- [ ] **Antimalware:** Protección contra virus y malware
- [ ] **Backup:** Copias de seguridad regulares y probadas

### 5.2 Medidas organizativas implementadas

#### Políticas y procedimientos
- [ ] **Política de seguridad:** Documentada y aprobada
- [ ] **Procedimientos de backup:** Definidos y probados
- [ ] **Plan de respuesta a incidentes:** Actualizado
- [ ] **Política de contraseñas:** Implementada

#### Formación y concienciación
- [ ] **Formación en RGPD:** Personal sensibilizado
- [ ] **Formación en seguridad:** Mejores prácticas
- [ ] **Simulacros:** Ejercicios de respuesta a incidentes

#### Gestión de accesos
- [ ] **Alta/baja de usuarios:** Procedimientos definidos
- [ ] **Revisión periódica:** Auditoría de permisos
- [ ] **Segregación de funciones:** Separación de responsabilidades

---

## 6. Análisis de riesgos de protección de datos

### 6.1 Riesgos identificados

#### Riesgo 1: Acceso no autorizado a datos personales
- **Probabilidad:** [Alta/Media/Baja]
- **Impacto:** [Alto/Medio/Bajo]
- **Medidas mitigadoras:** Control de acceso, autenticación fuerte, monitorización
- **Riesgo residual:** [Alto/Medio/Bajo]

#### Riesgo 2: Pérdida o destrucción de datos
- **Probabilidad:** [Alta/Media/Baja]
- **Impacto:** [Alto/Medio/Bajo]
- **Medidas mitigadoras:** Backup automático, RAID, procedimientos de recuperación
- **Riesgo residual:** [Alto/Medio/Bajo]

#### Riesgo 3: Modificación no autorizada
- **Probabilidad:** [Alta/Media/Baja]
- **Impacto:** [Alto/Medio/Bajo]
- **Medidas mitigadoras:** Control de versiones, logs de auditoría, checksums
- **Riesgo residual:** [Alto/Medio/Bajo]

### 6.2 Matriz de riesgo

| Riesgo | Probabilidad | Impacto | Nivel | Medidas | Estado |
|--------|--------------|---------|-------|---------|--------|
| Acceso no autorizado | [P] | [I] | [Alto/Medio/Bajo] | [Medidas] | [Implementado/Pendiente] |
| Pérdida de datos | [P] | [I] | [Alto/Medio/Bajo] | [Medidas] | [Implementado/Pendiente] |
| Modificación no autorizada | [P] | [I] | [Alto/Medio/Bajo] | [Medidas] | [Implementado/Pendiente] |

---

## 7. Cumplimiento de obligaciones específicas

### 7.1 Información a los interesados (Art. 13-14 RGPD)

#### Política de privacidad para empleados
```

INFORMACIÓN SOBRE TRATAMIENTO DE DATOS PERSONALES

Responsable: [Nombre empresa]
Finalidad: Gestión del acceso remoto y seguridad informática
Base legal: Interés legítimo y ejecución del contrato laboral
Destinatarios: No se ceden datos a terceros
Conservación: [Plazo específico]
Derechos: Acceso, rectificación, supresión, limitación, oposición
Contacto DPO: [Si aplica]
Reclamaciones: Agencia Española de Protección de Datos

```

### 7.2 Registro de actividades de tratamiento (Art. 30 RGPD)

**Entrada del registro:**
```

Denominación: Acceso remoto VPN
Finalidad: Permitir teletrabajo seguro
Base legal: Art. 6.1.b) Ejecución de contrato
Categorías de interesados: Empleados
Categorías de datos: Identificación, logs de conexión
Destinatarios: No aplica
Transferencias internacionales: No
Plazos de supresión: [Especificar]
Medidas de seguridad: Cifrado, autenticación, logs

```

### 7.3 Notificación de violaciones de seguridad (Art. 33-34 RGPD)

**Procedimiento establecido:**
1. **Detección** (< 24 horas) → Evaluación de la violación
2. **Notificación a AEPD** (< 72 horas) → Si riesgo para derechos
3. **Comunicación a interesados** (sin dilación) → Si alto riesgo
4. **Documentación** → Registro de todas las violaciones

**Plantilla de notificación:**
```

1. Descripción de la violación
2. Categorías y número de interesados afectados
3. Categorías y número de registros afectados
4. Consecuencias probables
5. Medidas adoptadas o propuestas
6. Contacto del DPO (si aplica)
```

---

## 8. Análisis de cumplimiento LSSI-CE

### 8.1 Servicios de la sociedad de la información identificados

- [ ] **Página web corporativa:** [URL si existe]
- [ ] **Portal de empleados:** [Acceso interno]
- [ ] **Servicios cloud:** [Especificar si aplica]
- [ ] **Comunicaciones electrónicas:** [Email, newsletter]

### 8.2 Obligaciones de información (Art. 10 LSSI-CE)

**Información general obligatoria:**
- [ ] Denominación social
- [ ] Residencia o domicilio
- [ ] Dirección de correo electrónico
- [ ] Datos de inscripción registral
- [ ] NIF/CIF
- [ ] Datos del colegio profesional (si aplica)

### 8.3 Conservación de datos de conexión (Art. 12 LSSI-CE)

**Datos conservados:**
- Logs de acceso web
- Datos de tráfico de red
- Identificadores de sesión

**Plazo de conservación:** 12 meses
**Finalidad:** Seguridad y prevención de delitos
**Acceso:** Solo autoridades competentes con orden judicial

---

## 9. Recomendaciones y plan de acción

### 9.1 Deficiencias identificadas

#### Deficiencia 1: [Descripción]
- **Gravedad:** [Alta/Media/Baja]
- **Riesgo legal:** [Descripción del riesgo]
- **Acción correctiva:** [Medida a tomar]
- **Responsable:** [Persona responsable]
- **Plazo:** [Fecha límite]

#### Deficiencia 2: [Descripción]
- **Gravedad:** [Alta/Media/Baja]
- **Riesgo legal:** [Descripción del riesgo]
- **Acción correctiva:** [Medida a tomar]
- **Responsable:** [Persona responsable]
- **Plazo:** [Fecha límite]

### 9.2 Mejoras recomendadas

- [ ] **Implementar DPO:** Si los tratamientos lo requieren
- [ ] **Evaluación de impacto:** Para tratamientos de alto riesgo
- [ ] **Certificación ISO 27001:** Para demostrar buenas prácticas
- [ ] **Auditoría externa:** Validación independiente del cumplimiento
- [ ] **Formación específica:** Personal especializado en protección de datos

### 9.3 Cronograma de implementación

| Acción | Responsable | Inicio | Fin | Estado |
|--------|-------------|--------|-----|--------|
| [Acción 1] | [Nombre] | [DD/MM] | [DD/MM] | [Pendiente/En curso/Completado] |
| [Acción 2] | [Nombre] | [DD/MM] | [DD/MM] | [Pendiente/En curso/Completado] |
| [Acción 3] | [Nombre] | [DD/MM] | [DD/MM] | [Pendiente/En curso/Completado] |

---

## 10. Documentación y evidencias

### 10.1 Documentos generados

- [ ] **Política de privacidad** actualizada
- [ ] **Avisos legales** para web corporativa
- [ ] **Registro de actividades** de tratamiento
- [ ] **Procedimiento de ejercicio** de derechos
- [ ] **Plan de respuesta** a violaciones de seguridad
- [ ] **Contratos con encargados** (si aplica)

### 10.2 Evidencias técnicas

- [ ] **Configuraciones de seguridad** documentadas
- [ ] **Logs de auditoría** configurados
- [ ] **Certificados SSL/TLS** instalados
- [ ] **Backups cifrados** funcionando
- [ ] **Accesos con autenticación** fuerte

### 10.3 Formación impartida

- [ ] **Sesión RGPD básico** para todo el personal
- [ ] **Formación técnica** en seguridad informática
- [ ] **Procedimientos de incidentes** comunicados
- [ ] **Contactos de escalado** establecidos

---

## 11. Conclusiones y certificación

### 11.1 Nivel de cumplimiento alcanzado

**Evaluación global:**
- **RGPD:** [Completo/Parcial con observaciones/Deficiente]
- **LOPDGDD:** [Completo/Parcial con observaciones/Deficiente]
- **LSSI-CE:** [Completo/Parcial con observaciones/Deficiente]
- **ISO 27001:** [Conforme/No conforme]

### 11.2 Riesgos residuales

**Riesgos que permanecen tras las medidas implementadas:**
- [Riesgo 1]: [Descripción y justificación de aceptación]
- [Riesgo 2]: [Descripción y justificación de aceptación]

### 11.3 Certificación de cumplimiento

> Certifico que la infraestructura tecnológica implementada en el proyecto PYME SecureHome cumple con los requisitos legales aplicables en materia de protección de datos y servicios de la sociedad de la información, con las observaciones y recomendaciones indicadas en este informe.

**Auditor responsable:** [Nombre]
**Fecha:** [DD/MM/AAAA]
**Firma:** [Firma digital]

---

## 12. Anexos

### Anexo A: Normativa aplicable completa
- [Reglamento (UE) 2016/679 - RGPD](https://eur-lex.europa.eu/legal-content/ES/TXT/?uri=CELEX%3A32016R0679)
- [Ley Orgánica 3/2018 - LOPDGDD](https://www.boe.es/eli/es/lo/2018/12/05/3)
- [Ley 34/2002 - LSSI-CE](https://www.boe.es/eli/es/l/2002/07/11/34)
- [Real Decreto 3/2010 - ENS](https://www.boe.es/eli/es/rd/2010/01/08/3)

### Anexo B: Plantillas de documentos
- Política de privacidad modelo
- Aviso legal tipo
- Formulario de ejercicio de derechos
- Plantilla de notificación de violaciones

### Anexo C: Configuraciones técnicas
- Extractos de configuración de servicios
- Capturas de pantalla de medidas implementadas
- Resultados de auditorías técnicas

---

## Control de versiones

| Versión | Fecha | Autor | Cambios |
|---------|-------|-------|---------|
| v1.0 | [DD/MM/AAAA] | [Nombre] | Versión inicial |
| v1.1 | [DD/MM/AAAA] | [Nombre] | [Descripción cambios] |
