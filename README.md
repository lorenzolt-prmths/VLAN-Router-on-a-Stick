##Inter-VLAN Routing (Router on a Stick)
📌 Descripción

En este proyecto se ha implementado una red segmentada mediante VLANs para separar diferentes departamentos de una empresa (Administración, Ventas e IT).
Para permitir la comunicación entre las distintas VLANs se ha configurado Inter-VLAN Routing utilizando Router on a Stick en Cisco Packet Tracer.

El router realiza el enrutamiento entre VLANs mediante subinterfaces y encapsulación IEEE 802.1Q, mientras que el switch gestiona la segmentación de la red mediante VLANs y enlaces trunk.

##🗺️ Topología de red

La red está compuesta por:

1 Router
1 Switch
3 VLANs
3 Equipos finales
Enlace trunk entre switch y router

🧩 Diseño de red

Se ha dividido la red en tres VLANs correspondientes a distintos departamentos:

VLAN	Departamento	Red
10	ADMIN	192.168.10.0/24
20	VENTAS	192.168.20.0/24
30	IT	192.168.30.0/24

Cada VLAN tiene su propia red y su puerta de enlace configurada en el router.

⚙️ Configuración

En el switch se han creado las VLANs y se han asignado los puertos de acceso a cada departamento.
El puerto conectado al router se ha configurado como trunk para permitir el tráfico de todas las VLANs.

En el router se han configurado subinterfaces en la interfaz física utilizando encapsulación 802.1Q.
Cada subinterfaz actúa como puerta de enlace de su VLAN correspondiente.

🧪 Verificación y pruebas

Para verificar el funcionamiento de la red se han realizado las siguientes comprobaciones:

Comprobación de VLANs en el switch
Comprobación del enlace trunk
Comprobación de subinterfaces en el router
Ping entre equipos de diferentes VLANs
Traceroute para verificar el paso por el router




Las pruebas confirman que existe conectividad entre las distintas VLANs y que el router enruta correctamente el tráfico entre ellas.

🛠️ Tecnologías utilizadas
Cisco Packet Tracer
VLAN
Trunking
Inter-VLAN Routing
Router on a Stick
Redes LAN
Routing
🎯 Objetivos del proyecto
Segmentar una red mediante VLANs
Configurar enlaces trunk
Implementar Inter-VLAN Routing
Configurar subinterfaces en router
Permitir comunicación entre VLANs
Verificar conectividad entre redes
📚 Conclusión

Mediante la implementación de Router on a Stick se ha conseguido que diferentes VLANs puedan comunicarse entre sí manteniendo la segmentación de red.
Este tipo de configuración es habitual en redes empresariales donde es necesario separar departamentos pero permitir comunicación controlada entre ellos.
