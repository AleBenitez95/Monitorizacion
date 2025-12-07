
# Monitorización del Tráfico de Red

## TCPDUMP: Análisis de paquetes
Es la herramienta de línea de comandos estándar para la captura de tráfico. Permite interceptar y mostrar los paquetes que están siendo transmitidos o recibidos por la red del sistema.

```
tcdump
```
![tarjeta](/ud3/img/tarjeta1.png)
### TCPTRACK: Monitorización de conexiones

Esta herramienta rastrea y muestra el estado de las conexiones TCP en tiempo real. Funciona de manera similar al comando top, pero enfocada en la red, proporcionando detalles como el origen, destino y estado de la conexión.

```
tcptrack -i <tarjeta_de_red>
```
![tarjeta2](/ud3/img/tarjeta2.png)
### IPTRAF: Estadísticas detalladas

Herramienta basada en menús de texto (ncurses) que genera estadísticas en tiempo real del tráfico IP. Permite desglosar la información por protocolos (TCP, UDP), puertos e interfaces específicas.


```
iptraf
```
![tarjeta3](/ud3/img/tarjeta3.png)
### BMON: Monitor de ancho de banda

bmon (Bandwidth Monitor) es una herramienta diseñada para la depuración y monitorización del ancho de banda. Su principal característica es la visualización del flujo de tráfico mediante gráficos ASCII directamente en la terminal.

```
bmon

```

![tarjeta4](/ud3/img/tarjeta4.png)
