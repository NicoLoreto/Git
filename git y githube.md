# Configuracion global

nicol@LAPTOP-BQ870N7O MINGW64 ~ (master)
$ git congig --global
git: 'congig' is not a git command. See 'git --help'.

The most similar command is
        config

nicol@LAPTOP-BQ870N7O MINGW64 ~ (master)
$ git config --global
usage: git config [<options>]

Config file location
    --global              use global config file
    --system              use system config file
    --local               use repository config file
    --worktree            use per-worktree config file
    -f, --file <file>     use given config file
    --blob <blob-id>      read config from given blob object

Action
    --get                 get value: name [value-pattern]
    --get-all             get all values: key [value-pattern]
    --get-regexp          get values for regexp: name-regex [value-pattern]
    --get-urlmatch        get value specific for the URL: section[.var] URL
    --replace-all         replace all matching variables: name value [value-pattern]
    --add                 add a new variable: name value
    --unset               remove a variable: name [value-pattern]
    --unset-all           remove all matches: name [value-pattern]
    --rename-section      rename section: old-name new-name
    --remove-section      remove a section: name
    -l, --list            list all
    --fixed-value         use string equality when comparing values to 'value-pattern'
    -e, --edit            open an editor
    --get-color           find the color configured: slot [default]
    --get-colorbool       find the color setting: slot [stdout-is-tty]

Type
    -t, --type <type>     value is given this type
    --bool                value is "true" or "false"
    --int                 value is decimal number
    --bool-or-int         value is --bool or --int
    --bool-or-str         value is --bool or string
    --path                value is a path (file or directory name)
    --expiry-date         value is an expiry date

Other
    -z, --null            terminate values with NUL byte
    --name-only           show variable names only
    --includes            respect include directives on lookup
    --show-origin         show origin of config (file, standard input, blob, command line)
    --show-scope          show scope of config (worktree, local, global, system, command)
    --default <value>     with --get, use default value when missing entry


nicol@LAPTOP-BQ870N7O MINGW64 ~ (master)
$ git config --global user.name
NicoLoreto

nicol@LAPTOP-BQ870N7O MINGW64 ~ (master)
$ git config --global email
error: key does not contain a section: email

nicol@LAPTOP-BQ870N7O MINGW64 ~ (master)
$ git config --global user.email
nicoloreto2@gmail.com

nicol@LAPTOP-BQ870N7O MINGW64 ~ (master)
$ git config --global core.editor
"C:\Users\nicol\AppData\Local\Programs\Microsoft VS Code\bin\code" --wait

nicol@LAPTOP-BQ870N7O MINGW64 ~ (master)
$ git config --global -e

nicol@LAPTOP-BQ870N7O MINGW64 ~ (master)
$ git  config --global core.autocrlf true

nicol@LAPTOP-BQ870N7O MINGW64 ~ (master)
$ git config -h
usage: git config [<options>]

Config file location
    --global              use global config file
    --system              use system config file
    --local               use repository config file
    --worktree            use per-worktree config file
    -f, --file <file>     use given config file
    --blob <blob-id>      read config from given blob object

Action
    --get                 get value: name [value-pattern]
    --get-all             get all values: key [value-pattern]
    --get-regexp          get values for regexp: name-regex [value-pattern]
    --get-urlmatch        get value specific for the URL: section[.var] URL
    --replace-all         replace all matching variables: name value [value-pattern]
    --add                 add a new variable: name value
    --unset               remove a variable: name [value-pattern]
    --unset-all           remove all matches: name [value-pattern]
    --rename-section      rename section: old-name new-name
    --remove-section      remove a section: name
    -l, --list            list all
    --fixed-value         use string equality when comparing values to 'value-pattern'
    -e, --edit            open an editor
    --get-color           find the color configured: slot [default]
    --get-colorbool       find the color setting: slot [stdout-is-tty]

Type
    -t, --type <type>     value is given this type
    --bool                value is "true" or "false"
    --int                 value is decimal number
    --bool-or-int         value is --bool or --int
    --bool-or-str         value is --bool or string
    --path                value is a path (file or directory name)
    --expiry-date         value is an expiry date

Other
    -z, --null            terminate values with NUL byte
    --name-only           show variable names only
    --includes            respect include directives on lookup
    --show-origin         show origin of config (file, standard input, blob, command line)
    --show-scope          show scope of config (worktree, local, global, system, command)
    --default <value>     with --get, use default value when missing entry

# git.init = inicializar un repositorio en el directorio que estoy

$ git init
Initialized empty Git repository in C:/Programacion/github.com/NicoLoreto/miweb/.git/

# Comandos

# ls listado de carpetas y archivos

nicol@LAPTOP-BQ870N7O MINGW64 /c/Programacion/github.com/NicoLoreto/lenguajes (master)
$ ls
'html y css'/   javascript/   phyton/   sql/

