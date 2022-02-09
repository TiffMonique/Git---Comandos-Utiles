# Comandos Utiles de Git

<div align="center">
    <img src="https://media.giphy.com/media/kH1DBkPNyZPOk0BxrM/giphy.gif" width="300px"> </img> 
    
<!-- Encabezado -->
## Git | Control de versiones
### Autor 

| Nombre  |
|:-------------:|
|Tiffany Monique Matamoros Gonzalez | 
</div>

_____
_____

### ¿Qué es Git?
* Git es un sistema de control de versiones distribuido gratuito y de código abierto diseñado para manejar todo, desde proyectos pequeños hasta proyectos muy grandes, con rapidez y eficiencia.

### Funciones
* Controlar y administrar las distintas versiones de un programa
* Contribuir con varios desarrolladores en cualquier parte del mundo
* Revertir cualquier cambio hecho por cualquier desarrollador en una rama especifica
* Se pueden trabajar con repositorios locales o remotos
  
_____
### Estados 
| Estado | Descripción |
|:-------|:------------|
|Working Directory |Donde se trabaja con todos los archivos|
|Staging Area|Donde se agregan los archivos a guardar en git|
|Repository|Donde se guardan los archivos en formato git| 


### Comandos básicos en la terminal
| Comando | Función|
|:-------|:------------|
pwd | sirve para ver en que carpeta estamos
cd |Nos permite navegar entre carpetas.
cd /| Ir a la ruta principal
cd o cd ~|Ir a la ruta de tu usuario
cd carpeta/subcarpeta| Navegar a una ruta dentro de la carpeta donde estamos ahora mismo.
cd /c |para ir al disco c
cd .. |retroceder a una ruta anterior
ls| mostrar contenido de la carpeta actual
ls -al |mostrar contenido incluso oculto
ls -a| muestra el grupo de archivos pero no en una lista
ls -l|Ver todos los archivos como una lista.
ctrl+l o Commad L o clear| limpia la consola
mkdir| permite crear carpetas (por ejemplo, mkdir Carpeta-Importante)
touch| Nos permite crear archivos (por ejemplo, touch archivo.txt)
rm| Nos permite borrar un archivo o carpeta (por ejemplo, rm archivo.txt). Mucho cuidado con este comando, puedes borrar todo tu disco duro.
cat| Ver el contenido de un archivo (por ejemplo, cat nombre-archivo.txt)
history| Ver los últimos comandos que ejecutamos y un número especial con el que podemos repetir su ejecución. Si presionas la tecla Arriba puedes ver el último comando que ejecutamos.
! + número| Ejecutar algún comando con el número que nos muestra el comando history (por ejemplo, !72).
--help!|Descubrir todos los argumentos de un comando con el argumento --help (por ejemplo, cat --help)

### Credenciales | Git User Git Email
* **git config user.name** : Nombre del usuario
* **git config user.email** : Correo del usuario
* **git config --global user.name "Nombre Usuario"** : Cambiar Nombre del usuario
* **git config --global user.email "Correo Usuario"** : Cambiar Correo del usuario

## Comandos básicos
| Comando | Función|
|:-------|:------------|
 **git init** | Inicializa un repositorio git
 **git clone url_servidor_remoto** | Clonar un repositorio
**git branch** | Crear una rama|
 **git checkout <branch>**|Cambiar de una rama a otra
 **git diff** | Muestra los cambios que se han hecho en el staging area
 **git push** | Luego de hacer git add y git commit debemos ejecutar este comando para mandar los cambios al servidor remoto.
 **git pull** | Recibir los archivos de un repositorio remoto (cambios hechos por otros desarrolladores)
 **git log** | Muestra los commits hechos en el repositorio
 **git merge** | Unir dos ramas, Lo necesitamos para combinar los últimos cambios del servidor remoto y nuestro directorio de trabajo.
 
 
 ### Comandos para mover archivos entre estados de Git
| Comando | Función|
|:-------|:------------|
 **git status** | Muestra el estado de los archivos (si estan en staging area o en el respositorio)
 **git add <files>** | Agregar un archivo al staging area
 **git add .** | Agregar todos los archivos al staging area
 **git reset HEAD:**| nos ayuda a sacar archivos del estado Staged para devolverlos a su estado anterior. Si los archivos venían de Unstaged, vuelven allí. Y lo mismo se venían de Untracked.
