
██████╗░░█████╗░░█████╗░██╗░░░██╗██╗░░░░░░█████╗░  
██╔══██╗██╔══██╗██╔══██╗██║░░░██║██║░░░░░██╔══██╗  
██████╦╝███████║██║░░╚═╝██║░░░██║██║░░░░░███████║  
██╔══██╗██╔══██║██║░░██╗██║░░░██║██║░░░░░██╔══██║  
██████╦╝██║░░██║╚█████╔╝╚██████╔╝███████╗██║░░██║  
╚═════╝░╚═╝░░╚═╝░╚════╝░░╚═════╝░╚══════╝╚═╝░░╚═╝  

██████╗░░█████╗░░█████╗░██╗░░░██╗██╗░░░░░██╗░░░██╗███╗░░░███╗
██╔══██╗██╔══██╗██╔══██╗██║░░░██║██║░░░░░██║░░░██║████╗░████║
██████╦╝███████║██║░░╚═╝██║░░░██║██║░░░░░██║░░░██║██╔████╔██║
██╔══██╗██╔══██║██║░░██╗██║░░░██║██║░░░░░██║░░░██║██║╚██╔╝██║
██████╦╝██║░░██║╚█████╔╝╚██████╔╝███████╗╚██████╔╝██║░╚═╝░██║
╚═════╝░╚═╝░░╚═╝░╚════╝░░╚═════╝░╚══════╝░╚═════╝░╚═╝░░░░░╚═╝


----------------------------------------------------------------------
|                CONFIGURACIÓN DE API BACULUM                        |
----------------------------------------------------------------------

Ingresamos por web 192.168.X.X por el puerto 9095 (ip:port), con las credenciales por defecto de Baculum, realizar el respectivo test para la verificación de las configuraciones.
        
        Usuario: admin 
        Contraseña: admin

a)	Seleccionaremos el lenguaje

b)	Compartiremos la base de datos de Bacula con Baculum, seleccionaremos “Yes” 
  
    Base de datos: MySQL
    IP address (hostname): localhost
    (En password dejaremos en blanco para que entre a la base de datos sin problemas y no para que no pida  autenticación en la base de datos MySQL)

c)	Configurar la interfaz para el compartimiento de interfaz de bconsole en la API
    ![api3](https://user-images.githubusercontent.com/103973381/228109440-b5f7ce07-b318-499a-b5df-78f708087198.png)

d)	Configurar los componentes para el compartimiento de Bacula en la API, añadir la ruta del directorio web.
        /etc/bacula/web
        ![api4](https://user-images.githubusercontent.com/103973381/228301704-e8e65fd0-89eb-4951-9349-dbbfd1551137.png)

e)	Añadir usuario y contraseña (configuración personalizada)
        ![api5](https://user-images.githubusercontent.com/103973381/228329343-41a5ca2e-fc26-42b3-a96d-2fa22b74e191.png)

f)	Observar las configuraciones realizadas y guardar
        ![api6](https://user-images.githubusercontent.com/103973381/228331216-3bf9079b-c6ee-4893-ade3-5aefb08ef3ff.png)


----------------------------------------------------------------------
|                    CONFIGURACIÓN DE WEB BACULUM                    |
----------------------------------------------------------------------

Ingresamos por web 192.168.X.X por el puerto 9095 (ip:port), con las credenciales por defecto de Baculum, realizar el respectivo test para la verificación de las configuraciones.

        Usuario: admin 
        Contraseña: admin
        
a)	Selección de idioma: English

b)	Introducir las credenciales que guardamos en la API
![web2](https://user-images.githubusercontent.com/103973381/229323884-0c2e52bc-0be2-4ca5-ad8e-abda2a5192d1.png)

c)	Crearemos las credenciales para el ingreso a Baculum Web
![web3](https://user-images.githubusercontent.com/103973381/229323925-133886ca-714e-455f-9064-617a86dcc8e3.png)

d)	Observar las configuraciones realizadas y guardar.
    (El resultado es el mismo que presenta en la configuración de la API Baculum)

e)	Una vez finalizado la instalación se debe ingresar con la ip y puerto e ingresar con las credenciales creada en el proceso de configuración.
        (Bacula, Configuración gráfica de Baculum, 2022)

----------------------------------------------------------------------
|         Instalación de clientes Bacula Windows / Linux             |
----------------------------------------------------------------------

## Clientes Windows
Descargar el archivo .exe en el siguiente enlace dependiendo de cuantos bits es su sistema operativo Windows y seguir las siguientes configuraciones.          ( https://www.bacula.org/download/11049/ ).

a)	Ejecutar el programa .exe y aceptar la licencia de acuerdo.     
b)	Dejar el archivo de instalación por defecto y dar click siguiente.      
c)	Seleccionar solo el cuadro de “Client” y dar click en siguiente.        
d)	Seleccionar el tipo de instalación personalizada, realizar las siguientes acciones, luego dar click en siguiente y finalizar.

