
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
d)	Seleccionar el tipo de instalación personalizada, realizar las siguientes acciones, luego dar click en siguiente y finalizar   


