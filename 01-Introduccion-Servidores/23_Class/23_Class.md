[🔙 << Clase 22](../22_Class/22_Class.md) | [Clase 24 >>](../24_Class/24_Class.md)

[🔙 Volver](../README.md)


# Escaneo de Procesos en Linux

En Linux, puedes utilizar varias herramientas para escanear procesos y monitorear la actividad del sistema. Este README te proporcionará algunos ejemplos utilizando los comandos `ps` y `top`.

## Comando ps

El comando `ps` (procesos) te permite obtener información sobre los procesos en ejecución. Puedes utilizar diversas opciones para filtrar la salida y obtener detalles específicos. Por ejemplo, puedes ejecutar el siguiente comando para obtener una lista detallada de todos los procesos del sistema:
- **ps**
    ```bash
    ps aux
    ```

Si deseas buscar un proceso específico, puedes combinar ps con grep. Por ejemplo, el siguiente comando mostrará los procesos que coinciden con el nombre especificado:
- **ps con grep**
    ```bash
    ps aux | grep nombre_del_proceso
    ```

Reemplaza nombre_del_proceso con el nombre real del proceso que deseas escanear.


## Comando top
El comando top muestra una lista en tiempo real de los procesos en ejecución y actualiza la información periódicamente. Proporciona detalles como el uso de CPU, memoria, PID (identificador de proceso), entre otros. Puedes ejecutar el siguiente comando para iniciar top:
- **top:**
    ```bash
    top
    ```
Dentro de la interfaz de top, puedes utilizar diferentes teclas de función para interactuar con los procesos, ordenarlos y enviar señales a procesos individuales.

## Otras herramientas
Además de ps y top, existen otras herramientas útiles para el escaneo y monitoreo de procesos en Linux:

htop: Es una herramienta interactiva similar a top que proporciona una interfaz más amigable y gráfica para navegar y gestionar los procesos.

pstree: Muestra una representación jerárquica de los procesos en ejecución, lo que facilita la comprensión de la estructura del sistema.

lsof: Muestra los archivos abiertos por los procesos en el sistema, incluyendo sockets de red y otros recursos abiertos.

Recuerda consultar las páginas de manual de cada comando (man ps, man top, man htop, etc.) para obtener más detalles y aprender cómo utilizar eficientemente estas herramientas.

Explora estas herramientas y encuentra la que mejor se adapte a tus necesidades para escanear y monitorear procesos en tu sistema Linux.

[🔙 << Clase 22](../22_Class/22_Class.md) | [Clase 24 >>](../24_Class/24_Class.md)