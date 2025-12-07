
# Memoria y Espacio

## Comando FREE
Este comando proporciona información detallada sobre la memoria del sistema, incluyendo la memoria física (RAM) y la memoria de intercambio (Swap).

### Visualización básica y legible
Por defecto, `free` muestra los valores en kilobytes. Para una lectura más sencilla (mostrando unidades como MB o GB), se utiliza la opción `-h`.

```bash
free        # Muestra los atributos básicos en bruto
free -h     # Muestra memoria usada y libre en unidades legibles (Human Readable)
````

![memoria1](/ud2/img/memoria1.png)

### Espacio en disco legible

```
df -h
```
Comando utilizado para reportar el uso del espacio en disco de los sistemas de archivos.

### Información extendida

```
df -ht
```

![memoria2](/ud2/img/memoria2.png)

### Resumen de ocupación

```
du
```
Herramienta para estimar y visualizar el espacio utilizado por archivos y directorios.
Ejecuta un análisis para mostrar el resumen total del tamaño ocupado por el directorio actual y sus subdirectorios.



![memoria3](/ud2/img/memoria3.png)

[Volver al índice principal](../README.md)
