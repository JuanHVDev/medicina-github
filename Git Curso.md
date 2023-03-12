git --version: Te da la version de git que tienes instalado.
git help: te da descripciones de cada comando.
git config --global user.name "": Para el nombre de usuario
git config --global user.email "": Para el correo.
git init: Inicializa un repositorio
git config --global init.defaultBranch: para cambiar el nombre de la rama a "main"
git status: te da la rama en la que estás, y el estado en el que se encuentran los archivos del repositorio si no se les da un seguimiento.
git add . = Agrega todos los archivos al repositorio.
git reset <nombre del archivo>: para eliminar el archivo.
git commit -m "Primer commit": toma la fotografia
git checkout -- . : reconstruye el proyecto como estaba en el ultimo commit.
git bran -m master main: cambia el nombre de la rama del repositorio.
git commit -am <Mensaje>: Solo funciona si ya le dan seguimiento al archivo
git log: Te muestra todos los commits 
git status --short: Te muestra el archivo muy resumido
Para hacer un alias tienes que poner:
git config --global alias.<comoquierestualias> <loquequieresquehaga> ejemplo: git congif --global alias.s "status --short"
git diff: te muestra que cambio en un archivo
git diff --staged: Te muestra los cambios.
git commit --amend -m "Mensaje": Para arreglar un mensaje del ultimo commit 
git reset --soft HEAD^ :Modificar un commit anterior al ultimo
git reset --soft HEAD^numero: Modificar el commit segun su numero.
## Un viaje en el tiempo
git init
git add README.md
git commit -m "README agregado"
git add misiones.md
git commit -m "agragamos misiones"

git reset --mixed [hash]: Quita del stage y los cambios se mantienen para que los vuelvas a añadir.
git reset --hard [hash] :Quita del stage y regresa al estado que se encontraba en el comit con el hash dado
git reflog: te muestra todos los commit y los reset que se han hcho.
Cambiar el nombre y eliminar archivos mediante git:
git mv (nombre del archivo) (nuevo nombre del archivo)
Eliminar archivos:
git rm nombre-del-archivo
Ramas
git branch ramanueva: para hacer nueva rama
git checkout ramaname: para cambiar a la rama que quieres
git branch: te enlista todas tus ramas
Para traer los cambios de una rama a la rama original debes de estar en está ultima.
git merge rama(que tiene los cambios)
eliminar una rama mediante:
git branch -d nombre-de-la-rama-a-eliminar
crear una rama y moverme a ella con:
git checkout -b nombre-de-la-rama
crear un tag:
git tag nombre-del-tag
git tag: te muestra todos los tags
eliminar un tag: git tag -d nombre-del-tag
trabajar en modo versiones-
Ejemplo: git tag -a v.1.0.0 -m "Version 1.0.0 lista"
Poner un tag a un commit anterior
git tag -a v0.1.0 el-hash-del-commit- -m "Version alpha de la aplicacion"
git show v0.1.0 te muestra todo lo referente de esa version.
stash
git stash
git stash list te enumera todos los stash que tengas
git push --tags sube todos los tags que tienes.