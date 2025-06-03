# 📊 Evaluación

## **Instrumentos de evaluación**

### **Rúbricas como instrumento principal**

Siguiendo las directrices del **Gobierno de Canarias sobre rúbricas competenciales** y la investigación sobre **evaluación basada en evidencias**, se implementan rúbricas específicas que incorporan descriptores operativos vinculados a las competencias clave y facilitan la evaluación de aprendizajes mediante criterios de evaluación claramente definidos.

#### **Rúbrica general del proyecto**

| **Criterio de Evaluación** | **Excelente (9-10)** | **Bueno (7-8)** | **Aceptable (5-6)** | **Insuficiente (0-4)** | **RA** | **Peso** |
|---------------------------|---------------------|-----------------|-------------------|---------------------|--------|----------|
| **Seguridad inicial y políticas** | Implementa todas las medidas de seguridad, documenta políticas completas y justifica decisiones técnicas | Implementa la mayoría de medidas con documentación adecuada y justificación básica | Implementa medidas básicas con documentación mínima | No implementa medidas suficientes o documentación inadecuada | RA1 | 15% |
| **Sistemas de detección activa** | Configura fail2ban con reglas personalizadas, documenta anatomía de ataques y implementa medidas preventivas | Configura fail2ban correctamente y documenta medidas básicas de prevención | Configuración básica de fail2ban con documentación mínima | Configuración incorrecta o sin documentación | RA2 | 15% |
| **Acceso remoto seguro** | Configura múltiples protocolos VPN, implementa autenticación robusta y optimiza rendimiento | Configura VPN funcional con autenticación adecuada | Configuración básica de VPN operativa | VPN no funcional o insegura | RA3 | 20% |
| **Cortafuegos y filtrado** | Diseña arquitectura completa de filtrado, documenta reglas y justifica decisiones de seguridad | Configura cortafuegos funcional con documentación adecuada | Configuración básica operativa | Configuración insuficiente o no funcional | RA4 | 15% |
| **Proxy inverso y balanceo** | Implementa proxy con SSL, balanceo de carga y protección anti-DDoS | Configura proxy inverso funcional con SSL básico | Proxy básico operativo | Proxy no funcional o inseguro | RA5 | 15% |
| **Alta disponibilidad** | Implementa soluciones completas con Docker, DDNS y documenta estrategias de recuperación | Configura servicios en contenedores con DDNS funcional | Implementación básica de contenedores | Soluciones no funcionales o inadecuadas | RA6 | 15% |
| **Legislación** |Realiza un estudio completo de toda la normativa aplicable y revisa el ENS | Identifica si se cumplen las principales normativas | Estudio básico de normativa | Faltan normativas por estudiar | RA7 | 5% |

#### **Rúbricas específicas por competencia técnica**

**Rúbrica RA3 - Acceso remoto seguro (Ejemplo detallado)**

| **Indicador** | **Nivel 4 (9-10)** | **Nivel 3 (7-8)** | **Nivel 2 (5-6)** | **Nivel 1 (0-4)** |
|---------------|-------------------|------------------|------------------|------------------|
| **Configuración OpenVPN** | Servidor completo con certificados propios, múltiples clientes, configuración optimizada | Servidor funcional con certificados, configuración estándar | Configuración básica operativa | No funcional o insegura |
| **Configuración WireGuard** | Implementación completa con keys propias, múltiples peers, optimización de rendimiento | Configuración funcional estándar | Configuración básica operativa | No funcional |
| **Métodos de autenticación** | Implementa 2FA, certificados personalizados y políticas de acceso | Autenticación con certificados estándar | Autenticación básica por usuario/contraseña | Sin autenticación adecuada |
| **Documentación técnica** | Manual completo con diagramas, troubleshooting y procedimientos | Documentación adecuada con procedimientos básicos | Documentación mínima | Sin documentación o inadecuada |
| **Pruebas de conectividad** | Pruebas exhaustivas desde múltiples ubicaciones con métricas de rendimiento | Pruebas básicas de conectividad documentadas | Verificación mínima de funcionamiento | Sin pruebas o no funcional |

