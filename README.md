# De la oficina al hogar inteligente: asegurando el acceso remoto, la domótica y la continuidad del negocio en una PYME

## 📋 Descripción del proyecto

Este repositorio contiene un **proyecto educativo por competencias** diseñado para el módulo **"Seguridad y alta disponibilidad"** del Ciclo Formativo de Grado Superior en **Administración de Sistemas Informáticos en Red**.

El proyecto simula un escenario empresarial real donde una PYME necesita implementar una infraestructura tecnológica segura que permita:
- Acceso remoto seguro para empleados en teletrabajo
- Automatización inteligente de oficinas y espacios de trabajo
- Continuidad del negocio ante interrupciones
- Cumplimiento de normativas de ciberseguridad

## 🎯 Objetivos de aprendizaje

### Resultados de Aprendizaje (RA) desarrollados:

| RA | Descripción | Contenidos |
|----|-----------|-----------| 
| **RA1** | Adoptar pautas de tratamiento seguro de la información | DietPi, configuración SSH segura |
| **RA2** | Implementar mecanismos de seguridad activa | Fail2ban, políticas de acceso |
| **RA3** | Configurar técnicas seguras de acceso remoto | OpenVPN, WireGuard |
| **RA4** | Implementar cortafuegos para asegurar sistemas | iptables, Pi-hole |
| **RA5** | Configurar servidores proxy seguros | Nginx Proxy Manager |
| **RA6** | Implementar soluciones de alta disponibilidad | Docker, Cloudflare DDNS |
| **RA7** | Reconocer la legislación y normativa sobre seguridad y protección de datos | RGPD, LOPDGDD, ISO 27001 |

## Estructura del repositorio

📦 Proyecto/\
├── 📄 README.md\
├── 📁 profesorado/\
│ ├── 📄 evaluacion.md\
│ ├── 📄 RAs-evaluar.xlsx\
│ ├── 📄 guia_didactica.pdf\
│ ├── 📄 metodologia.md\
│ ├── 📄 planificacion_temporal.md\
│ └── 📄 recursos.md\
── 📁 alumnado/\
│ ├── 📄 dosier.pdf\
│ ├── 📁 ejemplos/\
│ │ └── 📄 dietpi-imager\
│ ├── 📁 plantillas_trabajo/\
│ │ ├── 📄 plan_contingencias.md\
│ │ ├── 📄 plantilla_analisis_riesgos.md\
│ │ ├── 📄 plantilla_documentacion_tecnica.md\
│ │ └── 📄 plantilla_informe_legal.md\
│ ├── 📄 recursos.md\
└ └──  📄 videotutoriales.md\

## 🎓 Contexto educativo

- **Módulo:** Seguridad y alta disponibilidad
- **Ciclo:** Técnico Superior en Administración de Sistemas Informáticos en Red
- **Normativa:** Real Decreto 1629/2009, de 30 de octubre
- **Duración:** 12 semanas (60 horas)
- **Metodología:** Aprendizaje Basado en Proyectos (ABP)

## 🛠️ Tecnologías y herramientas

### Hardware requerido:
- **SBC (Single Board Computer):** Raspberry Pi 4 o similar
- **Tarjeta microSD:** 32GB mínimo, Clase 10
- **Conectividad:** Ethernet + WiFi

### Software principal:
- **Sistema base:** DietPi (distribución Linux optimizada)
- **VPN:** OpenVPN / WireGuard
- **Seguridad:** Fail2ban, iptables, Pi-hole
- **Proxy:** Nginx Proxy Manager
- **Contenedores:** Docker, Docker Compose
- **Domótica:** Home Assistant
- **DDNS:** Cloudflare

## 🚀 Fases del proyecto

### Fase 1: Análisis y planificación (Semanas 1-2)
- Análisis de vulnerabilidades empresariales
- Instalación segura de DietPi
- Configuración inicial de seguridad

### Fase 2: Seguridad perimetral (Semanas 3-5)
- Implementación de sistemas de detección de intrusiones
- Configuración avanzada de cortafuegos
- Filtrado DNS con Pi-hole

### Fase 3: Alta disponibilidad (Semanas 6-7)
- Proxy inverso para balanceo de carga
- Contenedores Docker para servicios críticos
- Sistema DDNS para IP dinámica

### Fase 4: Acceso remoto seguro (Semanas 8-10)
- Configuración de servidores VPN
- Métodos de autenticación robustos
- Pruebas de conectividad y rendimiento

### Fase 5: Domótica empresarial (Semana 11)
- Integración de Home Assistant
- Protocolos offline (Zigbee/Tasmota)

### Fase 6: Legislación y cumplimiento normativo (Semana 12)
- Auditoría legal y cumplimiento RGPD, LOPDGDD e ISO 27001
- Informe y presentación final


## 📊 Evaluación

El proyecto utiliza **evaluación continua por competencias** con:
- Rúbricas específicas por resultado de aprendizaje
- Portfolio digital de evidencias
- Autoevaluación y coevaluación
- Presentación final ante un "comité empresarial"

## 📖 Guía de uso

### Para profesorado:
1. Revisar la programación didáctica en `/profesorado/`
2. Adaptar la temporalización según el contexto
3. Utilizar las rúbricas para evaluación objetiva
4. Consultar el solucionario para resolución de dudas

### Para alumnado:
1. Comenzar por el dossier del proyecto en `/alumnado/`
2. Seguir las guías de actividades paso a paso
3. Utilizar las plantillas para documentación
4. Consultar recursos adicionales según necesidades

## 🎯 Competencias desarrolladas

### Competencias técnicas:
- Administración segura de sistemas Linux
- Configuración de redes privadas virtuales
- Implementación de sistemas de seguridad
- Gestión de servicios en contenedores
- Integración de sistemas domóticos
- Análisis de cumplimiento normativo

### Competencias transversales:
- Trabajo en equipo y liderazgo de proyectos
- Documentación técnica profesional
- Resolución de problemas complejos
- Comunicación técnica efectiva
- Pensamiento crítico en ciberseguridad

## 🔄 Adaptabilidad

El proyecto está diseñado para ser **flexible y escalable**:
- Adaptable a diferentes hardware (RPi, mini-PC, VPS)
- Modulable según tiempo disponible
- Escalable en complejidad técnica
- Reutilizable para formación continua

## 📚 Referencias curriculares

Basado en el **Real Decreto 1629/2009**, específicamente:
- Resultados de aprendizaje del módulo Seguridad y Alta Disponibilidad (0378)
- Competencias profesionales del perfil ASIR
- Conexiones con módulos complementarios
- Preparación para certificaciones profesionales

## 🤝 Contribuciones

Este material educativo está diseñado para ser:
- **Colaborativo:** Acepta mejoras y adaptaciones
- **Actualizable:** Incorpora nuevas tecnologías
- **Compartible:** Reutilizable en diferentes centros educativos

## 📄 Licencia

Este proyecto educativo se distribuye bajo licencia **Creative Commons Attribution-ShareAlike 4.0 International** (CC BY-SA 4.0), permitiendo:
- ✅ Compartir y adaptar el material
- ✅ Uso comercial en contextos educativos
- ⚠️ Atribución obligatoria
- ⚠️ Misma licencia para obras derivadas

---

## 📞 Contacto y soporte

**Módulo:** Seguridad y alta disponibilidad  
**Centro:** IES Abastos  
**Curso académico:** 2024-2025  

**Recursos adicionales:**
- 📋 [Issues](../../issues) para dudas y mejoras
- 📖 [Wiki](../../wiki) para documentación extendida
- 🔄 [Discussions](../../discussions) para intercambio entre docentes
