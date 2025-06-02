# Plantilla de Análisis de Riesgos de Seguridad
**Nota importante:** Este análisis debe actualizarse cuando se produzcan cambios significativos en la infraestructura, amenazas del entorno o marco normativo aplicable.
---

## Metadatos del documento

| Campo | Información |
|-------|-------------|
| **Título del análisis** | [Análisis de riesgos - Nombre del sistema/servicio] |
| **Equipo responsable** | [Nombres del equipo] |
| **Fecha de análisis** | [DD/MM/AAAA] |
| **Última revisión** | [DD/MM/AAAA] |
| **Versión** | [v1.0] |
| **Alcance del análisis** | [Descripción del sistema analizado] |
| **Estado** | [Borrador / En revisión / Aprobado] |

---

## 1. Resumen ejecutivo

### 1.1 Contexto del análisis
> Descripción breve del sistema, servicio o infraestructura analizada en el contexto del proyecto.

### 1.2 Metodología aplicada
- **Estándar de referencia:** ISO 27005 (adaptado para entorno educativo)
- **Alcance temporal:** [Periodo cubierto]
- **Participantes:** [Roles involucrados]

### 1.3 Resumen de hallazgos principales
- **Riesgos críticos identificados:** [Número]
- **Riesgos altos:** [Número]
- **Riesgos medios:** [Número]
- **Riesgos bajos:** [Número]

---

## 2. Inventario de activos

### 2.1 Activos de información
| ID | Activo | Tipo | Criticidad | Propietario | Ubicación |
|----|--------|------|------------|-------------|-----------|
| AI-01 | [Nombre del activo] | [Hardware/Software/Datos] | [C/A/M/B] | [Responsable] | [Ubicación física/lógica] |
| AI-02 | | | | | |
| AI-03 | | | | | |

**Leyenda de criticidad:**
- **C:** Crítico - Impacto muy alto en la organización
- **A:** Alto - Impacto significativo
- **M:** Medio - Impacto moderado  
- **B:** Bajo - Impacto menor

### 2.2 Valoración de activos

#### Criterios de valoración
**Confidencialidad:**
- 4: Muy alto (información clasificada)
- 3: Alto (información sensible empresarial)
- 2: Medio (información interna)
- 1: Bajo (información pública)

**Integridad:**
- 4: Muy alto (datos críticos para el negocio)
- 3: Alto (datos importantes)
- 2: Medio (datos de respaldo disponible)
- 1: Bajo (datos fácilmente recuperables)

**Disponibilidad:**
- 4: Muy alto (disponibilidad 24/7 crítica)
- 3: Alto (interrupciones impactan el negocio)
- 2: Medio (tolerancia a interrupciones cortas)
- 1: Bajo (interrupciones no críticas)

### 2.3 Matriz de valoración de activos
| Activo | Confidencialidad | Integridad | Disponibilidad | Valor Total | Criticidad |
|--------|------------------|------------|-----------------|-------------|------------|
| [Activo 1] | [1-4] | [1-4] | [1-4] | [3-12] | [C/A/M/B] |
| [Activo 2] | | | | | |

---

## 3. Identificación de amenazas

### 3.1 Catálogo de amenazas

#### 3.1.1 Amenazas naturales
| ID | Amenaza | Descripción | Probabilidad | Activos afectados |
|----|---------|-------------|--------------|-------------------|
| AN-01 | Incendio | Fuego en instalaciones | [1-5] | [Lista de activos] |
| AN-02 | Inundación | Entrada de agua | [1-5] | [Lista de activos] |
| AN-03 | Corte eléctrico | Falta de suministro eléctrico | [1-5] | [Lista de activos] |

#### 3.1.2 Amenazas humanas accidentales
| ID | Amenaza | Descripción | Probabilidad | Activos afectados |
|----|---------|-------------|--------------|-------------------|
| HA-01 | Error de configuración | Configuración incorrecta de servicios | [1-5] | [Lista de activos] |
| HA-02 | Borrado accidental | Eliminación no intencionada de datos | [1-5] | [Lista de activos] |
| HA-03 | Uso inadecuado | Mal uso de sistemas o aplicaciones | [1-5] | [Lista de activos] |