### **Instrumentos complementarios**

#### **1. Portfolio digital**
**Herramienta**: GitHub/GitLab personal del estudiante
- **Contenido**: Documentación técnica, scripts, configuraciones, reflexiones
- **Evaluación continua**: Commits regulares, evolución del proyecto
- **Peso**: 15% de la nota final

#### **2. Cuestionarios técnicos**
**Modalidad**: Evaluación automática mediante scripts de verificación
- **RA1-RA2**: Verificación de configuraciones de seguridad
- **RA3**: Tests de conectividad VPN automatizados  
- **RA4-RA5**: Validación de reglas de cortafuegos y proxy
- **RA6**: Comprobación de servicios en contenedores

#### **3. Presentaciones técnicas**
**Formato**: Presentación ante "comité empresarial" simulado
- **Duración**: 15 minutos presentación + 10 minutos preguntas
- **Contenido**: Solución integral, justificación técnica, demostración en vivo
- **Evaluación**: Competencias comunicativas y dominio técnico

#### **4. Evaluación por pares (Coevaluación)**
**Metodología**: Evaluación entre equipos utilizando rúbricas específicas
- **Momento**: Presentaciones intermedias (semanas 5, 8)
- **Criterios**: Claridad técnica, documentación, funcionalidad
- **Peso**: 10% de la evaluación de cada fase

---

## **Criterios de calificación**

### **Sistema de calificación por competencias**

Basándose en los **lineamientos socio-formativos basados en evidencias**, el sistema de calificación integra:

#### **Distribución de pesos por instrumento**

| **Instrumento de evaluación** | **Peso** | **Momento de evaluación** | **RA evaluados** |
|------------------------------|----------|---------------------------|------------------|
| **Evaluaciones parciales** | 50% | Semanas 5, 10 | RA1-RA4 |
| **Portfolio digital** | 15% | Continuo | Todos los RA |
| **Entrega final** | 25% | Semana 12 | RA5-RA6 + Integración |
| **Evaluación por pares** | 10% | Semanas 5, 9, 12 | Transversales |

#### **Criterios de progresión competencial**

**Nivel 1 (Inicial - 0-4 puntos)**
- Conocimiento teórico básico sin aplicación práctica
- Configuraciones no funcionales o con errores graves de seguridad
- Documentación inexistente o inadecuada

**Nivel 2 (En desarrollo - 5-6 puntos)**
- Aplicación básica de conocimientos con configuraciones operativas
- Implementación de medidas de seguridad fundamentales
- Documentación mínima pero presente

**Nivel 3 (Competente - 7-8 puntos)**
- Dominio sólido con configuraciones funcionales y seguras
- Justificación técnica adecuada de las decisiones
- Documentación completa y estructurada

**Nivel 4 (Experto - 9-10 puntos)**
- Implementación avanzada con optimizaciones y mejores prácticas
- Innovación en soluciones y análisis crítico
- Documentación profesional con valor añadido

### **Criterios de recuperación**

**Evaluación continua**: Permite recuperación inmediata de competencias no alcanzadas
- **Reentrega**: Posibilidad de mejorar entregas parciales hasta semana 11
- **Tutorías**: Sesiones personalizadas para resolver deficiencias específicas
- **Evaluación extraordinaria**: Proyecto alternativo para casos excepcionales

---

## **Evidencias a calificar**

### **Clasificación de evidencias según enfoque socio-formativo**

#### **1. Evidencias de desempeño (Hacer - 45%)**

**RA1: Seguridad inicial**  
	✓ Instalación segura de DietPi documentada  
	✓ Configuración de políticas de contraseñas funcional   
	✓ Desactivación de accesos root por SSH verificada

