Seminario
=========

Seminario 2012 - 2do cuatrimestre

algunos comandos basicos

COMO AGREGAR EL REPOSITORIO
1) En tu pc crea el directorio donde vas a seguir los datos (puede tener cualquier nombre, pero quiza es mejor para este caso crear el mismo nombre SEMINARIO)

2) ejecutar un "git init" (en windows se puede hacer desde el boton derecho)
*nota: conviene que la carpeta este vacia

3) traer los datos colgados en la web 

	3.a) crear la conexion (indicando un alias, que servira para trabajarlo)
comando: git remote add alias direccion_http
para nuestro caso: (ejemplo funcional)
git remote add seminarioenlaweb https://github.com/GRUPOFDASYSTEMS/Seminario.git
	
	3.b) traer los datos desde internet hacia la pc local
hay 2 formas clonando o trayendolo paso a paso (todo esto se puede hacer con las herramientas que pueden bajar de internet, pero les muestro los comandos si les parece mejor, usen el que quieran)
forma manual
comando: git pull alias master
para nuestro caso: (ejemplo funcional)
git pull seminarioenlaweb master
(quiza pida autentificacion)
 
4) A TRABAJAR
Bueno ahora tienen 2 repositorios:
1- el local: desde donde van a trabajar
2- el web: donde van a sincronizar datos

para trabajar
	a) cuando realizan cambios a los archivos deben informar esto asi:
      git add . (punto)
               b) confirmar los cambios para establecer un punto de confirmacion/reposicion
     git commit 

5) SINCRONIZANDO...

ENVIAR DATOS (cuando envian datos al servidor si ninguno hizo cambios acepta el envio sin problemas)
git push -u alias master

* Si tira algun error quiere decir que hubo un cambio deben bajar el archivo y acoplarle sus datos y luego reintentar subirlo

SINCRONIZACION DOBLE
git fetch alias master

CONVERGENCIA DE DATOS (INTENTA ARMAR EL ARCHIVO AUTOMATICAMENTE)
git merge alias master

VER ESTADO 
git status

VER LOG
git log