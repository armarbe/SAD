# 🛠️ Guía de integración de coordinador Zigbee en contenedor de Home Assistant  

  ## Pasos iniciales - creación de contenedor
Para crear un contenedor de Home Assistant con docker run podemos utilizar los siguientes comandos:
1. Creamos la carpeta donde se guarda la información:
```bash
mkdir /home/homeassistant
```
2. Docker run:
```bash
docker run -d --name homeassistant --privileged --restart=unless-stopped -e TZ=ES -p 8123:8123 -v /home/homeassistant:/config -v /run/dbus:/run/dbus:ro ghcr.io/home-assistant/home-assistant:stable
```
  ## Integración Zigbee
Si queremos integrar el coordinador Zigbee debemos introducir en el terminal:
```bash
ls -l /dev/serial/by-id
```
Por ejemplo, si el resultado obtenido es:
```bash
usb-1a86_USB_Single_Serial_550D016405-if00 -> ../../ttyACM0
```
Deberíamos añadir a nuestro docker run la siguiente opción:
```bash
--device=/dev/serial/by-id/usb-1a86_USB_Single_Serial_58E9038794-if00:/dev/ttyACM0
```
Si ya estaba en ejecución el contenedor, introducimos los siguientes comandos:
```bash
docker stop homeassistant
docker remove homeassistant
```
Y ya podemos volver a desplegar el contenedor conservando la configuración utilizando la opción mencionada:
```bash
docker run -d --name homeassistant --privileged --restart=unless-stopped -e TZ=ES -p 8123:8123 -v /home/homeassistant:/config -v /run/dbus:/run/dbus:ro  --device=/dev/serial/by-id/usb-1a86_USB_Single_Serial_58E9039644-if00:/dev/ttyACM0 ghcr.io/home-assistant/home-assistant:stable
```
  ## Backup
Para hacer un backup de Home Assistant podemos ejecutar el siguiente comando:
```bash
tar -zcvf ha_bk.tar.gz /home/homeassistant
```
Y para restaurarlo:
```bash
tar -xzvf ha_bk.tar.gz /
```
