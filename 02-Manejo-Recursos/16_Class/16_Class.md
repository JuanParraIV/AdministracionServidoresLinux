[🔙 << Clase 15](../15_Class/15_Class.md) | [Clase 17 >>](../17_Class/17_Class.md)

[🔙 Volver](../README.md)


# Tipos de Archivos en Linux

En Linux, existen diferentes tipos de archivos que se utilizan para diversos propósitos. A continuación, se enumeran algunos de estos tipos de archivos:

- **Archivos regulares**: Contienen datos en formato de texto o binario y se pueden crear y editar con editores de texto o programas de procesamiento de datos.

- **Directorios**: Son archivos que contienen información sobre los archivos y subdirectorios que contienen. Se utilizan para organizar y estructurar los archivos en el sistema de archivos.

- **Hard links**: Estos enlaces son copias de un archivo original y hacen referencia a un punto en la memoria donde se almacena el archivo. Si modificamos uno de los enlaces, los cambios se reflejarán en todos los enlaces, ya que apuntan al mismo archivo en el sistema.

- **Links simbólicos**: También conocidos como soft links, son archivos que apuntan al archivo original a través de una referencia por nombre. Si eliminamos el archivo original, el enlace simbólico quedará inservible. Además, también se pueden crear enlaces simbólicos a directorios.

- **Archivos de dispositivos**: Estos archivos permiten que los programas se comuniquen con los periféricos y el hardware del sistema. Hay dos tipos de archivos de dispositivos: de caracteres y de bloque. Estos archivos no son unidades de almacenamiento en sí mismos, pero definen la comunicación y el manejo de los dispositivos conectados al sistema. Por ejemplo, `/dev/null` es un archivo de caracteres que no almacena ningún dato y se borra después de ejecutar el proceso que lo utiliza.

- **Sockets de dominio local**: Son conexiones entre procesos que facilitan la comunicación, especialmente en lo que respecta a la red. Los sockets de dominio local solo se pueden acceder desde el propio equipo (localhost) y permiten la comunicación entre aplicaciones en diferentes equipos.

- **Named Pipes**: Son archivos que permiten la comunicación entre dos procesos en ejecución simultánea. También se conocen como "FIFO files" (first in/first out), y se asemejan a una pila de procesos donde los datos se envían de forma secuencial.
Cada tipo de archivo tiene su propia función y características en el sistema operativo Linux. Comprender estos tipos de archivos es fundamental para comprender el funcionamiento del sistema de archivos y cómo interactuar con él.

¡Explora y aprovecha los diferentes tipos de archivos en Linux para administrar y organizar tus datos de manera eficiente!



[🔙 << Clase 15](../15_Class/15_Class.md) | [Clase 17 >>](../17_Class/17_Class.md)
