# Administración de la nube con Azure CLI y Azure Service Health
## Azure CLI
Buscamos y descargamos el [Azure CLI](https://docs.microsoft.com/en-us/cli/azure/install-azure-cli-windows?tabs=azure-cli), dependiendo de nuestro sistema operativo.

![Práctica 14 - parte 1](imagenes\p14p1.png)

Abrimos un cmd y escribimos _az login_. Se nos abrirá una página para iniciar seción con nuestra cuenta de Azure.

![Práctica 14 - parte 2](imagenes\p14p2.png)

Para crear un recurso escribimos el siguiente comando:
_az group create --location westus --resourse-group sesion7_

![Práctica 14 - parte 3](imagenes\p14p3.png)

Nuestro grupo de recursos tardará un poco pero se creará y podremos verlo desde el portal de [Azure](https://portal.azure.com/).

![Práctica 14 - parte 4](imagenes\p14p4.png)

## Azure Service Health
En la barra de búsqueda de Azure buscamos "Service Health".

![Práctica 14 - parte 5](imagenes\p14p5.png)

Nos aparecerá un mapa que, dependiendo de los parámetros seleccionados, podemos ver diferentes servicios y si hay problemas en alguna región.

![Práctica 14 - parte 6](imagenes\p14p6.png)

Podemos crear alertas que nos notifiquen del fallo de algún servicio en alguna región, para ello seleccionamos "Crear alerta de Service Health"

![Práctica 14 - parte 7](imagenes\p14p7.png)

Configuramos las alertas con los parámetros:
- Suscripción
- Servicios
- Regiones
Seleccionamos los grupos de acciones, si no tenemos o queremos agregar otro lo creamos.

![Práctica 14 - parte 8](imagenes\p14p8.png)

Para crear un grupo de acciones configuramos los Datos básicos:
- Suscripción
- Grupo de recursos: sesion7
- Nombre de las acciones: notificacionesazure

![Práctica 14 - parte 9](imagenes\p14p9.png)

En notificaciones elegimos el tipo de notificación (correro electrónico en este caso) y el Nombre.

![Práctica 14 - parte 10](imagenes\p14p10.png)

Para editar esta notificación podemos elegir un correo electrónico, SMS, notificación en Azure Mobile App o voz.

![Práctica 14 - parte 11](imagenes\p14p11.png)

Al revisar y crear esta acción podemos usar un Grupo de acciones de prueba (versión preliminar).

![Práctica 14 - parte 12](imagenes\p14p12.png)

Esta prueba nos permite selecciona que tipo de alerta queremos.

![Práctica 14 - parte 13](imagenes\p14p13.png)

Dependiendo de la forma de notificación recibiremos una notificación prueba de la alerta.

![Práctica 14 - parte 14](imagenes\p14p14.png)

Una vez configurados los grupos de acciones configuramos los detalles de la regla de alertas:
- Nombre de la regla de alertas: notificacion servicios de azure
- Grupo de recursos: sesion7

![Práctica 14 - parte 15](imagenes\p14p15.png)

En Azure Service Health podemos ver eventos como:
- Problemas de servicio
- Mantenimiento planeado
- Avisos de estado
- Avisos de seguridad

![Práctica 14 - parte 16](imagenes\p14p16.png)
También podemos ver el Historial de  estado, Estado de loos recursos y Alertas de estado.

![Práctica 14 - parte 17](imagenes\p14p17.png)

En las Alertas de estado podemos ver las alertas que hemos creados, así como añadir más o eliminarlas.

![Práctica 14 - parte 18](imagenes\p14p18.png)