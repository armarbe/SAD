# 🛠️ Materiales y Recursos

## **Listado de materiales**

### **Hardware requerido**

#### **Por puesto de trabajo (recomendado 2 estudiantes por equipo)**
| Componente | Especificaciones mínimas | Especificaciones recomendadas | Cantidad |
|------------|-------------------------|-------------------------------|----------|
| **SBC (Single Board Computer)** | Raspberry Pi 3B+ o superior | Raspberry Pi 4B (4GB RAM) | 1 por equipo |
| **Tarjeta microSD** | 32GB Clase 10 | 64GB Clase 10 U3 | 1 por equipo |
| **Alimentación** | 5V/2.5A USB-C | 5V/3A USB-C oficial | 1 por equipo |
| **Cable Ethernet** | Cat 5e mínimo | Cat 6 | 1 por equipo |
| **Carcasa** | Básica con ventilación | Con ventilador activo | 1 por equipo |
| **Lector tarjetas SD** | USB básico | USB 3.0 integrado | 1 por aula |
| **Coordinador Zigbee** | CH9102X | CP2102N | 1 por equipo |

#### **Infraestructura del aula**
| Recurso | Especificaciones | Observaciones |
|---------|-----------------|---------------|
| **Switch de red** | 24 puertos Gigabit mínimo | Para conectividad de todas las SBC |
| **Router/Firewall** | Configurable, VLAN support | Para crear redes de prueba aisladas |
| **Proyector/Pantalla** | Full HD mínimo | Para demostraciones grupales |
| **Ordenadores estudiantes** | SSH client, navegador web | Para acceso remoto a las SBC |
| **Dispositivos de domótica** | Compatibles con Zigbee/Tasmota | Para integrar en HomeAssistant |

### **Software base**

#### **Sistema operativo y herramientas**
| Software | Versión | Licencia | Propósito |
|----------|---------|----------|-----------|
| **DietPi** | Última estable | GPL | Sistema base optimizado |
| **Docker** | CE (Community Edition) | Apache 2.0 | Contenedores |
| **Docker Compose** | v2.17+ | Apache 2.0 | Orquestación de contenedores |
| **SSH Client** | OpenSSH o PuTTY | Libre/MIT | Acceso remoto |
| **Balena Etcher** | Última versión | Libre | Grabación de imágenes |

#### **Aplicaciones específicas del proyecto**
| Aplicación | Repositorio/Fuente | Función en el proyecto |
|------------|-------------------|----------------------|
| **Fail2ban** | Repositorios oficiales Debian | Detección de intrusiones |
| **iptables** | Incluido en DietPi | Cortafuegos |
| **Pi-hole** | https://pi-hole.net | Filtrado DNS |
| **OpenVPN** | https://github.com/d3vilh/openvpn-server | VPN con interfaz gráfica (guía incluida en el repositorio) |
| **WireGuard** | https://github.com/wg-easy/wg-easy | VPN moderna (guía incluida en el repositorio) |
| **Nginx Proxy Manager** | https://github.com/NginxProxyManager/nginx-proxy-manager | Proxy inverso (guía incluida en el repositorio) |
| **Cloudflare DDNS** | https://github.com/timothymiller/cloudflare-ddns | DNS dinámico (guía incluida en el repositorio) |
| **Home Assistant** | https://www.home-assistant.io | Plataforma domótica (guía oficial en la web) |

---

## **Guías de uso para el profesorado**

### **1. Preparación inicial del entorno**

- **Descarga e instalación de DietPi**: [DietPi Download](https://dietpi.com/#download) - incluye guías para hardware compatible y no compatible
- **Securización SSH**: [Guía IONOS para deshabilitar root login](https://www.ionos.com/help/server-cloud-infrastructure/getting-started/important-security-information-for-your-server/deactivating-the-ssh-root-login/)

### **2. Instalación de componentes principales**

- **Docker**: [Guía oficial instalación en Debian](https://docs.docker.com/engine/install/debian/)
- **Docker Compose**: [Guía oficial instalación](https://docs.docker.com/compose/install/linux/#install-using-the-repository)
- **VPN OpenVPN**: [Repositorio con guía completa](https://github.com/d3vilh/openvpn-server)
- **VPN WireGuard**: [Repositorio con guía completa](https://github.com/wg-easy/wg-easy)
- **Nginx Proxy Manager**: [Repositorio con documentación](https://github.com/NginxProxyManager/nginx-proxy-manager)
- **Cloudflare DDNS**: [Repositorio con instrucciones](https://github.com/timothymiller/cloudflare-ddns)
- **Home Assistant**: [Guía oficial instalación Linux](https://www.home-assistant.io/installation/linux)

### **3. Alternativas**
- **DuckDNS** (alternativa gratuita a Cloudflare): https://www.duckdns.org/

---

## **Repositorios y recursos adicionales**


### **Enlaces a recursos externos**

#### **Documentación base**
- **DietPi**: https://dietpi.com/#download
- **DietPi Hardware Guide**: https://dietpi.com/docs/hardware/#make-your-own-distribution
- **SSH Security**: https://www.ionos.com/help/server-cloud-infrastructure/getting-started/important-security-information-for-your-server/deactivating-the-ssh-root-login/

#### **Docker y contenedores**
- **Docker**: https://docs.docker.com/engine/install/debian/
- **Docker Compose**: https://docs.docker.com/compose/install/linux/#install-using-the-repository

#### **Servicios del proyecto**
- **OpenVPN Server**: https://github.com/d3vilh/openvpn-server
- **WireGuard Easy**: https://github.com/wg-easy/wg-easy
- **Nginx Proxy Manager**: https://github.com/NginxProxyManager/nginx-proxy-manager
- **Cloudflare DDNS**: https://github.com/timothymiller/cloudflare-ddns
- **DuckDNS**: https://www.duckdns.org/
- **Home Assistant**: https://www.home-assistant.io/installation/linux

---

## **Herramientas de verificación (pendiente - en construcción)**

### **Scripts de verificación automática**
- Scripts para verificar estado de servicios
- Herramientas de monitorización de logs
- Comandos de diagnóstico esenciales
- Procedimientos de backup y restauración

*Disponibles en el repositorio del profesorado*

### **Material complementario**

#### **Recursos didácticos**
- Presentaciones de conceptos teóricos
- Diagramas de arquitectura del sistema
- Videos tutoriales de configuraciones críticas
- Guías de troubleshooting visual

#### **Documentación técnica**
- Flowcharts de configuración paso a paso
- Diagramas de red y seguridad
- Templates de documentación para estudiantes
- Ejemplos de configuraciones funcionando

---

## **Consideraciones especiales para el profesorado**

### **Preparación del entorno**
- **Red aislada**: Configurar VLAN dedicada para las prácticas
- **Imágenes de respaldo**: Mantener backups de configuraciones base
- **Acceso remoto**: VPN del centro para soporte desde casa
- **Mirror local**: Repositorios críticos disponibles offline

### **Gestión de incidencias**
- **Hardware**: Procedimientos para tarjetas SD corruptas
- **Red**: Scripts de diagnóstico automatizado
- **Software**: Checklist de verificación de contenedores
- **Recuperación**: Procedimientos de restauración rápida

### **Escalabilidad**
- **Grupos grandes**: Estrategias para más de 20 estudiantes
- **Hardware limitado**: Adaptaciones para recursos reducidos
- **Tiempo reducido**: Versiones simplificadas del proyecto
- **Nivel diferente**: Adaptaciones para otros niveles formativos
