# Reto-Github
Esto son algunos apuntos que he tomado durante mi aprendizaje del curso de Microsoft Learn y Github

MÓDULO 1

git --version (te devuelve la versión)

git config --global user.name “STOSKR” (registra un usuario global con nombre)

git config --list (devuelve la lista de los elementos actuales)

git init -b main (inicia un nuevo branch que se llama main)

git status (ver estado del árbol)

ls -Hidden (ver archivos ocultos, empezados por un punto)

git add (para almacenar los cambios provisionalmente)

git commit (confirmar cambiso para subir)

git log (ver historial de commits)

git help (pedir ayuda sobre posibles comandos)

---------------------------------------------

MÓDULO 2

touch index.html 
(code index.html desde VS code en Windows)

git commit -a -m "Texto" (-a para guardar todos los archivos cambiados, pero no agrega archivos nuevos)

git diff (ver cambios realizados), se puede agragar HEAD al final de la instrucción para comparar con la última confirmación

Es muy importante crear un archivo ".gitignore" agregando
    *.bak
    *~
Para ignorar los archivos terminados en ".bak" o "~"

git add -A (-A para agregar todos los archivos sin seguimiento y no omitidos, como los cambiados)

git diff HEAD^ (Comparar las últimas dos confirmaciones)

git status, solo sigue los cambios en los archivos y no en los directorios

git log --oneline (lista concisa de cambios), se puede añadir -nX donde X es el número de líneas que se quiere mostrar

Después de corregir errores se puede utilizar:
git commit --amend --no-edit (--amend para guardar en la misma confirmación que la original y --no-edit para no modificar el mensaje de confirmación)

git checkout -- file_name, si se borra algún archivo por accidente, se puede recuperar de esta forma, siendo file_name el nombre del archivo y -- sirve para 

git rm archivo.extension, guarda en su índice que se ha borrado ese archivo

git reset HEAD index.html, revierte la eliminación del archivo del almacenamiento provisional. Después se utiliza git checkout para recuperar el archivo al disco

git revert, cancela la última confirmación anterior

git revert HEAD, realiza una confirmación exactamente opuesta a la última, dejando el historial intacto

Existen varios tipos de restablecimiento:
    - Por defecto, --mixed, restableceel índice pero no el arbol de trabajo, también mueve HEAD si se especifica otra confirmación
    - --soft, solo mueve HEAD y deja el índice y el 
    árbol de trabajo sin cambios (todos los cambios como pedientes de confirmar)
    - --hard, cambia el índice y el árbol de trabajo para que concidan con la confirmación especificada. Los vambiso realizados en los archivos seguidos se descartan

----------------------------------------------

MÓDULO 3

git clone, puede clonar un repositorio independientemente de dónde esté almacenado

origin, referencia al repositorio original

git pull, para incorporar cambios confirmados de origin

scp, copia todo

git request-pull -p origin/main, solicitud de incorporación de cambios. Para evitar errores de incorporación

pwd, para comprobar la ubicación de la carpeta

Se puede volver a usar git config user.name para crear otro usuario y otro correo

----------------------------------------------

MÓDULO 4

git branch, creación de ramas

git checkout, cambio entre ramas

git merge, combinar ramas
    --ff-only BRANCH, produce error si main ha cambiado 
    
Primero se hace el cambio a la rama principal y después se hace merge para combinar con la rama deseada