nicol@LAPTOP-BQ870N7O MINGW64 /c/Programacion/github.com/NicoLoreto/lenguajes (master)
$

# pwd saber donde me encuentro

$  pwd
/c/Programacion/github.com/NicoLoreto/lenguajes

nicol@LAPTOP-BQ870N7O MINGW64 /c/Programacion/github.com/NicoLoreto/lenguajes (master)
$

# cd moverme a un directorio

nicol@LAPTOP-BQ870N7O MINGW64 /c/Programacion/github.com/NicoLoreto/lenguajes (master)
$ cd javascript/
nicol@LAPTOP-BQ870N7O MINGW64 /c/Programacion/github.com/NicoLoreto/lenguajes/javascript (master)

# cd .. = salir del directorio y moverme uno atras

# mddir (nombre del directorio) = crear un directorio nuevo en donde estoy posicionado

nicol@LAPTOP-BQ870N7O MINGW64 /c/Programacion/github.com/NicoLoreto (master)
$ ls
Proyecto-Integrador/    ejerciciosEnJavaScript/  miweb/
conceptosEnJavaScript/  lenguajes/               pruebaGit/

# mostrar archivos ocultos

$ ls -a
./  ../  .git/

# ingreso al repositorio y muestro los archivos donde se van a almacenar las ramas, commit, archivos, etc. DETALLES DE IMPLEMENTACION. esta carpeta permanece ignorada y no se comparte con los demas desarrolladores

$ cd .git

nicol@LAPTOP-BQ870N7O MINGW64 /c/Programacion/github.com/NicoLoreto/miweb/.git (GIT_DIR!)
$ ls -a
./  ../  HEAD  config  description  hooks/  info/  objects/  refs/

nicol@LAPTOP-BQ870N7O MINGW64 /c/Programacion/github.com/NicoLoreto/miweb/.git (GIT_DIR!)
$

# code . = abre el editor de texto  con el directorio donde estoy

# git status

muestra el estado del repo. si no hay commit no muestra nada y si no lo selecciono no lo seguira. para seguirlo uso git add

# git add
seguir archivos. puede ser el nombre del archivo, una expresion regular (.txt) o punto que agregara todos los archivos (cuidado porq es una mala practica), usar si estoy seguro de que es codigo seguro y claro. 
En verde esta en etapa de stage.

$ git add "Hola mundo.txt"

