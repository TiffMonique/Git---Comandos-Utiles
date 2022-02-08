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

### Comandos básicos
| Comando | Función|
|:-------|:------------|
 **git init** | Inicializa un repositorio git
 **git status** | Muestra el estado de los archivos (si estan en staging area o en el respositorio)
**git add < files >** | Agregar un archivo al staging area
**git add .** | Agregar todos los archivos al staging area|
**git commit** | Guardar los archivos del staging area al repositorio (crear un primer snapshot)
**git commit -m "mensaje"** | Agregar un mensaje al commit|
**git branch** | Crear una rama|
 **git checkout < branch >**|Cambiar de una rama a otra
 **git diff** | Muestra los cambios que se han hecho en el staging area
 **git push** | Enviar los archivos del staging area a un repositorio remoto
 **git pull** | Recibir los archivos de un repositorio remoto (cambios hechos por otros desarrolladores)
 **git log** | Muestra los commits hechos en el repositorio
 **git merge** | Unir dos ramas
 **git clone** | Clonar un repositorio

### Conceptos importantes
**Ciclo de vida o estados de los archivos en Git:**
Cuando trabajamos con Git nuestros archivos pueden vivir y moverse entre 4 diferentes estados (cuando trabajamos con repositorios remotos pueden ser más estados)
* **Archivos Tracked:**




_____


### Git Ignore - No tomar en cuenta archivos
1. Crear un archivo llamado **.gitignore** en el directorio del proyecto
2. Escribir el nombre o ruta de los archivos que no se quieren subir al repositorio
    ```
    Practica Git/Test
    ```
_____
### Bibliogrfía
* [Git Pagina Oficial](https://git-scm.com/)
* [Git Documentación](https://git-scm.com/docs)
