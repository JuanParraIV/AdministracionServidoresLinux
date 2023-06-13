[🔙 << Clase 18](../18_Class/18_Class.md) | [Clase 20 >>](../20_Class/20_Class.md)

[🔙 Volver](../README.md)


# Uso de Manejadores de Paquetes en Linux

Los manejadores de paquetes son herramientas esenciales en Linux para instalar, actualizar y eliminar software en el sistema. A continuación, se muestra cómo utilizar los manejadores de paquetes APT y DNF en diferentes distribuciones:

## APT (Ubuntu y Linux Mint)

- **Actualizar la lista de paquetes disponibles en los repositorios:**
    ```bash
    sudo apt update
    ```

- **Instalar un paquete:**
    ```bash
    sudo apt install <nombre_del_paquete>
    ```

- **Actualizar todos los paquetes instalados en el sistema:**
    ```bash
    sudo apt upgrade
    ```

- **Eliminar un paquete:**
    ```bash
    sudo apt remove <nombre_del_paquete>
    ```

- **Buscar un paquete en los repositorios:**
    ```bash
    apt search <nombre_del_paquete>
    ```
    

## DNF (Fedora y CentOS 8+)
- **Actualizar la lista de paquetes disponibles en los repositorios:**
    ```bash
    sudo dnf update
    ```

- **Instalar un paquete:**
    ```bash
    sudo dnf install <nombre_del_paquete>
    ```
    
- **Actualizar todos los paquetes instalados en el sistema:**
    ```bash
    sudo dnf upgrade
    ```

- **Eliminar un paquete:**
    ```bash
    sudo dnf remove <nombre_del_paquete>
    ```

- **Buscar un paquete en los repositorios:**
    ```bash
    sudo dnf search <nombre_del_paquete>
    ```

## Estos son solo algunos comandos básicos para comenzar a utilizar los manejadores de paquetes. Cada distribución puede tener sus propias particularidades y opciones adicionales. Explora la documentación oficial para obtener más información sobre el uso de los manejadores de paquetes en tu distribución específica.

[🔙 << Clase 18](../18_Class/18_Class.md) | [Clase 20 >>](../20_Class/20_Class.md)
