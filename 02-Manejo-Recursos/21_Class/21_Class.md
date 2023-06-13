[🔙 << Clase 20](../20_Class/20_Class.md) | [Clase 22 >>](../22_Class/22_Class.md)

[🔙 Volver](../README.md)


# Manejos de repositorios a profundidad
Existen repositorios con paquetes de uso privativo o no libre, que podemos activar en nuestro SO. Para ello se deberá tener en cuenta qué distribución tenemos o, más específicamente, qué manejador de paquetes. Siendo APT mucho más amigable, dado que podemos, por medio de un comando, conocer los repositorios existentes y activarlos con tan solo borrar el # inicial.

## En el caso de los RPM, los rpm fusión suplen esta necesidad de instalar paquetes por fuera de la licencia o filosofía de software libre del SO.

## Manejadores APT
- Para consultar los paquetes APT que tienes disponibles, ejecuta el siguiente comando:

    ```bash
    cat /etc/apt/sources.list
    ```

- o, si deseas solo conocer los que actualmente tienes activos, puedes:

    ```bash
    grep ^[^#] /etc/apt/sources.list →La expresión regular ^[^#] usada 
    en conjunto con grep hace que se filtren todos los resultados que inicien con #.
    ```

Ahora, si deseamos añadir repositorio que tampoco tenemos desactivado con el #. Debemos buscar en internet lo siguiente:

ubuntu server multiverse repository

Y la siguiente página es la más recomendada por sus guías sobre el mundo linux y su alta credibilidad:

[https://itsfoss.com/ubuntu-repositories/](https://itsfoss.com/ubuntu-repositories/)

Ahora, para manejadores APT, podemos encontrar dos tipos de repositorios externos:

Los universe: No incluyen software privativo. (solo software de código libre)
Los multiverse: Estos incluyen software privativo.

- Si quisieras instalar alguno de los anteriores paquetes, deberías utilizar el siguiente comando:
    ```bash
    sudo add-apt-repository universe
    sudo add-apt-repository multiverse
    sudo apt update
    ```
## Manejadores RPM:
- Para listar los repositorios con el manejador de paquetes RPM usamos el comando
    ```bash
    dnf repolist
    dnf repolist all ->  te mostrará los repositorios que están desactivados.
    ```

Ahora, para añadir repositorios extras debes buscar en google:

RPM fusión y entramos al siguiente link.

[rpmfusion.org](http://rpmfusion.org) 

copiamos y pegamos los siguientes comandos

```bash
sudo dnf install --nogpgcheck https://dl.fedoraproject.org/pub/epel/epel-release-latest-$(rpm -E %rhel).noarch.rpm
sudo dnf install --nogpgcheck https://mirrors.rpmfusion.org/free/el/rpmfusion-free-release-$(rpm -E %rhel).noarch.rpm https://mirrors.rpmfusion.org/nonfree/el/rpmfusion-nonfree-release-$(rpm -E %rhel).noarch.rpm
```

Finalmente, actualizamos los repositorios y, de preferencia, reiniciamos la consola o el sistema operativo.


[🔙 << Clase 20](../20_Class/20_Class.md) | [Clase 22 >>](../22_Class/22_Class.md)
