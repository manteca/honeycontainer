# Ideas Consideradas
## Generales
Low Interaion Honeypot ( por el tiempo que se dispone ), pero se intentara de colocar herram
ientas que permitan mas informacio, por lo tanto sería un intermadiate Interacion Honeypot

## MAC
Se debe considera que la MAC debe tener los digitos iniclaes de la marca de IoT

## Docker
Con docker se levantara el servicio para contener al atacante en un ambinte semi-controlado.
El volumne donde se guarden los registros, debe ser accedido solo por un usuario espesifico y no el usuario con el que se conecat al sistema

# Malware
Enviar los archivos descar¡gados a Virtitotal

# Protocolos
## Seleccionados
Serv    Prot/Port   Otros
http
https   TCP/443
ssh     TCP/22
telnet TCP/23       TCP/2323

# Posibles...
Mqtt    TCP/1883 8883
xmpp    TCP/5222
UPnp    UDP/1900
smb     TCP/445


# Acciones en IoT
Debe estar recibiendo ( generando datos periodicos)

# TipoLinux a correr
Al parecer el tipo de Linux que deberian correr en los contenedores es un
--BusyBox--

## "Imagenes"
Low Int Web Browser
https://github.com/buffer/thug
https://hub.docker.com/r/honeynet/thug/
Web browser

DockerFiles HoneyPot( podria ser la base)
https://github.com/sreinhardt/Docker-Honeynet
(Revisar todos los honeypots que se crearon en docker)

---
### Advance
https://github.com/MattCarothers/mhn-core-docker

HoneyPot Famosos
Kippo, Glastopf, Dionaea, Thug, Cowrie
