[<< Volver al Inicio](../../README.md) | [Siguiente: Clase 2 >>](../02_Class/02_Class.md)


# ¿Cómo es el arranque del sistema?

- **El SO es almacenado en memoria:** En este proceso se busca encontrar un espacio dentro de la memoria para poder ejecutarse sin problemas.
↓

- **Revisión de hardware:** A través de este proceso se busca monitorizar todos los dispositivos conectados a través del Firmware.
↓

- **Selección del dispositivo de arranque:** En ella se muestra un grub donde seleccionaremos que sistema operativo a utilizar.
↓

- **Detección de la partición EFI:** Luego de seleccionar la partición se verificará el espacio de almacenamiento del sistema elegido.
↓

- **Carga del bootloader:** Este proceso arrancara el sistema elegido anteriormente.
↓

- **Determina el kernel a usar:** A través de este paso el sistema elige el kernel mediante el cual el sistema funcionara este proceso lo hace el sistema tomando en cuenta lo que ya se tiene instalado.
↓ 

- **Carga del kernel:** Paso donde se ira iniciando el sistema para mostrar al usuario.
↓

- **Se carga el primer proceso (PID1):** Este proceso es que se comenzara a iniciar el proceso de INIT en Linux.
↓

- **Ejecuta scripts de inicio:** Para este proceso se cargarán todos los scripts que se irán ejecutando en segundo plano conocidos como daemons o demonios.
↓

- **Inicia el sistema:** El sistema se habrá iniciado correctamente para poder ser usado por el usuario administrador o usuario normal.

## Conceptos Claves

Firmware del sistema

Hace un inventario y chequeo de todos
los dispositivos conectados al sistema al
momento del arranque (discos, memorias,
etc.).
Este a su vez crea interfaces para que
el software del sistema operativo pueda
usar estos dispositivos.


Boot Loader

Separa el firmware del sistema y el

arranque del sistema operativo. Es un paso
previo a que se ejecute el sistema
operativo.

Es util para correr el SO en forma de rescate
0 con parametros extra.



GRUB: the GRand
Unified Boot loader

Es el boot loader por defecto en la mayoria
de distribuciones Linux.

Actualmente contamos con dos versiones:
e GRUB Legacy
e GRUB 2


BIOS VS UEFI


## Requisitos previos

Antes de tomar este curso, es recomendable tener algunos conocimientos previos en los siguientes aspectos:

- Conceptos básicos de ingeniería de software: Familiaridad con los principios y fundamentos de la ingeniería de software te ayudará a comprender mejor los conceptos y técnicas relacionadas con Linux.
- Manejo básico de la terminal: Es importante tener conocimientos básicos sobre cómo navegar y ejecutar comandos en la terminal, ya que gran parte de la administración de Linux se realiza a través de la línea de comandos.
- Opcional: Saber Shell o Python: Tener conocimientos básicos de scripting en Shell o Python puede ser beneficioso para automatizar tareas y escribir scripts en Linux.
- Opcional: Conocimiento de redes computacionales: Si tienes conocimientos básicos sobre redes computacionales, te resultará más fácil comprender los conceptos relacionados con la configuración y administración de redes en Linux.

## Uso y popularidad de Linux

Contrario a la creencia popular, Linux no es poco usado. De hecho, aproximadamente el 80% de los servidores en todo el mundo utilizan Linux como sistema operativo. Además, Linux también se encuentra presente en supercomputadoras y la mayoría de los servidores en la nube. Su popularidad se debe a su estabilidad, seguridad y capacidad de personalización.

## Contenido del curso

Al finalizar este curso, adquirirás los siguientes conocimientos:

- Conocerás los diferentes tipos de servidores y su aplicación en el entorno empresarial.
- Tendrás un entendimiento claro de los conceptos clave de un sistema Linux, como la estructura de directorios, permisos de archivos y la gestión de procesos.
- Serás capaz de administrar de manera básica un servidor Linux, lo que incluye la instalación y configuración del sistema operativo, la gestión de usuarios y permisos, y la administración de paquetes.
- Obtendrás un conocimiento profundo sobre cómo funciona el sistema por dentro, lo que te permitirá comprender mejor su funcionamiento interno y solucionar problemas comunes.



[<< Volver al Inicio](../../README.md) | [Siguiente: Clase 2 >>](../02_Class_Habilidades/02_Habilidades.md)

