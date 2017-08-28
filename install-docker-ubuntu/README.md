# Instalando Docker en Ubuntu 16.04

1. Actualice la base de datos de paquetes
    ```   
    $ sudo apt-get update
    ```
1. Se agrega la clave GPG para el repositorio oficial de Docker al sistema
    ```
    $ sudo apt-key adv --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 58118E89F3A912897C070ADBF76221572C52609D
    ```

1. Se agrega el repositorio oficial de Docker a las fuentes APT
    > $ sudo apt-add-repository 'deb https://apt.dockerproject.org/repo ubuntu-xenial main'

1. Actualizamos de nuevo la base de datos, ahora con los paquetes de Docker recien actualizados
    > $ sudo apt-get update

1. Con la siguiente linea verificamos que vamos a instalar desde el repositorio de Docker correcto:
    > $ apt-cache policy docker-engine

1. Instalamos Docker
    > $ sudo apt-get isntall -y docker-engine

1. Docker ya debe estar instalado, verificamos que el servicio se encuentra activo y en ejecucion
    > $ service --status-all