**RA2: Seguridad activa**   
	✓ Configuración de fail2ban operativa con logs de funcionamiento   
	✓ Bloqueo automático de intentos de intrusión documentado   
	✓ Políticas de detección personalizadas implementadas

**RA3: Acceso remoto**   
	✓ Servidor OpenVPN/WireGuard funcional con conexiones exitosas   
	✓ Certificados y autenticación configurados correctamente   
	✓ Conectividad desde múltiples ubicaciones verificada

**RA4: Cortafuegos**   
	✓ Reglas de iptables funcionales documentadas   
	✓ Pi-hole operativo con filtrado DNS activo   
	✓ Arquitectura de seguridad perimetral implementada

**RA5: Proxy inverso**   
	✓ Nginx Proxy Manager funcional con SSL   
	✓ Balanceo de carga entre servidores backend   
	✓ Protección anti-DDoS configurada

**RA6: Alta disponibilidad**   
	✓ Servicios críticos ejecutándose en contenedores Docker   
	✓ Cloudflare DDNS actualiza IP pública automáticamente   
	✓ HomeAssistant integrado con protocolos offline

**RA7: Legislación**   
	✓ RGPD   
	✓ LOPDGDD   
	✓ ISO 27001  
 	✓ LSSI

#### **2. Evidencias de conocimiento (Saber - 40%)**

**Documentación técnica profesional**
- Manual de instalación y configuración paso a paso
- Análisis comparativo de tecnologías (OpenVPN vs WireGuard)
- Documentación de arquitectura de seguridad con diagramas
- Procedimientos de troubleshooting y resolución de incidencias
- Plan de contingencias y recuperación ante desastres

**Pruebas teóricas integradas**
- Cuestionarios de verificación automática de configuraciones
- Análisis de logs y identificación de anomalías
- Justificación técnica de decisiones de diseño

#### **3. Evidencias de actitud (Ser/Estar - 15%)**

**Competencias transversales**
- **Trabajo en equipo**: Colaboración efectiva en proyecto grupal
- **Organización**: Gestión eficiente del tiempo y recursos
- **Innovación**: Propuestas de mejora y soluciones creativas
- **Responsabilidad**: Cumplimiento de normativas de seguridad
- **Comunicación**: Presentación clara de soluciones técnicas

**Autoevaluación y reflexión**
- Bitácora de aprendizaje con reflexiones semanales
- Autoevaluación de progreso competencial
- Identificación de áreas de mejora y plan de acción

### **Sistema de registro de evidencias**

**Herramienta tecnológica**: Plataforma integrada
- **GitHub**: Repositorio de código y documentación con control de versiones
- **Aules (Moodle)**: Portfolio digital con rúbricas integradas
- **Scripts automáticos**: Verificación continua de configuraciones
- **Dashboard**: Seguimiento en tiempo real del progreso competencial

**Criterios de validación de evidencias**   
	✓ **Autenticidad**: Evidencias propias verificables   
	✓ **Actualidad**: Reflejan el nivel competencial actual   
	✓ **Suficiencia**: Cantidad adecuada para demostrar competencia   
	✓ **Pertinencia**: Directamente relacionadas con criterios de evaluación

### **Cronograma de recogida de evidencias**

| **Semana** | **Evidencias a entregar** | **Instrumento** | **RA** |
|-----------|---------------------------|-----------------|--------|
| 2 | Análisis de vulnerabilidades + Configuración base | Portfolio + Demo | RA1 |
| 5 | **Evaluación Parcial 1**: Seguridad perimetral completa | Rúbrica + Prueba práctica | RA1,RA2,RA4 |
| 7 | Proxy inverso + Alta disponibilidad | Demo + Documentación | RA5,RA6 |
| 9 | Comparativa técnica VPN + Configuraciones | Documentación técnica | RA3 |
| 10 | **Evaluación Parcial 2**: Acceso remoto funcional | Rúbrica + Demo conectividad | RA3 |
| 12 | **Entrega Final**: Proyecto integrado + Presentación | Rúbrica integral + Exposición | Todos |