#### 3.1.3 Amenazas humanas intencionadas
| ID | Amenaza | Descripción | Probabilidad | Activos afectados |
|----|---------|-------------|--------------|-------------------|
| HI-01 | Acceso no autorizado | Intrusión en sistemas | [1-5] | [Lista de activos] |
| HI-02 | Malware | Virus, troyanos, ransomware | [1-5] | [Lista de activos] |
| HI-03 | Ataques de denegación | DDoS, DoS | [1-5] | [Lista de activos] |
| HI-04 | Ingeniería social | Manipulación para obtener información | [1-5] | [Lista de activos] |
| HI-05 | Ataques de fuerza bruta | Intentos masivos de acceso | [1-5] | [Lista de activos] |

#### 3.1.4 Amenazas técnicas
| ID | Amenaza | Descripción | Probabilidad | Activos afectados |
|----|---------|-------------|--------------|-------------------|
| AT-01 | Fallo de hardware | Avería de componentes físicos | [1-5] | [Lista de activos] |
| AT-02 | Fallo de software | Errores en aplicaciones o SO | [1-5] | [Lista de activos] |
| AT-03 | Saturación de recursos | Agotamiento de CPU, RAM, disco | [1-5] | [Lista de activos] |

**Escala de probabilidad:**
- 1: Muy baja (< 10%)
- 2: Baja (10-30%)
- 3: Media (30-60%)
- 4: Alta (60-85%)
- 5: Muy alta (> 85%)

---

## 4. Identificación de vulnerabilidades

### 4.1 Vulnerabilidades por categoría

#### 4.1.1 Vulnerabilidades de configuración
| ID | Vulnerabilidad | Descripción | Activo afectado | Facilidad de explotación |
|----|----------------|-------------|-----------------|-------------------------|
| VC-01 | Contraseñas débiles | Passwords por defecto o simples | [Activo] | [1-5] |
| VC-02 | Servicios innecesarios | Servicios activos sin uso | [Activo] | [1-5] |
| VC-03 | Permisos excesivos | Privilegios superiores a los necesarios | [Activo] | [1-5] |

#### 4.1.2 Vulnerabilidades de software
| ID | Vulnerabilidad | Descripción | Activo afectado | Facilidad de explotación |
|----|----------------|-------------|-----------------|-------------------------|
| VS-01 | Software desactualizado | Versiones con vulnerabilidades conocidas | [Activo] | [1-5] |
| VS-02 | Falta de validación | Input sin sanitizar | [Activo] | [1-5] |

#### 4.1.3 Vulnerabilidades físicas
| ID | Vulnerabilidad | Descripción | Activo afectado | Facilidad de explotación |
|----|----------------|-------------|-----------------|-------------------------|
| VF-01 | Acceso físico sin control | Dispositivos accesibles | [Activo] | [1-5] |
| VF-02 | Falta de redundancia | Sin sistemas de backup | [Activo] | [1-5] |

**Escala de facilidad de explotación:**
- 1: Muy difícil (requiere conocimientos avanzados y herramientas especializadas)
- 2: Difícil (requiere conocimientos técnicos)
- 3: Media (requiere conocimientos básicos)
- 4: Fácil (herramientas disponibles públicamente)
- 5: Muy fácil (sin conocimientos técnicos necesarios)

---

## 5. Análisis de riesgos

### 5.1 Matriz de riesgos

| ID Riesgo | Amenaza | Vulnerabilidad | Activo | Probabilidad | Impacto | Riesgo | Nivel |
|-----------|---------|----------------|--------|--------------|---------|--------|-------|
| R-001 | [ID amenaza] | [ID vulnerabilidad] | [Activo] | [1-5] | [1-5] | [1-25] | [Muy bajo/Bajo/Medio/Alto/Muy alto] |
| R-002 | | | | | | | |
| R-003 | | | | | | | |

**Cálculo del riesgo:** Riesgo = Probabilidad × Impacto

