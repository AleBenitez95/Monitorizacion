
# Auditoría de Puertos y Reconocimiento de Red

En este documento se presentan los comandos necesarios para monitorizar el estado de los puertos, identificar servicios activos y obtener información sobre hosts en la red.

---

## SS (Socket Statistics)
Herramienta moderna utilizada para volcar estadísticas de sockets. Es el sustituto recomendado del obsoleto `netstat`.

### Puertos a la escucha
El comando `ss -plunt` es fundamental para identificar qué servicios están esperando conexiones.
* **-p**: Muestra el proceso asociado.
* **-l**: Solo sockets en escucha (listening).
* **-u / -t**: UDP y TCP respectivamente.
* **-n**: No resuelve nombres de servicio (muestra números de puerto).

```bash
ss -plunt

```


![puertos1](/ud4/img/puertos1.png)

![puertos2](/ud4/img/puertos2.png)

### NMAP (Network Mapper)
Es la herramienta estándar para el descubrimiento de redes y auditoría de seguridad.
```bash
nmap -sn <ip>
```

### Verificación de host (Ping Scan)
Realiza un escaneo sin verificar puertos, simplemente para confirmar si el host objetivo está activo (online).
```
nmap <dirección_de_red>
```

![puertos3](/ud4/img/puertos3.png)


### ARP (Address Resolution Protocol)
Permite visualizar y manipular la caché ARP del sistema, que asocia direcciones IP con direcciones físicas (MAC).

### Visualizar tabla ARP
Muestra la tabla actual de vecinos conocidos por el sistema. Es útil para identificar hardware local en la red.

```
arp -a
```

![puertos4](/ud4/img/puertos4.png)

### WHOIS
Herramienta de consulta para obtener información sobre dominios o direcciones IP públicas.

### Consulta de registros
Consulta las bases de datos de los registros regionales de Internet (RIR) para revelar datos administrativos del objetivo, como el propietario, proveedor de servicios (ISP) y rangos de IP asignados.

```bash
whois <ip_o_dominio>
```



![puertos5](/ud4/img/puertos5.png)

[Volver al índice principal](../README.md)