**git commit** | nos ayuda a mover archivos de Unstaged a Tracked
**git commit -m "mensaje"** | Agregar un mensaje al commit
 **git rm:** |este comando necesita alguno de los siguientes argumentos para poder ejecutarse correctamente:
- git rm --cached: Mueve los archivos que le indiquemos al estado Untracked.
- git rm --force: Elimina los archivos de Git y del disco duro. Git guarda el registro de la existencia de los archivos, por lo que podremos recuperarlos si es necesario (pero debemos usar comandos más avanzados).


 

### Conceptos importantes
**Ciclo de vida o estados de los archivos en Git:**
Cuando trabajamos con Git nuestros archivos pueden vivir y moverse entre 4 diferentes estados (cuando trabajamos con repositorios remotos pueden ser más estados)
* **Archivos Tracked:** son los archivos que viven dentro de Git, no tienen cambios pendientes y sus últimas actualizaciones han sido guardadas en el repositorio gracias a los comandos git add y git commit.
*  **Archivos Staged:** son archivos en Staging. Viven dentro de Git y hay registro de ellos porque han sido afectados por el comando git add, aunque no sus últimos cambios. Git ya sabe de la existencia de estos últimos cambios, pero todavía no han sido guardados definitivamente en el repositorio porque falta ejecutar el comando git commit.
*  **Archivos Unstaged:** entiéndelos como archivos “Tracked pero Unstaged”. Son archivos que viven dentro de Git pero no han sido afectados por el comando git add ni mucho menos por git commit. Git tiene un registro de estos archivos, pero está desactualizado, sus últimas versiones solo están guardadas en el disco duro.
*  **Archivos Untracked:** son archivos que NO viven dentro de Git, solo en el disco duro. Nunca han sido afectados por git add, así que Git no tiene registros de su existencia.


_____


### Git Ignore - No tomar en cuenta archivos
1. Crear un archivo llamado **.gitignore** en el directorio del proyecto
2. Escribir el nombre o ruta de los archivos que no se quieren subir al repositorio
____
____
    

<div align="center">
    <h1>Uso de Github </h1>
        <img src="https://media4.giphy.com/media/KzJkzjggfGN5Py6nkT/giphy.gif?cid=ecf05e477ahax0ifww2ichfow8b28azoitatookt05vo09sl&rid=giphy.gif&ct=s" width="200px"></img> </div>
    
### ¿Qué es GitHub?
GitHub es una plataforma que nos permite guardar repositorios de Git que podemos usar como servidores remotos y ejecutar algunos comandos de forma visual e interactiva (sin necesidad de la consola de comandos).

Luego de crear nuestra cuenta, podemos crear o importar repositorios, crear organizaciones y proyectos de trabajo, descubrir repositorios de otras personas, contribuir a esos proyectos, dar estrellas y muchas otras cosas.

#### README.md
El README.md es el archivo que veremos por defecto al entrar a un repositorio. Es una muy buena práctica configurarlo para describir el proyecto, los requerimientos y las instrucciones que debemos seguir para contribuir correctamente.

 ### ¿Como Clonar un proyecto de Github?   
Para clonar un repositorio desde GitHub (o cualquier otro servidor remoto) debemos copiar la URL (por ahora, usando HTTPS) y ejecutar el comando git clone + la URL que acabamos de copiar. Esto descargara la versión de nuestro proyecto que se encuentra en GitHub.
    
Sin embargo, esto solo funciona para las personas que quieren empezar a contribuir en el proyecto. Si queremos conectar el repositorio de GitHub con nuestro repositorio local, el que creamos con git init, debemos ejecutar las siguientes instrucciones:

1. Primero: Guardar la URL del repositorio de GitHub con el nombre de origin
```    
git remote add origin URL
```
2. Segundo: Verificar que la URL se haya guardado correctamente:
```   
git remote -v
```

3. Tercero: Traer la versión del repositorio remoto y hacer merge para crear un commit con los archivos de ambas partes. Podemos usar git fetch y git merge
o solo el git pull con el flag --allow-unrelated-histories:
```
git pull origin main --allow-unrelated-histories
```

4. Por último, ahora sí podemos hacer git push para guardar los cambios de nuestro repositorio local en GitHub:
```
git push origin main
```








    
_____
### Bibliogrfía
* [Git Pagina Oficial](https://git-scm.com/)
* [Git Documentación](https://git-scm.com/docs)
