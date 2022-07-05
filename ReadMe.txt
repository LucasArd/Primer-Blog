- La página principal es:
http://127.0.0.1:8000/
o tambien http://127.0.0.1:8000/AppAero


- En el header están las cuatro opciones que llevan a las distintas clases (pasajeros,
azafatas, pilotos y personal administrativo), la función de busqueda y la de registrarse.
Una vez registrado, la opción de registrarse cambia a una vista de tú perfil.

- Haciendo click en las primeras cuatro opciones mencionadas lleva al usuario a un
formulario donde puede insertar datos de un nuevo objeto que pertenezca al modelo
seleccionado, pero solo si está registrado como usuario. De lo contrario, solo podrá añadir
datos de pasajeros.

- Haciendo click en el botón "Busqueda", y si el usuario está registrado, el usuario puede
ingresar el apellido de la persona que busca. El sistema muestra todos los pasajeros,
pilotos y/o azafatas con ese apellido. Desde esta misma página también se pueden ver listas
con todos los pasajeros, pilotos o azafatas registrados. A partir de estas listas se pueden
modificar o borrar la información de los mismos.

- En http://127.0.0.1:8000/AppAero/about hay informacion sobre nosotros, los creadores de
la página.

- Si se ingresa en la barra de busqueda una URL no reconocida, lleva a una página 404 que
permite volver al inicio.

#----------------------------------------------------------------------------------------------------------------------

- Creamos CRUD por Vista de:
pasajeros, azafatas, pilotos y personal administrativo

- Modificando Settings.py a:
DEBUG = False
ALLOWED_HOSTS = ["*"]

- Agregamos ruta de STATIC para que pueda obtener los archivos de STATIC ya que si no hacemos esto la pagina carga sin static files

- Creamos vista, url y template ABOUT/ en donde hablamos de nosotros los desarrolladores. Ademas agregamos boton de redireccionamiento

- Cambiamos el Model BOLETO por PERSONAL ADMINISTRATIVO, para darle mas sentido a la pagina. Esto conlleva la modificacion de las views, urls, base de datos, formularios, etc.

- Se crea  INICIO con direccionammiento directo desde localhost, aunque tambien se deja INICIO desde AppAero/INICIO. 

- Se crea y perfecciona creado del Perfil y edicion del mismo.