**Clasificación de niveles de riesgo:**
- **Muy alto (21-25):** Riesgo inaceptable, requiere acción inmediata
- **Alto (16-20):** Riesgo alto, requiere plan de mitigación prioritario
- **Medio (11-15):** Riesgo moderado, requiere medidas de control
- **Bajo (6-10):** Riesgo aceptable con controles básicos
- **Muy bajo (1-5):** Riesgo muy bajo, monitorización periódica

### 5.2 Escala de impacto
**Criterios de evaluación del impacto:**

| Nivel | Confidencialidad | Integridad | Disponibilidad | Impacto económico |
|-------|------------------|------------|-----------------|-------------------|
| **5 - Muy alto** | Divulgación masiva de información clasificada | Corrupción crítica de datos | Interrupción > 48h | > 50.000€ |
| **4 - Alto** | Divulgación de información sensible | Corrupción importante de datos | Interrupción 24-48h | 10.000-50.000€ |
| **3 - Medio** | Divulgación de información interna | Corrupción parcial de datos | Interrupción 8-24h | 2.000-10.000€ |
| **2 - Bajo** | Divulgación de información poco sensible | Corrupción menor de datos | Interrupción 2-8h | 500-2.000€ |
| **1 - Muy bajo** | Sin impacto en confidencialidad | Sin impacto en integridad | Interrupción < 2h | < 500€ |

---

## 6. Evaluación del riesgo

### 6.1 Riesgos por nivel

#### 6.1.1 Riesgos críticos y altos (requieren acción inmediata)
| ID | Descripción | Nivel | Justificación | Plazo de acción |
|----|-------------|-------|---------------|-----------------|
| R-001 | [Descripción del riesgo] | Alto/Muy alto | [Por qué es crítico] | [Inmediato/Corto plazo] |

#### 6.1.2 Riesgos medios (requieren planificación)
| ID | Descripción | Nivel | Acciones propuestas | Plazo |
|----|-------------|-------|-------------------|-------|
| R-XXX | [Descripción del riesgo] | Medio | [Medidas a tomar] | [Medio plazo] |

#### 6.1.3 Riesgos bajos (monitorización)
| ID | Descripción | Nivel | Seguimiento propuesto | Frecuencia |
|----|-------------|-------|---------------------|-----------|
| R-XXX | [Descripción del riesgo] | Bajo/Muy bajo | [Tipo de monitorización] | [Periódica] |

---

## 7. Plan de tratamiento de riesgos

### 7.1 Estrategias de tratamiento

**Para cada riesgo identificado, seleccionar una estrategia:**
- **Mitigar:** Reducir probabilidad o impacto
- **Transferir:** Compartir o trasladar el riesgo (seguros, outsourcing)
- **Evitar:** Eliminar la actividad que genera el riesgo
- **Aceptar:** Asumir el riesgo (solo para riesgos bajos)

### 7.2 Medidas de mitigación

#### 7.2.1 Controles preventivos
| ID Control | Descripción | Riesgos mitigados | Responsable | Plazo | Coste estimado |
|------------|-------------|-------------------|-------------|-------|----------------|
| CP-01 | [Medida preventiva] | [R-001, R-003] | [Responsable] | [Fecha] | [Coste] |
| CP-02 | | | | | |

#### 7.2.2 Controles detectivos
| ID Control | Descripción | Riesgos mitigados | Responsable | Plazo | Coste estimado |
|------------|-------------|-------------------|-------------|-------|----------------|
| CD-01 | [Medida detectiva] | [R-002, R-005] | [Responsable] | [Fecha] | [Coste] |
| CD-02 | | | | | |

#### 7.2.3 Controles correctivos
| ID Control | Descripción | Riesgos mitigados | Responsable | Plazo | Coste estimado |
|------------|-------------|-------------------|-------------|-------|----------------|
| CC-01 | [Medida correctiva] | [R-004, R-006] | [Responsable] | [Fecha] | [Coste] |
| CC-02 | | | | | |

---

## 8. Plan de implementación

### 8.1 Cronograma de implementación

