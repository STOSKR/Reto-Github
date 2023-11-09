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
----------------------------------------------

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







