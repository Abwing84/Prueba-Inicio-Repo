# CLASE 01 MIÉRCOLES 12 DE AGOSTO DEL 2026 - Portafolio Inicio
# Comienzo del Readme... de Abel Astudillo

Hemos comenzado con el repositorio, les voy a dejar los comandos que utilice <br>


* Vimos como he creado el repositorio en la nube de Github
* Es importante saber que antes de todo esto se debe tener todos los pasos de ingreso y seguridad
* Cuando hablamos de seguridad y conetividad se trata de la ssh, es la clave publica y privada
* Abrimos la termianl de git bash como administrador
* Ingresamos al area de trabajo donde queremos agregar el repo
* El profe Ariel ingreso a la carpeta de Documents / en cambio yo tengo todo en mi usuario y luego TecnicaturaGit

```sh comilla backtick = Alt+96
    cd TecnicaturaGit
    mkdir Proyectos
    cd Proyectos
    git clone git@github.com:Abwing84/Prueba-Inicio-Repo.git
    cd Prueba-Inicio-Repo
    git pull origin main
    git fech
    git branch # Veran que esta la rama main por defecto
    touch README.md # Creamos el readme
    git status
    git add .
    git commit -m"Creacion del readme"
    git status
    git push origin main
    
```  

## Agregamos este trabajo al readme online

> ¿Como hacemos esto? 

Ingresamos al repositorio y solo apretamos punto <br>

```sh 
    .
```

Ingresamos todo esta informacion y terminamos.

# CLASE 02 MIÉRCOLES 19 DE AGOSTO DEL 2026 - Portafolio 1

Vamos a cargar la llave SSH publica en GitHub -> SI YA HAZ HECHO ESTE TRABAJO, NO SE DEBE REPETIR EL SSH

Para copiar la llave publica debes ir al archivo .ssh y allí encontrarás el archivo .pub lo podes abrir con el txt, luego copiar el contenido que esta dentro.

copiar la llave publica #Ir a GitHub, vamos a setting, vamos a SSH and GPG keys

crear una nueva #New SSH key poner nombre y pegar la ssh publica, con esto esta listo.

Aconsejo que la ssh tenga el nombre del ordenador en el que estas trabajando. Esto se debe hacer con cada pc nueva o dispositivo nuevo que tengamos para acceder a nuestra cuenta de GitHub.

```sh comilla backtick = Alt+96
git branch #Vemos en que rama estamos

git checkout master #Ponernos en la rama master

git branch -M main #Cambiamos el nombre a la rama master

git remote add origin git@github.com:nombreUsuario/class-git.git #Agregamos el repositorio remoto, este es un ejemplo

git remote -v #Vemos si ya esta conectado

git merge segunda #Mergeamos lo que tenemos en la rama segunda en main

git commit -am "Uso de GitHub parte 20" #Hacemos el commit de hoy

git push origin main #Pasamos todo lo hecho a GitHub, revisar en el repositorio en GitHub.

Frente al cambio de nombre de rama master a main, suele suceder que en el repo de GitHub se hayan creado dos ramas, la rama master y la rama main, se debe ir al repo, settings y ahí se puede cambiar la rama principal, en vez de que siga siendo master, que sea la rama main, luego de eso ya podemos borrar la rama master.
    
```  
# CLASE 03 MIÉRCOLES 26 DE AGOSTO DEL 2026 - Portafolio 2


## Cambios en GitHub: de master a main

* El escritor Argentino Julio Cortázar afirma que las palabras tienen color y peso. Por otro lado, los sinónimos existen por definición, pero no expresan lo mismo. Feo no es lo mismo que desagradable, ni aromático es lo mismo que oloroso.


Por lo anterior, podemos afirmar que los sinónimos no expresan lo mismo, no tienen el mismo “color” ni el mismo “peso”.

Sí, esta lectura es parte de la enseñanza profesional de Git & GitHub.

Desde el 1 de octubre de 2020 GitHub cambió el nombre de la rama principal: ya no es “master” -como aprenderás aquí- sino main.

Este derivado de una profunda reflexión ocasionada por el movimiento #BlackLivesMatter.

La industria de la tecnología lleva muchos años usando términos como master, slave, blacklist o whitelist y esperamos pronto puedan ir desapareciendo.

Y sí, las palabras importan.

Por lo que de aquí en adelante cada vez que me escuches mencionar “master” debes saber que hago referencia a “main”. *

¿Cuando es que sigue siendo master y cuando sigue siendo main?
Cuando se crea un repositorio desde git bash en nuestro ordenador a través de git init, sigue siendo el estandar como master. ¿Qué hacer con esto? Debes cambiar el nombre de la rama master a main con el comando:

```sh comilla backtick = Alt+96
 git branch -M main

O cambiando la asignación por default con este otro comando:

git config --global init.defaultBranch main

A partir de este comando siempre que ingreses git init será la rama main.

Ahora cuando creamos un repositorio desde la nube, osea desde GitHub, ya verás que la rama principal tiene por default el nombre de main y al clonar a nuestro ordenador seguira teniendo este nombre y no será necesario ningun cambio.

Otro comando que deben saber es:

gitk

Si no te funciona el comando gitk es posible no lo tengas instalado por defecto.

Para instalar gitk debemos ejecutar los siguientes comandos:

sudo apt-get update

sudo apt-get install gitk

Recuerda que podemos ver gráficamente nuestro entorno y flujo de trabajo local con Git utilizando el comando gitk. Gitk fue el primer visor gráfico que se desarrolló para ver de manera gráfica el historial de un repositorio de Git.

```
