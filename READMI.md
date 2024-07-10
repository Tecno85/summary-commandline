# La Terminal o Linea de Comandos

Git Bash es una herramienta que proporciona una interfaz de línea de comandos y un entorno de emulación de bash (shell) en Windows. Está diseñada para permitir a los usuarios de Windows usar comandos de Git en un entorno similar al de Unix.

¿Qué es Git?

Git es un sistema de control de versiones distribuido que permite a los desarrolladores rastrear y gestionar cambios en el código fuente de un proyecto. Es muy útil para colaborar con otros desarrolladores y mantener un historial de cambios.

¿Qué es Bash?

Bash (Bourne Again Shell) es una interfaz de línea de comandos y un lenguaje de comandos utilizado en sistemas Unix y Linux. Permite a los usuarios ejecutar comandos, scripts y programas.

¿Qué es Git Bash?

Git Bash combina estas dos herramientas. Proporciona una terminal de comandos de Git en un entorno de Bash en Windows. Esto significa que puedes usar comandos de Git y comandos de Bash en la misma terminal.

Ventajas de usar Git Bash

Comandos Unix en Windows: Puedes usar comandos típicos de Unix como ls, grep, cat, entre otros.
Comandos de Git: Puedes ejecutar todos los comandos de Git, como git clone, git commit, git push, etc.
Entorno Consistente: Proporciona un entorno similar al de Linux, lo cual es útil si trabajas en proyectos que también se desarrollan en sistemas Unix o Linux.

GraphicUserInterface (GUI) Ventanas Gráficas VS CommandLineInterface (CLI) Líneas de Comandos.

## Comando Básicos

- (PrintWorkDirectory) **_pwd_**: Esta línea de comando imprime en pantalla el directorio de trabajo actual.
- (quien soy) **_whoami_**: Esta línea de comando muestra el usuario actual de la computadora.
- **_help_**: Esta línea de comando imprime todos los comando que nos brindan ayuda.
  Se puede usar este comando de dos formas diferentes:

1. **_help pwd_**: Esta manera permite entrar a la opción de ayuda del comando **_pwd_**. Para utilizarlo se escribe la palabra **_help_**, seguido de un espacio más el nombre del comando, en este caso **_pwd_**.
1. **_pwd --help_**: Esta es otra manera para ingresar a la opción de ayuda del comando **_pwd_**. Para utilizarlo se escribe la palabra **_pwd_**, seguido de un espacio más la palabra **_--help_**.

- **Historial de comandos**: Este nos muestra los ultimos 20 comando ejecutados. Para acceder ha ellos solo se debe dar click en las flechas de arriba y abajo.

- _**clear**_: Este comando nos permite limpiar la pantalla.

- **_ls_**: Este comando nos muestra el listado de los archivos que estan en nuestra ubicación. Este comando tiene unas variantes:

1. **_ls -l_**: Este comando muestra el listado de los archivos con varios datos que especifican no solo la ubicación sino fecha, hora de creacion etc.
1. **_ls -a_**: Este comando muestra el listado de todos los archivos incluyendo los ocultos.
1. **_ls -la_**: Este comando muestra el listado de todos los archivos incluyendo los ocultos con varios datos que especifican no solo la ubicación sino fecha, hora de creacion etc.
1. (Change Directory) **_cd_**: Este comando permite cambiar de ubicación de carpeta o directorio.

Para moverte a una ubicación en Git Bash que contiene espacios en el nombre, puedes utilizar comillas para encapsular la ruta completa, o puedes usar la barra invertida ( \ ) antes del espacio. Aquí tienes dos formas de hacerlo:

- _Usando Comillas_: `cd "My Documents"` o `cd 'My Documents'` o `cd "C:/Users/TuUsuario/My Documents/Carpeta"` , se puede usar comillas dobles o simples.

- _Usando Barra invertida_: `cd My\ Documents` o `cd C:/Users/TuUsuario/My\ Documents/Carpeta`.

### Comandos para cambiar de Directorios

- (change directory) `cd`: Este comando tiene como significado "cambiar directorio". Cuando se usa solo, sin ningún argumento, te lleva al directorio home del usuario. Ejemplo: Si estás en `/home/usuario/proyectos/proyecto1` y ejecutas `cd`, volverás a `/home/usuario.`

- `cd .` : El comando `cd .` en la terminal se usa para cambiar al directorio actual. Es un comando que realmente no hace nada porque el punto ( . ) representa el directorio actual en Unix y sistemas similares. Por lo tanto, cuando ejecutas `cd .` simplemente le estás diciendo a la terminal que cambie al directorio en el que ya estás. Este comando podría ser útil en scripts o comandos automatizados donde se desea asegurar que el contexto no cambia accidentalmente, pero en la mayoría de los casos de uso interactivo, no tiene un efecto práctico.

- `cd ..` : Este comando en la terminal se utiliza para moverse al directorio padre del directorio actual en el que te encuentras. Ejemplo: Si estás en `/home/usuario/proyectos/proyecto1` y ejecutas `cd ..`, subirás a `/home/usuario/proyectos`.

- `cd ~`: Este comando regresa a la carpeta principal, al home o carpeta del usuario que este utilizando el computador. Hay se utiliza el comando `cd` seguido por el símbolo de la "Virgulilla" `~`.

- `cd -` : Este comando en la terminal se utiliza para moverse al directorio padre del directorio actual en el que te encuentras, y además te muestra en la ruta en que estas. Esto a diferencia del comando `cd ..`, el cual regresa al directorio anterior pero no te muestra la ruta en la que te deja.  

