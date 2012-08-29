Seminario
=========

Seminario 2012 - 2do cuatrimestre

algunos comandos basicos

COMO AGREGAR EL REPOSITORIO
1) En tu pc crea el directorio donde vas a seguir los datos (puede tener cualquier nombre, pero quiza es mejor para este caso crear el mismo nombre SEMINARIO)

2) ejecutar un "git init" (en windows se puede hacer desde el boton derecho)

3) traer los datos colgados en la web 
	3.a) crear la conexion (indicando un alias, que servira para bajar los a)
comando: git remote add alias direccion
para nuestro caso: (ejemplo funcional)
git remote add seminarioenlaweb https://github.com/GRUPOFDASYSTEMS/Seminario.git
	
	3.b) traer los datos desde internet hacia la pc local
comando: git pull alias master
para nuestro caso: (ejemplo funcional)
git pull seminarioenlaweb master
(quiza pida autentificacion)

ENVIAR DATOS
git push -u alias master

VER ESTADO 
git status

VER LOG
git log