# Ansible
Conjunto de ejercicios usando ansible

Ejercicio 1

Debes crear un playbook que realice las siguientes tareas de forma automática:

    Crear un usuario en el servidor remoto que tenga tu nombre.
    Descarga el fichero desde la url https://wordpress.org/latest.zip.
    Descomprime ese fichero en el home del usuario creado anteriormente.
    Instala el paquete mariadb.
    Crea una base de datos que se llame tunombre_wordpress.
    Crea un usuario que se llame my_nombre que tenga privilegios sobre la base de datos.
    Clona el repositorio: https://github.com/josedom24/ansible_ejemplos.giten el home del usuario que hemos creado en el primer punto.


Ejercicio 3: Configuración del escenario router-nat

Queremos configurar el escenario para que cumpla lo siguiente:

    La máquina router debe acceder a internet por eth1. eth0 sólo se utiliza para acceder a la máquina con vagrant ssh.
    La máquina cliente debe tener acceso a internet. Para ello debe salir por eth1 y la máquina router debe estar configurada para enrutar las peticiones de cliente. del mismo modo, eth0 sólo se utiliza para acceder con vagrant ssh. Debes pensar que configuración debe tener la máquina cliente: puerta de enlace, configuración dns,…

Crea un playbook en ansible con los siguientes roles:

    common: Estas tareas se deben ejecutar en los dos nodos. La única tarea es actualizar los paquetes.
    router: Todas las tareas necesarias para configurar router cómo router-nat y que salga a internet por eth1. Las configuraciones deben ser permanente.
    cliente: Todas las tareas necesarias para que el cliente salga a internet pot eth1.

Crea un playbook que configure todo lo anterior
