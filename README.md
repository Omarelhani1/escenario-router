# escenario-router

**Entrega: Ejercicio 2**

**En este ejercicio sólo vamos a construir el escenario.**

*El fichero Vagrantfile que construya el escenario.*
*Una captura de pantalla donde se vea un ping de la máquina cliente a la máquina router.*

**Ejercicio 3: Configuración del escenario router-nat**

Queremos configurar el escenario para que cumpla lo siguiente:

*La máquina router debe acceder a internet por eth1. eth0 sólo se utiliza para acceder a la máquina con vagrant ssh.*
*La máquina cliente debe tener acceso a internet. Para ello debe salir por eth1 y la máquina router debe estar configurada para enrutar las peticiones de cliente. del mismo modo, eth0 sólo se utiliza para acceder con vagrant ssh. Debes pensar que configuración debe tener la máquina cliente: puerta de enlace, configuración dns,…*

Crea un playbook en ansible con los siguientes roles:

*common: Estas tareas se deben ejecutar en los dos nodos. La única tarea es actualizar los paquetes.*
*router: Todas las tareas necesarias para configurar router cómo router-nat y que salga a internet por eth1. Las configuraciones deben ser permanente.*
*cliente: Todas las tareas necesarias para que el cliente salga a internet pot eth1.*


