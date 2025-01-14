# Proyecto sobre Odoo 01

Este proyecto va a tratar la instalación de la versión 17 community edition de Odoo a través de Docker, a su vez, también lo conectaremos a PgAdmin para poder utilizar una base de datos conjunta que mejorará las propias funciones de Odoo.

Para llevar este proyecto a cabo, vamos a tratar los siguientes temas:

    - Instalación de Odoo 17 Community Edition
    - Creación de la base de datos
    - Conexión con la base de datos
    
# 1. Instalación de Odoo 17 Community Edition

Para instalar Odoo utilizaremos Docker, una aplicación de codigo abierto que permite la automatización del despliegue de aplicaciones dentro de contenedores

> [!TIP]
> Para comprender como instalar Docker visita este repositorio: https://github.com/Nvieitez/Proyecto_Docker_01

Una vez instalado Docker y su respectivo Docker Compose, debemos encontrar la imagen de la versión del Odoo que deseemos instalar, para ello podemos visitar su respectiva página web dentro de Dockerhub, donde encontraremos su documentación y todos los parametros

> [!TIP]
> La página de documentación de Odoo dentro de dockerhub es: https://hub.docker.com/_/odoo

Una vez encontremos la documentacion necesaria, dentro buscamos los comandos de instalación de la versión deseada:

![Imagen de la documentación]()

Ahora dentro de la página web, encontramos un docker compose que nos puede servir como plantilla para iniciar nuestro servicio con los valores que nosotros necesitemos

![Imagen del docker compose]()

Una vez copiado el docker compose, vamos a crear de manera local desde la consola de comandos nuestro nuevo archivo docker-compose.yml, luego introduciremos dentro el contenido del docker compose que encontramos en el DockerHub

![Imagen del nuevo Docker Compose]()

Finalmente para instalar e iniciar el servicio iniciamos la imagen con el comando **"sudo docker-compose up -d"**

![Imagen del lanzamiento del Docker Compose]()

# 2. Creación de la base de datos

Una vez instalado y iniciado el servicio, vamos a entrar en odoo desde localhost, lo cual nos permite iniciar sesión con todos los datos que pusimos en el propio docker compose

![Imagen de inicio de sesión en el Odoo]()

Para confirmar que se cree correctamente la base de datos, una vez estemos dentro selecionamos un módulo, en mi caso seleccioné ventas

![Imagen de los módulos]()