| Fase | Controles a implementar | Inicio | Fin | Responsable | Recursos necesarios |
|------|-------------------------|--------|-----|-------------|---------------------|
| **Fase 1** | [Controles críticos] | [DD/MM] | [DD/MM] | [Responsable] | [Recursos] |
| **Fase 2** | [Controles importantes] | [DD/MM] | [DD/MM] | [Responsable] | [Recursos] |
| **Fase 3** | [Controles complementarios] | [DD/MM] | [DD/MM] | [Responsable] | [Recursos] |

### 8.2 Presupuesto estimado

| Categoría | Descripción | Coste |
|-----------|-------------|-------|
| **Software** | Licencias, herramientas | [Coste] € |
| **Hardware** | Equipos, componentes | [Coste] € |
| **Formación** | Capacitación del personal | [Coste] € |
| **Servicios externos** | Consultoría, auditorías | [Coste] € |
| **TOTAL** | | [Coste total] € |

---

## 9. Monitorización y revisión

### 9.1 Indicadores de riesgo (KRI)

| Indicador | Descripción | Valor objetivo | Frecuencia de medición | Responsable |
|-----------|-------------|----------------|------------------------|-------------|
| [KRI-01] | [Métrica de seguridad] | [Valor] | [Diaria/Semanal] | [Responsable] |
| [KRI-02] | | | | |

### 9.2 Programa de revisiones

- **Revisión mensual:** Seguimiento de indicadores y controles
- **Revisión trimestral:** Evaluación de nuevas amenazas y vulnerabilidades
- **Revisión anual:** Actualización completa del análisis de riesgos

### 9.3 Gestión de incidentes

**Procedimiento de escalado:**
1. **Nivel 1:** Técnico local (< 2 horas)
2. **Nivel 2:** Supervisor técnico (< 4 horas)
3. **Nivel 3:** Responsable de seguridad (< 8 horas)
4. **Nivel 4:** Dirección (> 8 horas)

---

## 10. Cumplimiento normativo

### 10.1 Requisitos legales aplicables

| Normativa | Artículos aplicables | Controles relacionados | Estado cumplimiento |
|-----------|---------------------|------------------------|-------------------|
| **RGPD** | Art. 32 - Seguridad del tratamiento | [CP-01, CD-02] | [Completo/Parcial/Pendiente] |
| **LOPDGDD** | Art. 25 - Análisis de riesgos | [Este documento] | [Completo/Parcial/Pendiente] |
| **ISO 27001** | A.12.6 - Gestión de vulnerabilidades | [CP-02, CD-01] | [Completo/Parcial/Pendiente] |

### 10.2 Evidencias de cumplimiento

- [ ] Documentación del análisis de riesgos completada
- [ ] Medidas de seguridad implementadas
- [ ] Procedimientos de monitorización establecidos
- [ ] Personal formado en gestión de riesgos

---

## 11. Anexos

### Anexo A: Metodología detallada
[Descripción de la metodología utilizada]

### Anexo B: Herramientas utilizadas
- **Herramienta 1:** [Nmap para escaneo de vulnerabilidades]
- **Herramienta 2:** [OpenVAS para análisis automático]

### Anexo C: Referencias bibliográficas
- ISO/IEC 27005:2018 - Information security risk management
- NIST SP 800-30 - Guide for Conducting Risk Assessments
- ENISA - Risk Management/Risk Assessment Methods and Tools

---

## 12. Control de versiones

| Versión | Fecha | Autor | Cambios realizados |
|---------|-------|-------|-------------------|
| v1.0 | [DD/MM/AAAA] | [Autor] | Versión inicial |
| v1.1 | [DD/MM/AAAA] | [Autor] | [Descripción de cambios] |

---

## 13. Aprobaciones

| Rol | Nombre | Fecha | Firma |
|-----|--------|-------|-------|
| **Responsable de seguridad** | [Nombre] | [DD/MM/AAAA] | [Firma] |
| **Responsable del proyecto** | [Nombre] | [DD/MM/AAAA] | [Firma] |
| **Revisor técnico** | [Nombre] | [DD/MM/AAAA] | [Firma] |
