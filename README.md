# web_LcBox
Proyecto de tienda online con registro, login y gestión de productos

Tecnologías usadas:

	PHP:
En este proyecto he utilizado php para la comunicación entre la aplicación y la base de datos, toda la parte de gestión de datos, operaciones de consulta, inserción, actualización, borrado, para la validación del login y la inserción de cookies cuando se añade algún producto al carrito.
Además para poder hacer la gestión de las sesiones, todas los archivos html los he tenido que pasar a la extension .php, con el fin de mantener las opciones personaizadas del menú para el usuario “admin” en toda la página web.

	MySQL: 
He montado una base de datos de tipo InnoDB utilizando un servidor MariaDB y el gestor de base de datos phpMyAdmin.
Las consultas a dicha base de datos las he realizado en php utilizando SQL.
	Javascript:
Con esta tecnología he desarrollado todo el comportamiento de la aplicación del lado del cliente, tanto la animación del logo, inserciones de código según las acciones del usuario así como las ventanas modales de añadir al carrito han sido programadas desde esta tecnología.
	Bootstrap:
La maquetación de este proyecto web ha sido realizada con Boostrap 4, consiguiendo que sea completamente responsive, dependiendo del tamaño de la pantalla se vera de una forma u de otra, aparecerán y desapareceran contenidos etc..
	Animaciones CSS:
He utilizado este tipo de animación en el borde de ciertos elementos para hacer que se vaya cambiando su color conforme pasa el tiempo, así como el rotulo de bienvenida al iniciar sesión.
	Ajax:
La mayor parte de esta tecnología la he usado para hacer la gestión de productos desde el usuario de admin.
Para enviar y recibir datos de la tabla a la base de datos pasando por php en el proceso.
Gracias a este sistema basado en promesas no es necesario recargar la página cada vez que se actualiza la información de la tabla de gestión de productos.


Especificaciones técnicas

1.	Descomprimir el pryecto en la carpeta htdocs de xampp, para poder usar el servidor apache como host.
2.	Importar la base de datos a partir del script lcbox.sql desde la opción de importación en phpMyAdmin.
3.	Asegurarse de tener un usuario que se llame root sin contraseña para poder acceder a la base de datos.
4.	Ingresar a la dirección donde hemos guardado el pryecto a traves del navegador poniendo la siguiente ruta:
http://localhost: 80/xampp/ruta de la carpeta 
 
5.	La pagina principal del proyecto es el index.php, hay creados 3 usuarios:
	Usuario : admin    Contraseña:  admin
	Usuario: cliente1   Contraseña:   cliente
	Usuario: cliente2   Contraseña:   cliente
 
La aplicación esta diseñada para tener un solo usuario de administración, pero se puede añadir más usuarios de administración ya que estos tipos de usuarios se diferencias únicamente en el campo tipo de la tabla de cuentas en la base de datos.

Los administradores pueden añadir, editar o elminiar los productos de la web a través de la pestaña “Edición de productos”, la cual contiene una tabla muy intuitiva para ello.

En este proyecto no he implementado el carrito ni la pasarlea de pago, pero he dejado la opción por si en un futuro se quisiera aplicar estas funcionalidades.
