[🔙 << Clase 12](../12_Class/12_Class.md) | [Clase 14 >>](../14_Class/14_Class.md)

[🔙 Volver](../README.md)


# Comandos para administrar particiones y sistemas de archivos en Linux

## df
El comando `df` (Disk Free) se utiliza para mostrar información sobre el espacio en disco utilizado y disponible en el sistema de archivos. Sin argumentos, muestra una lista de todas las particiones montadas en el sistema junto con su uso de espacio y capacidad total. Algunos argumentos comunes incluyen:
- `-h`: muestra la información de uso de espacio en formato legible por humanos (GB, MB, KB, etc.).
- `-T`: muestra el tipo de sistema de archivos en lugar del tipo de dispositivo.
- `-i`: muestra información sobre el uso de inodos en lugar de bloques.
- `-t`: muestra solo las particiones que coinciden con el tipo de sistema de archivos especificado.

## lsblk
El comando `lsblk` se utiliza para listar información acerca de los dispositivos de almacenamiento del sistema, como discos duros, unidades flash USB, tarjetas SD y particiones. Sin argumentos, muestra una lista jerárquica de los dispositivos de almacenamiento conectados al sistema, incluyendo el tamaño, el nombre del dispositivo y el tipo de partición. Algunos argumentos comunes incluyen:
- `-a`: muestra todos los dispositivos, incluso aquellos que no están en uso o no tienen sistemas de archivos asociados.
- `-f`: muestra información adicional sobre los sistemas de archivos asociados con cada dispositivo.
- `-n`: suprime la cabecera y muestra solo la lista de dispositivos en una columna.
- `-o`: permite al usuario especificar qué columnas deben mostrarse en la salida.

## fdisk
El comando `fdisk` se utiliza para crear, editar y administrar particiones en el disco duro de un sistema. Con `fdisk`, se pueden ver las particiones existentes, crear nuevas particiones, modificar sus tamaños, tipos y formatos de sistema de archivos. También permite realizar otras tareas, como imprimir la tabla de particiones, verificar la integridad de las particiones o escribir una tabla de particiones en un archivo.

## Partición swap
La partición swap en Linux es un área de almacenamiento temporal en el disco duro que se utiliza cuando se agota la memoria RAM del sistema. Permite al sistema operativo manejar eficientemente los recursos de memoria y actúa como una extensión de la memoria RAM. Es importante asignar un tamaño apropiado a la partición swap para evitar un uso excesivo que pueda perjudicar el rendimiento del sistema.

Recuerda utilizar estos comandos con precaución, ya que pueden afectar los datos en tu sistema de almacenamiento.


# Comando mas usados

## lsblk
El comando `lsblk` se utiliza para listar los dispositivos de bloques y las particiones en el sistema.

## fdisk
El comando `fdisk` se utiliza para crear, editar y administrar particiones en el disco duro de un sistema.

## parted
El comando `parted` es otra herramienta para crear y administrar particiones de disco.

## mkfs
El comando `mkfs` se utiliza para formatear una partición con un sistema de archivos específico.

## mount
El comando `mount` se utiliza para montar un sistema de archivos en una partición o directorio.

## umount
El comando `umount` se utiliza para desmontar un sistema de archivos.

## df
El comando `df` muestra el espacio libre y utilizado en las particiones montadas.

## du
El comando `du` se utiliza para mostrar el tamaño de un archivo o directorio.

## resize2fs
El comando `resize2fs` se utiliza para ajustar el tamaño de un sistema de archivos ext2, ext3 o ext4.

## Comandos relacionados con LVM (Logical Volume Management)
- `lvcreate`: Crea un volumen lógico en un grupo de volúmenes LVM.
- `lvextend`: Amplía el tamaño de un volumen lógico.
- `lvresize`: Ajusta el tamaño de un volumen lógico.
- `lvremove`: Elimina un volumen lógico.
- `vgcreate`: Crea un grupo de volúmenes LVM.
- `vgextend`: Amplía un grupo de volúmenes LVM.
- `vgreduce`: Reduce un grupo de volúmenes LVM.
- `pvcreate`: Crea un volumen físico LVM en una partición o dispositivo.
- `pvextend`: Amplía un volumen físico LVM.
- `pvresize`: Ajusta el tamaño de un volumen físico LVM.
- `pvremove`: Elimina un volumen físico LVM.

Estos comandos son útiles para administrar particiones, sistemas de archivos y volúmenes lógicos en Linux.

Recuerda utilizar estos comandos con precaución, ya que pueden afectar los datos en tu sistema de almacenamiento.



[🔙 << Clase 12](../12_Class/12_Class.md) | [Clase 14 >>](../14_Class/14_Class.md)
