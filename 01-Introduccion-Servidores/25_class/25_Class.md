[🔙 << Clase 24](../24_Class/24_Class.md) | [Clase 26 >>](../26_Class/26_Class.md)

[🔙 Volver](../README.md)


# Creación y manejo de demonios
Es un proceso de Linux que da un comportamiento de servicio a un programa: es decir, que se ejecuta en segundo plano sin la interacción de un usuario.

- **systemd : crea los demonios**
- **systemctl: gestiona los demonios**

## Para crear un demonio primero debes:

- Crear el script o unit file que usará de base tu demonio, esto puedes hacerlo con Python u otro lenguaje de scripting.

- Es importante crear el folder donde se alojará el unit file a nivel de root, de esta manera estará disponible para todos los usuarios.

- Crear la carpeta en donde alojaremos la información generada por nuestro unit file.

- ir a /etc/systemd/system y crear el script que beberá del primero para poder correr el demonio.

- reiniciamos los demonios con:
    ```bash
    systemctl daemons-reload
    ```

- Habilitamos con:
    ```bash
    systemctl enable loggerpython.service
    ```

- Activamos con:
    ```bash
    systemctl start loggerpython.service
    ```


[🔙 << Clase 24](../24_Class/24_Class.md) | [Clase 26 >>](../26_Class/26_Class.md)
