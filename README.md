
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