![WIN1](https://user-images.githubusercontent.com/103973381/229324850-c18e6ef6-ede5-469a-9e98-3060cfa01449.png)

## Configuración de regla entrada/salida para clientes Windows  
a)	Ingresar a “Windows Defender Firewall con seguridad avanzada”, las configuraciones deben ser para ambas reglas de entrada/salida y realizar las                         siguientes acciones
![WIN2](https://user-images.githubusercontent.com/103973381/229324936-cf76809d-fb53-4ca1-a3f7-8094dcd0b544.png)

b)	Seleccionar la opción de Puerto y agregar los puertos de Bacula 9101,9102,9103 y dar click en siguiente.
![WIN3](https://user-images.githubusercontent.com/103973381/229325003-b60fe625-4a2d-4dc9-a6a8-b0e8aa0e19dd.png)
![WIN4](https://user-images.githubusercontent.com/103973381/229325064-744ef3d8-95c9-41bd-a6cd-de2264dde609.png)

c)	En el siguiente paso dar click en “Permitir conexión” y dar click en siguiente para el paso de “Perfil” y dar click en todos los cuadros.
![WIN5](https://user-images.githubusercontent.com/103973381/229325136-cf4e699c-8387-4549-86d0-04dc1c0ce989.png)
![WIN6](https://user-images.githubusercontent.com/103973381/229325230-7e8b5cfc-d461-49c1-8bd4-10c4f1d56fa0.png)

d)	En el último paso escribir el nombre del servidor.
![WIN7](https://user-images.githubusercontent.com/103973381/229325242-7563d088-7ebe-4d7e-b071-d194bf074f0c.png)


## Clientes Linux

### Comandos para instalación
-	sudo apt install bacula-client --- Ubuntu
-	sudo apt-get install bacula-fd --- Linux Mint, Debian

### Configuración de cliente Linux
a)	Ingresar a /etc/bacula y editar el archivo bacula-fd.conf
![linux1](https://user-images.githubusercontent.com/103973381/229325435-09f9a5fe-ccdb-4062-879c-866068d4d715.png)

b)	Reiniciar Bacula cliente con el siguiente comando: systemctl restart bacula-fd
(Bacula, Instalación de clientes bacula Windows y Linux, 2022)

----------------------------------------------------------------------
|        Registro de clientes Windows y Linux en Baculum             |
----------------------------------------------------------------------
Para la agregación de los clientes y para su respectivo monitoreo de backup deben pertenecer a la misma red y hacer la siguiente configuración.

a)	Ingresar al portal de Baculum (IP: PORT) con las credenciales ya creadas anteriormente.

b)	Añadir el cliente LINUX/WINDOWS, con las siguientes indicaciones
-	Nombre 
-	Descripción 
-	IP
-	Contraseña
-	Catalogo

c)	Crear en FILESET (conjunto de archivo) una capeta específica para el cliente
-	Nombre
-	Descripción

d)	Crear en FILESET (conjunto de archivo) una capeta específica para el cliente
-	Nombre
-	Descripción

e)	Crear en JOBS los trabajos que realizara el cliente
-	Nombre
-	Descripción
-	Tipo de Backup: respaldo, restaurar, copia, verificación, migrar, administrar
-	Nivel: full, incremental, diferencial
-	Cliente: seleccionar el cliente para que realice el JOB asignado
-	Fileset: seleccionar el fileset creado para el cliente
-	Pool: seleccionar la entidad lógica (file, default, scratch)
-	Almacenamiento: seleccionar file 1
-	Mensajes: seleccionar estándar
-	Schedule: es opcional seleccionar en ciclo semanal o mensual
-	JobDefs: es opcional su selección
-	Priority: 10

Finalmente dar click en Create, y redirigirse nuevamente al JOB creado del cliente, seleccionar en CONFIGURE FILESET para establecer las rutas de los archivos del cliente el cual definirá que archivos estarán incluido para el respaldo.
-	Include: introducir la ruta de la carpeta para el respaldo puede ser uno o más rutas a elección Ej.: C:/Users/paula/Downloads/bacula
-	Ejecutar el JOB
Para el respaldo se debe ir al historial de JOBS, en detalles del JOB seleccionado es donde se debe seleccionar para restaurar y elegir al cliente donde se desea hacer el respaldo.
(Haba, Documentación de Baculum, 2021)


----------------------------------------------------------------------
|                           INTERFAZ                                 |
----------------------------------------------------------------------
![INTERFAZ](https://user-images.githubusercontent.com/103973381/229325867-f2295e17-b192-43f0-a772-d7c24f6dd0ec.png)

----------------------------------------------------------------------
|                           CLIENTES                                |
----------------------------------------------------------------------
![CLIENTES](https://user-images.githubusercontent.com/103973381/229325998-283a2e3a-0695-450e-873f-7cdbd85ec648.png)
