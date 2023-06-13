[🔙 << Clase 13](../13_Class/13_Class.md) | [Clase 15 >>](../15_Class/15_Class.md)

[🔙 Volver](../README.md)


# Manejo de un archivo swap en Linux
La partición swap en Linux es una parte importante del sistema para manejar eficientemente los recursos de memoria cuando la RAM se agota. En este readme, aprenderás cómo crear y administrar un archivo swap en Linux.

## Pasos para crear un archivo swap

1. **Ve al directorio raíz del sistema:**

    ```bash
        cd /
    ```

2. **Verifica si tienes un archivo swap actualmente:**

    ```bash
    ls -lh
    ```

3. **Verifica la cantidad de memoria disponible:**

    ```bash
    free -h
    ```

4. **Verifica si tienes suficiente espacio en disco para aumentar la partición swap actual o crear una nueva:**

    ```bash
    df -h
    ```

5. **Crea un archivo especial para tu memoria swap (por ejemplo, 2 GB):**

    ```bash
    sudo fallocate -l 2G /swapfile
    ```

6. **Configura los permisos para que solo el root pueda acceder a este archivo en lectura y escritura:**

    ```bash
    sudo chmod 600 /swapfile
    ```

7. **Confirma que tienes tu archivo swap creado:**

    ```bash
    ls -lh
    ```

8. **Convierte el archivo swap creado en un archivo swap válido:**

    ```bash
    sudo mkswap /swapfile
    ```

9. **Configura el archivo /etc/fstab para que se monte automáticamente en el arranque del sistema:**

    ```bash
    sudo vim /etc/fstab
    ```

    **Escribe la siguiente línea en el archivo fstab:**

    ```bash
    /swapfile swap swap defaults 0 0
    ```

    **Para salir de vim, presiona la tecla ESCAPE, luego escribe :wq y presiona ENTER. El archivo se guardará y saldrás del editor.**


10. **Comprueba los cambios que hiciste al archivo fstab:**

    ```bash
    cat /etc/fstab
    ```

11. **Activa tu archivo swap como memoria swap:**

    ```bash
    sudo swapon /swapfile
    ```

## ¡Listo! Ahora tienes un archivo swap configurado en tu sistema. Recuerda que si deseas desactivarlo, puedes utilizar el comando sudo swapoff /swapfile y eliminar la línea correspondiente del archivo fstab.

## Espero que esta guía te sea útil para administrar correctamente tu archivo swap en Linux.

## Recuerda ajustar el tamaño del archivo swap según las necesidades de tu sistema para garantizar un rendimiento óptimo. ¡No dudes en consultar la documentación oficial de tu distribución de Linux para obtener más información y mejores prácticas sobre el uso de swap!



[🔙 << Clase 13](../13_Class/13_Class.md) | [Clase 15 >>](../15_Class/15_Class.md)