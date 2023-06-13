[🔙 << Clase 10](../10_Class/10_Class.md) | [Clase 12 >>](../12_Class/12_Class.md)

[🔙 Volver](../README.md)


# Configuración básica para un servidor remoto

## SSH (Secure Shell Protocol)

El protocolo Secure Shell (SSH) nos permite acceder de manera remota a un servidor de forma segura.

### Comandos SSH

1. **Verificar la instalación de OpenSSH:**
    ```bash
    ssh
    ```

    **En caso de no tenerlo instalado, puedes instalarlo con el comando:**
    ```bash
    sudo apt install openssh
    ```

2. **Verificar el estado del servicio SSH:**
   ```bash
   systemctl status sshd
   ```


3. **Obtener la dirección IP interna del servidor:**
    ```bash
    ip address
    ```



### Conexión al servidor

Para conectarte al servidor desde un dispositivo en la misma red.

- **utiliza el siguiente comando desde la PowerShell de Windows o la consola del sistema operativo que estés usando:**

    ```bash
    ssh username@localip
    ```


- **Reemplaza "username" por tu nombre de usuario y "localip" por la dirección IP interna del servidor.**


### Acceso remoto al servidor

Si deseas acceder al servidor de forma remota, utiliza la dirección IP pública en lugar de la dirección IP interna. Puedes obtener la dirección IP pública desde un navegador de Internet buscando "myip" estando conectado a la misma red del servidor. 

- **También puedes utilizar el siguiente comando en el servidor para obtenerla:**

    ```bash
    curl ifconfig.me
    ```


Recuerda que es importante tener el puerto 22 abierto en el firewall y considerar prácticas de seguridad adicionales, como permitir solo ciertas direcciones IP para evitar accesos no autorizados.

¡Ahora estás listo para acceder y configurar tu servidor de forma remota!



[🔙 << Clase 10](../10_Class/10_Class.md) | [Clase 12 >>](../12_Class/12_Class.md)