- `cd /` : Este comando en la terminal se utiliza para cambiar el directorio de trabajo al directorio raíz del sistema de archivos.

- `cd ../..` : Este comando en la terminal se utiliza en la terminal para cambiar el directorio de trabajo actual dos niveles hacia arriba en la jerarquía de directorios.

### Comandos para crear Archivos y visualizar su contenido

- `touch` : El comando touch se utiliza para crear un archivo vacío y se coloca al final la extensión. Ejemplo: `touch nombre_del_archivo.txt`

- `echo`: Este comando permite crear un archivo y añadir contenido usando redireccionamiento (>). Por ejemplo: `echo "Este es el contenido del archivo" > nombre_del_archivo.txt`

- `cat`: Este comando permite visualizar el archivo desde la terminal. Ejemplo: `cat ivan_dario_madrid_daza.txt`

### Comandos para crear Carpetas

- `mkdir`: Este comando me permite crear una carpeta. Ejemplo: `mkdir Emma`. Cuando se quiere crear un archivo que contenga espasio hay que encerrar todo el texto entre `""` ejemplo: `mkdir "3. Git & GitHub"`

### Comandos para eliminar Carpetas y Archivos

- `rmdir`: Este comando me permite eliminar carpetas que esten vacia o sin contenido. Ejemplo: `rmdir Emma`.

- `rm`: Este comando se usa para eliminar archivos. Ejemplo: `rm ejemplo.txt`.

- `rm -r`: Este comando se usa para eliminar carpetas y archivos. Ejemplo: `rm -r Ivan` o `rm -r katerin.txt`.

- `rm -rf`: Este comando se usa para forzar la eliminación de carpetas y archivos. Ejemplo: `rm -r Ivan` o `rm -r katerin.txt`.

### Comandos para mover Carpetas y Archivos

- (move) `mv` : Se escribe las palabras `mv` se da un espacio, se coloca el nombre del archivo, se da otro espacio y finalmente se coloca el nombre del archivo al cual se desea mover. Ejemplo: `mv guardame.txt guardar`.

### Comando para renombrar Archivos y carpetas

- (move) `mv` : Se escribe las palabras `mv` se da un espacio, se coloca el nombre del archivo, se da otro espacio y finalmente se coloca el nombre del archivo al cual se desea renombrar. Ejemplo: `mv guardame.txt guardardado.txt`. De esta manera el archivo cambio del nombre `guardame.txt a guardado.txt`. En el caso de las carpetas es similar, la diferencia es que no se coloca ninguna extensión para definir el tipo de carpeta, dado que estas no lo utilizan. Ejemplo: `mv Ivan Katerin`. El resultado es el cambio de nombre de la carpeta de `Ivan a Katerin`.

### Comando para copiar Archivos

- (copy) `cp` : Se escribe las palabras `cp` se da un espacio, se coloca el nombre del archivo, se da otro espacio y finalmente se coloca el nombre del archivo al cual se ha enviar la copia o en su defecto se colocar `../` si se desea copiar a la carpeta padre.  Ejemplo: `cp guardado.txt conservar` o `cp guardado.txt ../` De esta manera el archivo se copia a la ruta que se le especificó. Para copiar el archivo y cambiar el nombre se escribe el nuevo nombre despues de la barra invertida `cp guardado.txt ../guardadoExitoso`.

### Comando para copiar Carpetas

- (copy) `cp -r` : Para copiar carpetas se escriben las palabras `cp -r` se da un espacio, se escribe el nombre de la carpeta, se da otro espacio y finalmente se coloca el nombre de la carpeta a la cual se ha enviar la copia  del contenido en la carpeta (carpetas o archivos) o en su defecto se colocar `../` si se desea copiar dicho contenido a la carpeta padre. Ejemplo: `cp -r Ivan Katerin` o `cp -r Ivan ../` De esta manera el archivo se copia a la ruta que se le especificó. Tambien es posible crear una nueva carpeta a donde se va a copiar la carpeta objeto, `cp -r Ivan "aqui va el nombre de la nueva carpeta"`. Ejemplo: `cp -r Ivan "carpetaReceptora"`.

### Comando para buscar Archivos y Carpetas

- (buscar) `find`: Este comando permite realizar la busqueda de archivos. Se coloca la palabra `find` espacio el nombre del archivo con su extensión o el nombre de la carpeta. Ejemplo: `find ivan.txt` o `find carpeta` Es posible tambien utilizar el selector universal dentro de la carpeta raíz para buscar dicho elemento en todo el sistema. Se puede utilizar el nombre completo a la primera palabra. Ejemplo: `find *i`.

### Comando para listar procesos activos de mi computadora

- `ps`: Este comando lista los procesos activos de la computadora.

### Abrir IDES desde la Línea de Comandos

- `code`: Este comando nos permite abril nuestro IDE de dos formas. La primera es colocando la palabra `code .` Para esto debemos estar en Git Bash en la ubicación del archivo que deseamos abrir. La segunda es escribir el comando `code` y se copia la dirección de la carpeta que se desea abrir.

### Crear y eliminar comando alias

- `alias`: Este comando me permite visualizar todos los comandos `alias` que han sido creados por el ususario. Su objetivo es crear `alias` para facilitar la creación de archivos. Un ejemplo: alias `hi="touch hola.txt"` esto me permite crear un archivo `hola.txt` solo escribiendo la palabra `hi`. Para eliminar un `alias`, se usa el comando `unalias` más espacio y el nombre del `alias` que se desea eliminar. Un ejemplo: `unalias hi`. De esta manera se elimina el `alias` `hi`. Estos `alias` se usan mucho sobre todo para comando que son muy largos.