nicol@LAPTOP-BQ870N7O MINGW64 /c/Programacion/github.com/NicoLoreto/miweb (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   Hola mundo.txt
        new file:   chanchito feliz.txt

# si hago un cambio aparecera en rojo.

 para agregar los cambios al stage uso add

$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   Hola mundo.txt
        new file:   chanchito feliz.txt

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   Hola mundo.txt

# no pasan los archivos sino los cambios

# commit
Comprometer el trabajo

# git commit -m "algo que tenga sentido"
$ git commit -m "Primer commit"
[master (root-commit) 10d5835] Primer commit
 2 files changed, 2 insertions(+)
 create mode 100644 Hola mundo.txt
 create mode 100644 chanchito feliz.txt

si pongo git commit y enter abre el editor y agrego el commit al principio

$ git commit
[master 8e1acc3] Agregando otra linea
 1 file changed, 2 insertions(+), 1 deletion(-)

cuando guardo y cierro el editor agrega el commit

# deleted = eliminar un archivo

primero veo el listado (ls), con rm elimino el archivo, con status veo que hay nuevos cambios por agregar, con add agrego el cambio. el archivo eliminado se agrega al stage. finalmente hago el commit para eliminar el archivo.

$ ls
'Hola mundo.txt'  'chanchito feliz.txt'

nicol@LAPTOP-BQ870N7O MINGW64 /c/Programacion/github.com/NicoLoreto/miweb (master)
$ rm chanchito\ feliz.txt

nicol@LAPTOP-BQ870N7O MINGW64 /c/Programacion/github.com/NicoLoreto/miweb (master)
$ git status
On branch master
Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        deleted:    chanchito feliz.txt

no changes added to commit (use "git add" and/or "git commit -a")

nicol@LAPTOP-BQ870N7O MINGW64 /c/Programacion/github.com/NicoLoreto/miweb (master)
$ git add chanchito\ feliz.txt

nicol@LAPTOP-BQ870N7O MINGW64 /c/Programacion/github.com/NicoLoreto/miweb (master)
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        deleted:    chanchito feliz.txt

$ git commit -m "Eliminando chanchito feliz"
[master b31b63d] Eliminando chanchito feliz
 1 file changed, 1 deletion(-)
 delete mode 100644 chanchito feliz.txt

$ ls
'Hola mundo.txt'

# quitar de la etapa de stage

uso restore --staged

$ git restore --staged "Hola mundo.txt"

$ git status
On branch master
Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        deleted:    Hola mundo.txt

no changes added to commit (use "git add" and/or "git commit -a")

# recuperar un archivo eliminado

uso restore y el nombre del archivo

$ git restore "Hola mundo.txt"

nicol@LAPTOP-BQ870N7O MINGW64 /c/Programacion/github.com/NicoLoreto/miweb (master)
$ ls
'Hola mundo.txt'

# cambiar el nombre de un archivo

se usa mv. primero el nombre original y desp el nuevo. entre un espacio

$ mv Hola\ mundo.txt HolaMundo

nicol@LAPTOP-BQ870N7O MINGW64 /c/Programacion/github.com/NicoLoreto/miweb (master)
$ ls
HolaMundo

# todo cambio necesita ser pasado al stage y luego commiteado

$ git add "HolaMundo"

$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        renamed:    Hola mundo.txt -> HolaMundo

$ git commit -m "Renombrando un archivo"
[master a7d2585] Renombrando un archivo
 1 file changed, 0 insertions(+), 0 deletions(-)
 rename Hola mundo.txt => HolaMundo (100%)

# puedo cambiar el nombre directamente con un comando

$ git mv HolaMundo HolaMundillo

$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        renamed:    HolaMundo -> HolaMundillo

$ git commit -m "Volviendo a cambiar el nombre"
[master 4917d53] Volviendo a cambiar el nombre
 1 file changed, 0 insertions(+), 0 deletions(-)
 rename HolaMundo => HolaMundillo (100%)

# variables de entorno

se usa para q no se pueda tener acceso a esos archivos. ej, base de datos en el local. Se usa env como standar.

tengo que crear un archivo (.gitignore) que senale la ruta a la cual no se podra acceder, archivos o carpetas.

.env.txt (archivo)
node_modules/ (carpeta)

si aparecera el archivo .gitignore. lo tengo que agregar y commitear

# git status -s

sirve para resumir la info que da status.
solo saber el estado del archivo

$ git status -s
 M .gitignore
?? archivo2.txt

M = en rojo archivo que ha sido modificado
M = en verde esta en stage
?? = no fue agregado

$ git add archivo2.txt

$ git status -s
M  .gitignore
A  archivo2.txt

A = significa q estoy agregando ese archivo

$ git commit -m "Mostrando status corto"
[master 6ec2fea] Mostrando status corto
 2 files changed, 2 insertions(+), 1 deletion(-)
 create mode 100644 archivo2.txt

# git diff

muestra los textos de los cambios que estoy por agregar, pero que todavia no pasaron a la etapa de staged. Permite comparar los cambios realizados y enviados en dos determinados commit, para esto se debe copiar la llave o indicador de cada commit.

git diff [commit vers 1] [commit vers 2]

$ git diff
diff --git a/archivo2.txt b/archivo2.txt
index 030b241..821f8e9 100644
--- a/archivo2.txt
+++ b/archivo2.txt
@@ -1 +1,3 @@
-chanchito feliz
\ No newline at end of file
+chanchito feliz
+chanchito triste
+felipe
\ No newline at end of file

- = indica lo que se elimino
+ = indica lo que se agrego

indica que la elimino porq no habia salto de linea
el salto de linea se agrega sobre chanchito feliz, entonces lo elimina y lo vuelve a agregar

@@ -1 +1,3 @@ = indica que desde donde comienza y las lineas que extrajo (cambio)

# git diff --staged
muestra los cambios que esten en la etapa de stage

$ git diff --staged
diff --git a/archivo2.txt b/archivo2.txt
index 030b241..821f8e9 100644
--- a/archivo2.txt
+++ b/archivo2.txt
@@ -1 +1,3 @@
-chanchito feliz
\ No newline at end of file
+chanchito feliz
+chanchito triste
+felipe
\ No newline at end of file

# git log

muestra el historial del repositorio

$ git log
commit 6ec2feaa54c7fe988109c96c3294049671b2463e (HEAD -> master)
Author: NicoLoreto <nicoloreto2@gmail.com>
Date:   Fri Jul 1 19:32:59 2022 -0300

    Mostrando status corto

commit 9fb691b7ca9d75ae15559c47ace8366b70b7deaf
Author: NicoLoreto <nicoloreto2@gmail.com>
Date:   Fri Jul 1 19:23:40 2022 -0300

    agregando .gitignore

commit 4917d53f39107b54003821a983e08c924ce6e173
Author: NicoLoreto <nicoloreto2@gmail.com>
Date:   Fri Jul 1 18:59:30 2022 -0300

    Volviendo a cambiar el nombre

commit a7d25857eb830fe151b9033d90f7e31529a80a22
Author: NicoLoreto <nicoloreto2@gmail.com>
Date:   Fri Jul 1 18:56:48 2022 -0300

    Renombrando un archivo

# git log --oneline

muestra el hisotial con un has que sera indentificador unico de cada commit. ademas muestra el mensaje

$ git log --oneline
6ec2fea (HEAD -> master) Mostrando status corto
9fb691b agregando .gitignore
4917d53 Volviendo a cambiar el nombre
a7d2585 Renombrando un archivo
b31b63d Eliminando chanchito feliz
8e1acc3 Agregando otra linea
10d5835 Primer commit

git log -S "palabra" = muestra los commit que contienen la palabra en los mens o el contenido

git log --grep "palabra" =  muestra los commit en los mensajes 

# ramas

Una rama es un nombre que se da a un commit, a partir del cual se empieza a
trabajar de manera independiente y con el que se van a enlazar nuevos
commits (de esa misma rama).

Por regla general a master se la considera la rama principal y la raíz de la mayoría de las demás ramas. Lo más habitual es que en master se encuentre el "código definitivo", que luego va a producción, y es  la rama en la que se mezclan todas las demás.

git checkout -b "nombre_rama"
Este comando es una fusión entre “git branch” y “git
checkout”, y crea una rama llamada “nombre_rama” y a la vez
hace un checkout de la rama “nombre_rama”

origin/master = Es una rama
remota, es una copia local de la
rama llamada "master", en el
repositorio remoto llamado
"origin"

GIT FLOW
Es una una guía que nos da ciertos
estándares para manejar la
ramificación de nuestros
proyectos


1. rama master = rama por defecto al iniciar un repo
2. rama develop = rama en la que está el código que conformará la siguiente versión planificada del proyecto.
3. rama release = ramas que se generan a partir de la rama develop y se incorporan a esta o a master. Se utilizan para
preparar el siguiente código en producción, se hacen los últimos ajustes y se corrigen los últimos bugs antes de pasar el código a producción incorporándolo a la rama master.
4. FEATURE ó TOPIC BRANCHES = Ramas que se generan a partir de la rama develop
y se incorporan siempre a esta. Se utilizan para
desarrollar nuevas características de la
aplicación.
5. RAMAS HOTFIX = Ramas que se generan a partir de la rama master
y se incorporan siempre a esta o develop. Se
utilizan para para corregir errores y bugs en el
código en producción. Funcionan de forma parecida
a las ramas Releases, siendo la principal diferencia
que los hotfixes no se planifican

salir del seguimiento lineal, para cuando estemos seguros de nuestro codigo volver a la rama principal. BRANCH

es independiente de la rama principal y desp podemos solicitar un merge para volver a la rama principal

$ git branch
* master

indica en que rama estoy.

Para crear una rama escribo checkout -b (nombre de la rama)

$ git checkout -b ramaB
Switched to a new branch 'ramaB'

agrego y commiteo y muestro el historial
el ultimo commit lo hice desde la ramaB

$ git log --oneline
3a1d12d (HEAD -> ramaB) Agregando otro chanchito desde la ramaB
6ec2fea (master) Mostrando status corto
9fb691b agregando .gitignore
4917d53 Volviendo a cambiar el nombre
a7d2585 Renombrando un archivo
b31b63d Eliminando chanchito feliz
8e1acc3 Agregando otra linea
10d5835 Primer commit

git branch -v = lista ramas locales

git branch -f = lista ramas remotas

git branch -a = lista todas las ramas

# cat
muestra el contenido del archivo

$ cat archivo2.txt
chanchito feliz
chanchito feliz

si me cambio a la rama master no muestra ese cambio

$ git checkout master
Switched to branch 'master'

nicol@LAPTOP-BQ870N7O MINGW64 /c/Programacion/github.com/NicoLoreto/miweb (master)
$ cat archivo2.txt
chanchito feliz

# para traer los cambios tengo que escribir desde rama master git merge y la rama desde donde tengo que traer

$ git merge ramaB
Updating 6ec2fea..3a1d12d
Fast-forward
 archivo2.txt | 1 +
 1 file changed, 1 insertion(+)

 # subir a githube

 creo un repositorio en githube

 copio el git remote add origin y la pego en la terminal. indica si voy a tener un servidor remoto donde subir los cambios

 git remote add origin https://github.com/NicoLoreto/miweb.git

 # git push

 para githube es el comando para subir los cambios con respecto a la rama en la que este trabajando. main no esta creada en githube asiq lo hago con -u. origin donde sera creado y desp el nombre.
 yo tengo master, no main.

git push -u origin master

para subir a githube desde una rama

$ git checkout -b ramaC
Switched to a new branch 'ramaC'

nicol@LAPTOP-BQ870N7O MINGW64 /c/Programacion/github.com/NicoLoreto/miweb (ramaC)
$ push -u origin ramaC
bash: push: command not found

nicol@LAPTOP-BQ870N7O MINGW64 /c/Programacion/github.com/NicoLoreto/miweb (ramaC)
$ git push -u origin ramaC
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'ramaC' on GitHub by visiting:
remote:      https://github.com/NicoLoreto/miweb/pull/new/ramaC
remote:
To https://github.com/NicoLoreto/miweb.git
 * [new branch]      ramaC -> ramaC
branch 'ramaC' set up to track 'origin/ramaC'.

# ver en que repositorio remoto estoy

git remote -v

$ git remote -v
origin  https://github.com/NicoLoreto/Git.git (fetch)
origin  https://github.com/NicoLoreto/Git.git (push)

# cambiar nombre a repositorio remoto

git remote add [nombre] [url]

$ git remote add Git_y_Githube https://github.com/NicoLoreto/Git.git

nicol@LAPTOP-BQ870N7O MINGW64 /c/Programacion/ISPC/2022/1 cuatrimestre/Programador/Metodologías Agiles y Gestión de Proyectos (master)
$ git remote
Git_y_Githube
origin

# Git show = Permite ver el ultimo commit y los cambios realizados en el archivo

# git reset = Permite volver a una versión anterior, sin poder volver al estado
anterior pero tiene dos atributos principales.

--hard = Permite restablecer      
al estado anterior,
todo vuelve como
estaba. Es el más
peligroso porque
borra todo y no
mantiene nada.

--soft = Permite restablecer al
estado anterior, pero
mantiene en staging los
commits "eliminados". Es
decir, el directorio de
trabajo vuelve a la versión
del commit seleccionado.

--mixed = Permite restablecer al estado anterior, pero mantiene en Working
Directory los commits "eliminados". Es decir, el directorio de trabajo
se restablece, pero deja en el directorio local los cambios realizados
posterior al commit seleccionado.

git log --stat = Permite ver los cambios específicos que se hicieron, en
cuales archivos, por cada commit.

git checkout = Permite volver a una versión anterior, es decir ver
como era el archivo en un determinado commit, en
realidad no ha cambiado todavía, lo que hace es pasarlo
al staging.
git checkout [Hash del commit] archivo.txt

git checkout master = Permite ver a la versión master del archivo, es decir la ultima versión
que se había enviado en el ultimo commit.
git checkout master archivo.txt

# git fetch

Lo usamos para traer actualizaciones del servidor remoto y guardarlas en
nuestro Local Repository. Traemos los cambios que no tenemos pero no lo
lo combina automáticamente con tu trabajo ni modifica el trabajo que llevas
hecho.

# git merge

Este comando se ejecuta para combinar los últimos cambios traídos del
servidor remoto (con git fetch), y nuestro Working Directory.

# git pull

Este comando se emplea para extraer y
descargar contenido desde un repositorio
remoto y actualizar al instante el proyecto
local para reflejar ese contenido.
Básicamente, git fetch y git merge  al
mismo tiempo.

git fetch nombre-rama 
#Trae los cambios del
repositorio remoto, crea
la rama y los deja en esta.
Luego debemos fusionar
con otra rama de nuestro
proyecto.
git pull nombre-remoto
nombre-rama  
#Trae los cambios del
repositorio remoto
llamado "nombreremoto" y los fusiona
con la rama "nombrerama"
git push nombre-remoto
nombre-rama
#Envía los cambios de
nuestro Local
Repository al
repositorio remoto
llamado "nombre-remoto"
y la rama "nombre-rama"

# add y commit a la vez = Puedo utilizar git commit -am "Mensaje" para hacer un add y un commit a la vez, solo para archivos previamente guardados.

git branch -v #para ver la última
confirmación de cambios en cada
rama
git branch --merged #ver las
ramas que han sido fusionadas con
la rama activa
git branch --no-merged #mostrar
todas las ramas que contienen
trabajos sin fusionar
git branch -D #Permite borrar la
rama, forzando el borrado incluso
si se tiene trabajos sin fusionar.
Se pierde el trabajo contenido en
ella.

# git branch -l

Comando para
ver la lista de los
branchs del
proyecto,
además que
indica la rama
actual

# git merge -d "nombre rama"
Comando que permite eliminar una rama, cuando esta ya no se va a usar, y
estamos seguros que el merge fue exitoso y no tiene trabajos sin fusionar

# git mergetool = Arranca una
herramienta visual en
consola que permite resolver
conflictos.

# git mergetool = Arranca una
herramienta visual en
consola que permite resolver
conflictos.

git reset --merge HEAD = Si hemos realizado
un merge con una rama con
la que no queríamos.

Para resolver el conflicto, se tiene que elegir
manualmente el contenido de uno o de otro lado.

✓ Una vez que se resolvieron los conflictos, se debe agregar los cambios, ejemplo:
git commit -am "Solucioné el conflicto de las ramas"

# GITHUBE

GitHub es una forja para alojar proyectos utilizando el sistema de control de
versiones Git. Se utiliza principalmente para la creación de código fuente de
programas de ordenador.

git clone "URL"
Comando para clonar un repositorio desde
GitHub (o cualquier otro servidor remoto)
debemos copiar la URL (por ahora, usando
HTTPS) y ejecutar el comando  git clone + la URL
que acabamos de copiar.

Conectar el repositorio de GitHub con
nuestro repositorio local:
1. Guardar la URL del repositorio de GitHub con el nombre origin. git remote add origin "URL".
2. Verificar que la URL se haya guardado correctamente. git remote git remote -v
3. Debemos traer la versión del repositorio remoto y hacer merge para crear
un commit con los archivos de ambas partes. Podemos usar git fetch y git
merge o solo el git pull, pero para forzar se debe usar: git pull origin master --allow-unrelated-histories
4.  Por último, ahora sí podemos hacer git push para guardar los cambios de nuestro repositorio local en GitHub

# llaves

Las llaves publicas y privadas sirven para compartir información en Internet de una forma
segura, incluso si el mensaje es interceptado la probabilidad de que se pueda descifrar es
casi nulo, si no se tiene la llave privada. Este método se usa incluso en el mundo
financiero.
Importante: Nunca compartir la llave privada porque con esta, pueden acceder a tus
proyectos, incluso los de tus clientes y perder TU información.

La criptografía asimétrica, también llamada criptografía de clave
pública o criptografía de dos claves, es el método criptográfico
que asegura que un mensaje enviado no pueda ser leido por ninguna
otra persona que la persona destinataria del mensaje.

La llaves se crean con un
proceso algoritmico y
esan vinculadas
matematicamente una
con la otra, de esta
manera estan asociadas.

Claves públicas y privadas
Empecemos por lo básico.

El protocolo SSH utiliza una técnica de criptografía llamada encriptación asimétrica. Este término puede parecer complicado y extraño, pero nada más lejos de la realidad.

Básicamente, el cifrado asimétrico es un sistema que utiliza un par de claves, a saber, las claves pública y privada.

Como puedes adivinar, la clave pública se puede compartir con cualquiera. Su objetivo principal es cifrar los datos, convirtiendo el mensaje en un código secreto o texto cifrado. Esta clave suele enviarse a otros sistemas -por ejemplo, servidores- para cifrar los datos antes de enviarlos por Internet.

Por otro lado, la clave privada es la que debes guardar para ti. Se utiliza para descifrar los datos cifrados con tu clave pública. Sin ella, es imposible descifrar tu información encriptada.

Este método permite que tú y el servidor mantengáis un canal de comunicación seguro para transmitir la información.

Esto es lo que ocurre en segundo plano cuando te conectas a un servidor mediante SSH:

El cliente envía la clave pública al servidor.
El servidor pide al cliente que firme un mensaje aleatorio cifrado con la clave pública utilizando la clave privada.
El cliente firma el mensaje y envía el resultado al servidor.
Se establece una conexión segura entre el cliente y el servidor.
Es importante mantener tus claves privadas a salvo y no compartirlas con nadie bajo ninguna circunstancia. Son literalmente la clave de toda la información que se te envía.

# generar claves ssh


nicol@LAPTOP-BQ870N7O MINGW64 ~ (master)
$ ssh-keygen -t ed25519 -C nicoloreto2@gmail.com
Generating public/private ed25519 key pair.
Enter file in which to save the key (/c/Users/nicol/.ssh/id_ed25519):

ssh-keygen: La herramienta de línea de comandos utilizada para crear un nuevo par de claves SSH. Puedes ver sus banderas con ssh-keygen help
–t ed25519: La bandera -t se utiliza para indicar el algoritmo utilizado para crear la firma digital del par de claves. Si tu sistema lo soporta, ed25519 es el mejor algoritmo que puedes utilizar para crear pares de claves SSH.
-C «email»: La bandera -c se utiliza para proporcionar un comentario personalizado al final de la clave pública, que suele ser el correo electrónico o la identificación del creador del par de claves.

# Tags y versiones en Git y GitHub

 Git tiene la posibilidad de
etiquetar puntos específicos del historial como importantes. Esta
funcionalidad se usa típicamente para marcar versiones de lanzamiento
(v1.0, por ejemplo).
git tag -a nombre-del-tag - m "mensaje" HASH-a-etiquetar
Comando para crear un tag y asignarlo a un determinado commit (hash)

# git tag = Comando para revisar la lista de tags creados.

# git show-ref --tags = Comando para revisar la lista de tags creados y sus referencias

# git push origin --tags = Comando para enviar los tags creados al repositorio remoto, y si revisamos en Github, comprobamos que el tag ha sido creado.

# git tag -d nombre-del-tag = Comando para eliminar un tag

Luego de eliminar y enviar los cambios a GitHub (git pull y luego git push origin —tags), nos damos cuenta que todavía aparecen los tags en Github, por ello hacemos lo siguiente: git push origin :refs/tags/nombre-del-tag
Comando para eliminar un tag y su referencia en el repositorio remoto, de esta forma borrar de la lista de tags de Github.

git tag -a nombre-tag -m
"mensaje" # si se omite el
HASH, el tag se referencia
al commit actual

git tag -l # comando para
ver la lista de tags
git show nombre-tag #
comando para ver la
información de la etiqueta
junto con el commit que
está etiquetado
Comandos útiles

git push origin nombretag # comando para enviar
un tag determinado a
Github

git config --global
alias."nombre del alias" "git
log --all --graph --decorate
--oneline" # comando para
guardar un alias en las
configuraciones de git, para
ejecutar 

git "nombre del alias", #En
este caso mostrará el log de
forma 'grafica'.

# Manejo de ramas en GitHub

git branch = Comando para revisar las ramas creadas, pero si queremos ver más
detalles podemos usar los siguientes comandos.

git show-branch
git show-branch —all

Comandos para revisar las ramas
creadas con su ubicación (remoto o
local), pero además nos muestra la
historia mas reciente de esas
ramas y sus commits. 

gitk = Con gitk podemos ver
toda la historia de
nuestro proyecto en
un software para
verlo de forma visual.

VAMOS A CREAR DOS RAMAS, FOOTER Y HEADER Y LUEGO LA ENVIAREMOS A GITHUB.
Nos ubicamos en la rama master con
git checkout master
git push origin "nombre rama"
Creamos la dos ramas: git branch header
y git branch footer

git push origin "nombre rama" = Comando para enviar a Github (origin)

> git push origin header
> git push origin footer
Con esto enviamos las ramas
a nuestro repositorio
remoto (Github).

git push origin --delete nombre-rama = Comando para eliminar un rama remota (en Github). Básicamente, lo que hace es eliminar el apuntador del servidor.

# Configurar múltiples colaboradores en un repositorio de Github

Podemos añadir a cada persona de nuestro equipo como colaborador de nuestro
repositorio.
1. En GitHub, visita la página principal del repositorio
2. Debajo de tu nombre de repositorio, da clic en Settings.
3. En la barra lateral izquierda, da
clic en Manage access
4. Da clic en Invite a collaborato
5. Comienza a teclear el nombre de la persona
que deseas invitar dentro del campo de
búsqueda. Posteriormente, da clic en algún
nombre de la lista de coincidencias. Despues
click en "Add [user] to [repository]"
El usuario recibirá un correo
electrónico invitándolo al
repositorio.
Se verifica que tenga la opción
Edit en algún archivo para
confirmar que el proceso fue
exitoso.
6. Click en View invitation y
luego de ingresar a su cuenta
Accept invitation.
Una vez que el colaborador
acepte la invitación, tendrá
acceso de colaborador a tu
repositorio.

# Flujo de trabajo profesional: Haciendo merge de ramas de desarrollo a master

Las ramas pueden tomar
diferentes caminos como partes del desarrollo del trabajo, pero que en algún momento, debemos
unirlos. Para esto, debemos elegir una rama principal y tener claro cual es el procedimiento para
tener éxito en la fusión de todos los avances y/o updates del proyecto

# Flujo de trabajo profesional con Pull requests

Es la acción de validar un código que se va a mergear de una rama a otra. En este
proceso de validación pueden entrar los factores que queramos: Builds
(validaciones automáticas), asignación de código a tareas, validaciones manuales
por parte del equipo, despliegues, etc.

En un entorno profesional
normalmente se bloquea
la rama master, y para
enviar código a dicha rama
pasa por un code review y
luego de su aprobación se
unen códigos con los
llamados pull request.

Los pull request no es
una caracteristica de
Git , si no de Github.
Los pull request podrían compararse con un control de calidad interno donde el equipo tiene la
oportunidad de detectar bugs o código que no sigue lineamientos, convenciones o buenas
prácticas. Incluso puede presentar ahorros a la empresa. Github nos permite llevar un control e
implementa un proceso para la atención y revisión de estas solicitudes.

La persona que hace todo esto, normalmente son los lideres de equipo o un perfil
muy especial que se llama DevOps (permite que los roles que antes estaban
aislados se coordinen y colaboren para producir productos mejores y más
confiables)

# Utilizando Pull Requests en GitHub

 Una vez realizada la corrección y enviado los cambios de la rama, Gihub
nos alerta de un push reciente y nos da la opción para comparar y crear un
Pull Request

Para crear un pull request debemos
dar click en "Compare & pull request"

Una vez creado el pull request, al
administrador recibirá una notificación

 El administrador puede comparar los
cambios haciendo click en Files changed,
y consultar con el equipo para la revisión
respectiva.

Dar click en Review Changes, en
caso de requerir cambios al solicitante.


Al solicitante, se le notifica del
cambio requerido ingresando en Pull
Requests

Una vez realizados los cambios
requeridos responder el Pull Request

 Podemos aprobar los cambios, en
Review Changes y Approve

El solicitante recibe una
notificación de aprobación de su
solicitud.


 Finalmente, el administrador o el
Devops debe hacer el merge con la
rama principal

Si se requiere , podemos eliminar la rama ya
que fue creada solo para solucionar un error
(Delete Branch)

# Creando un Fork, contribuyendo a un repositorio

Si quieres participar en un proyecto existente, en el que no tengas permisos
de escritura, puedes bifurcarlo (hacer un “fork”). Esto consiste en crear una
copia completa del repositorio totalmente bajo tu control: se almacenará en
tu cuenta y podrás escribir en él sin limitaciones.


visita la página del mismo y
pulsa sobre el botón
“Fork” del lado superior
derecho de la página.
En unos segundos te redireccionarán a una página nueva de proyecto,
en tu cuenta y con tu propia copia del código fuente.
Con esto podemos clonar el proyecto a nuestro repositorio local (git clone)
y podemos realizar cualquier cambio y aporte.

Para que nuestros cambios se fusionen en el repositorio remoto original, podemos
hacer un pull request y esperar que se realice el merge con el original.


Github nos advierte, si la rama del
repositorio original tiene commits, que el
repositorio forkeado no.
Para traer estos cambios al repositorio forkeado,
debemos agregar una nueva fuente remota:
git remote add upstream url-repositorio-original
Luego traemos los cambios del original, para actualizar en el
repositorio forkeado:
git pull upstream master # traemos cambios del repositorio original
git push origin master #enviamos cambios a nuestro repositorio forkeado

En un proyecto público
podemos dar click en
Watching y Star para
seguir el repositorio, de
esta manera apoyamos y
recibimos avisos cada
vez que hay cambios en
dicho repositorio.

# Ignorar archivos en el repositorio con .gitignore

Las reglas sobre los patrones que puedes incluir en el archivo .gitignore
son las siguientes:
Ignorar las líneas en blanco y aquellas que comiencen con #.
Aceptar patrones glob estándar.
Los patrones pueden terminar en barra (/) para especificar un
directorio.
Los patrones pueden negarse si se añade al principio el signo de
exclamación (!)

.Gitignore sirve para decirle a Git qué archivos o directorios completos debe ignorar y no subir al
repositorio de código. Únicamente se necesita crear un archivo especificando qué elementos se deben
ignorar y, a partir de entonces, realizar el resto del proceso para trabajo con Git de manera habitual

# Githube page sirve para alojar sitios gratis desde githube

# git stash
almacena temporalmente los cambios y posteriormente los deshace 

git stash pop se eliminan los cambios y se vuelven a aplicar al cod

git stash branch nombre-rama = crear una rama nueva basada en la confirmacion a partir de la cual se creo el stash

git stash list = listar los stash, muestra el num de stash

git stash drop = eliminar stash

git stash clear = elimina todos los stash

# git clean -f

eliminar los archivos sin seguimiento en un directorio de trabajo del repo

# git clean -n = simulacro de borrado

# git clean -d = tmb los directorios sin seguimiento

# git clean -x = que incluya tmb los archivos ignorados

# git cherry-pick [hash] [hash1] [hash2] = permite elegir una confirmacion de una rama y aplicarla a otra

nos ubicamos en la rama donde vamos a llevar esa conf y ejecutamos

# git commit -amend = modificar la conf mas reciente, cambiar la conf del mensaje o cambiar o remover archivos

git commit ammend -m = escribir un nuevo mensaje 

(las confirmaciones no pueden editarse, este comando lo que hace es enmendar una confirmacion haciendo otra)

# git reflog = referencia de los ultimos 90 dias

# git reset = deshace los cambios locales 

# git grep =  busca a traves de los archivos en el directorio

git grep -n "palabra"

# git shortlog = agrupa cada conf pot autor. forma de ver quien estuvo trabajando en que.

git shortlog -n = salida segun el numero de conf por auto

git shortlog -e = correo electronico de cada autor

git "alias" = alias para cada comando. git conf --global alias.alias-q-quiero 'comando'

# git blame = quien fue el ultimo q modifico la linea

git blame "nombreArchivo"






















