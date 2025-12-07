# Procesos
### Mostrar procesos
```
ps
```

### Mostrar procesos de forma extendida
El comando `ps` con las opciones `au` permite visualizar los procesos activos en la terminal actual, proporcionando detalles como el usuario propietario y el PID.

```
ps au
```
![img1](/ud1/img/procesos1.png)

### Mostrar todos los procesos del sistema
Al añadir la opción x (ps aux), el listado incluye absolutamente todos los procesos ejecutándose en el sistema, no solo los asociados a la terminal actual.
```
ps aux
```
![img2](/ud1/img/procesos2.png)

### Filtrar procesos por usuario
Para visualizar únicamente los procesos pertenecientes a un usuario específico, se utiliza la opción -u.

```
ps -u 'alumno'
```

![img3](/ud1/img/procesos3.png)

### Monitorización en tiempo real

El comando top muestra una tabla dinámica de los procesos, actualizándose en tiempo real para reflejar el consumo de CPU y memoria.

```
top
```

![img4](/ud1/img/procesos4.png)

### Gestión interactiva

htop es una alternativa mejorada al comando top. Equivale al "Administrador de tareas" en entornos gráficos, ofreciendo una interfaz navegable que permite interactuar con los procesos (como cerrarlos) sin necesidad de escribir comandos adicionales como kill
```
htop
```

![img5](/ud1/img/procesos5.png)

### Registro y auditoría avanzada
La herramienta atop se centra en el registro histórico. Toma instantáneas de los procesos y recursos en ejecución cada cierto tiempo (por defecto, cada 10 minutos), lo que permite analizar problemas ocurridos en el pasado.

```
atop
```


![img6](/ud1/img/procesos6.png)

### Prueba de estrés

Podemos simular una carga alta en la CPU para verificar cómo atop registra estos picos (stress test):

```
for i in {1..2}; do yes >/dev/null & done
atop
```

![img7](/ud1/img/procesos7.png)


[Volver al índice principal](../README.md)



