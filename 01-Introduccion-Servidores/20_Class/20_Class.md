[🔙 << Clase 19](../19_Class/19_Class.md) | [Clase 21 >>](../21_Class/21_Class.md)

[🔙 Volver](../README.md)


# Instalación de paquetes en Linux

En Linux, es común instalar software desde la línea de comandos utilizando el manejador de paquetes de la distribución que estés utilizando. El proceso para instalar un paquete es bastante sencillo y se realiza en unos pocos pasos.

## Paso 1: Actualizar la lista de paquetes disponibles

Antes de instalar un paquete, es recomendable actualizar la lista de paquetes disponibles en los repositorios. Utiliza el siguiente comando según la distribución que estés utilizando:

- **Distribuciones basadas en Debian (Ubuntu, Linux Mint):**
    ```bash
    sudo apt update
    ```

- **Distribuciones basadas en Red Hat (Fedora, CentOS):**
    ```bash
    sudo dnf update
    ```

## Paso 2: Buscar el paquete

Utiliza el comando de búsqueda correspondiente para encontrar el paquete que deseas instalar. Ejecuta el siguiente comando según la distribución:

- **Distribuciones basadas en Debian (Ubuntu, Linux Mint):**
    ```bash
    apt search <nombre_del_paquete>
    ```

- **Distribuciones basadas en Red Hat (Fedora, CentOS):**
    ```bash
    dnf search <nombre_del_paquete>
    ```

## Paso 3: Instalar el paquete

Una vez que encuentres el paquete que deseas instalar, utiliza el comando correspondiente para llevar a cabo la instalación. Utiliza el siguiente comando según la distribución:

- **Distribuciones basadas en Debian (Ubuntu, Linux Mint):**
    ```bash
    sudo apt install <nombre_del_paquete>
    ```
    

- **Distribuciones basadas en Red Hat (Fedora, CentOS):**
    ```bash
    sudo dnf install <nombre_del_paquete>
    ```

## Espera a que se complete la instalación del paquete. En algunos casos, se te pedirá que confirmes la instalación o que ingreses tu contraseña de administrador.

## ¡Y eso es todo! Ahora deberías tener el paquete instalado en tu sistema Linux y listo para ser utilizado. Recuerda que, dependiendo del paquete que estés instalando, es posible que necesites reiniciar ciertos servicios o aplicaciones para que los cambios tengan efecto.


[🔙 << Clase 19](../19_Class/19_Class.md) | [Clase 21 >>](../21_Class/21_Class.md)
