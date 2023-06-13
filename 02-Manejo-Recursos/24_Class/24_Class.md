[🔙 << Clase 23](../23_Class/23_Class.md) | [Clase 25 >>](../25_class/25_Class.md)

[🔙 Volver](../README.md)


# Manejo de Procesos

El manejo de procesos es una parte fundamental en el entorno de Linux. El process id (PID) nos permite identificar y controlar los diferentes software que se están ejecutando en el sistema. En este README, aprenderemos cómo administrar los procesos y realizar acciones como finalizarlos, pausarlos y reiniciarlos.

## Estados de un Proceso

Un proceso puede encontrarse en diferentes estados, que indican su actividad y disponibilidad. Estos estados son:

- **Running or Runnable (R):** El proceso está en ejecución o listo para ser ejecutado.
- **Uninterruptible Sleep (D):** El proceso está esperando a que se complete una operación de E/S y no puede ser interrumpido.
- **Interruptible Sleep (S):** El proceso está esperando a que se complete una operación de E/S y puede ser interrumpido.
- **Stopped (T):** El proceso ha sido detenido, generalmente debido a una señal enviada por el usuario o el sistema.
- **Zombie (Z):** El proceso ha finalizado, pero su entrada aún se mantiene en la tabla de procesos hasta que el padre recopile la información de salida.

## Envío de Procesos a Segundo Plano

Si deseas enviar un archivo o proceso a segundo plano, simplemente agrega el símbolo `&` al final de cada comando o utiliza ` ctrl + Z ` para pausar el proceso.

## Visualización de Procesos en Segundo Plano

- Puedes utilizar el siguiente comando para ver los jobs o procesos abiertos en segundo plano:
    ```bash
    jobs -l
    ```

## Volver a Primer Plano un Proceso Secundario

- Si tienes un proceso secundario en segundo plano y deseas volver a primer plano, utiliza el comando `fg` seguido del PID del proceso:
    ```bash
    fg [PID]
    ```


## Finalización de Procesos

Para finalizar un proceso, necesitamos conocer su PID. Puedes obtener el PID utilizando herramientas como `htop`. 
- Una vez que tengas el PID, ejecuta el siguiente comando para finalizar el proceso:
    ```bash
    kill [PID]
    ```

- Si el proceso se encuentra en segundo plano, agrega la siguiente opción para forzar la finalización:
    ```bash
    kill -s SIGKILL [PID]
    ```


## Finalización de Todos los Procesos Asociados a un Programa

- Si deseas finalizar todos los procesos asociados a un programa, puedes utilizar el siguiente comando:
    ```bash
    killall [nombre_del_programa]
    ```

Recuerda reemplazar `[nombre_del_programa]` por el nombre real del programa que deseas finalizar.

## ¡Asegúrate de tener precaución al finalizar procesos, ya que esto puede afectar el funcionamiento del sistema! Utiliza estos comandos con responsabilidad y ten en cuenta el impacto que pueden tener en tu sistema.


[🔙 << Clase 23](../23_Class/23_Class.md) | [Clase 25 >>](../25_class/25_Class.md)

