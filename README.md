**TUTORIAL BÁSICO PARA GITHUB**

Antes de seguir este tutorial es necesario que conozcas la funcionalidad
básica de GIT.

1.  Primero debemos registrarnos en la página principal de Github.com

> ![](.//media/image1.png){width="2.8956528871391076in"
> height="2.530975503062117in"}

2.  Ahora nos ubicamos en la parte izquierda superior de la pagina
    principal y señalamos New

> ![](.//media/image2.png){width="2.9583333333333335in"
> height="1.0625in"}

3.  En la nueva página podemos llenar los campos de la siguiente manera:

    1.  Comenzamos dándole un nombre único a nuestro proyecto. Podemos
        añadir también una descripción de lo que trata.

> ![](.//media/image3.png){width="4.765765529308837in"
> height="1.3871784776902887in"}

2.  El repositorio tendrá por defecto marcado la casilla de público, es
    decir que cualquier miembro de Github podrá ver tu código. Si la
    casilla privada es marcada solo podrá ser visto por las personas que
    tu elijas.

> ![](.//media/image4.png){width="3.3913035870516186in"
> height="0.9851345144356956in"}

3.  En la parte inferior podemos elegir si queremos que el proyecto se
    cree con un README, esta opción esta desmarcada por defecto y así la
    dejaremos debido a que si la seleccionamos se hará un commit inicial
    automáticamente y podemos tener problemas en nuestro primer push. Es
    una buena práctica agregar un README para describir de mejor manera
    al proyecto, explicar las tecnologías contenidas, el uso, etc. No lo
    creamos desde el inicio pero podemos agregarlo después con la
    extensión de archivo .md.

> ![](.//media/image5.png){width="3.6770833333333335in"
> height="0.7604166666666666in"}

4.  También puedes elegir si agregar un archivo .gitignore y una
    licencia para tu proyecto. Finalmente creamos el repositorio.

> ![](.//media/image6.png){width="3.4479166666666665in"
> height="1.1458333333333333in"}
>
> Para más información de las licencias puedes visitar el siguiente
> link:
> [https://help.Github.com/es/Github/creating-cloning-and-archiving-repositories/licensing-a-repository](https://help.github.com/es/github/creating-cloning-and-archiving-repositories/licensing-a-repository)

5.  Después de crear el repositorio se nos mostrará una página con los
    pasos a seguir para subir el repositorio a Github.

> ![](.//media/image7.png){width="5.342342519685039in"
> height="2.823827646544182in"}

6.  Si agregamos el archivo README en el momento de la creación del
    repositorio, automáticamente nos lo detectará como un commit en el
    proyecto y la página se verá de esta manera:

![](.//media/image8.png){width="5.378378171478565in"
height="3.0939588801399824in"}

4.  Ahora para llevar el proyecto desde el repositorio en git de mi
    computador, hacia el Github debo hacer los siguientes pasos:

    1.  Abro el git bash en la carpeta del proyecto.

> ![](.//media/image9.png){width="5.396396544181977in"
> height="2.908674540682415in"}

2.  Creo el repositorio con el comando git init

> ![](.//media/image10.png){width="5.315314960629921in"
> height="0.993517060367454in"}

3.  Agrego los documentos al staging area mediante el comando git add .

> ![](.//media/image11.png){width="0.8958333333333334in"
> height="0.40625in"}

4.  Realizo el primer git commit del proyecto

> ![](.//media/image12.png){width="5.351351706036746in"
> height="0.8425984251968504in"}

5.  Añadimos el origen de nuestro proyecto mediante el comando git
    remote add origin \[UrldelRepositorio.git\]

> ![](.//media/image13.png){width="5.324324146981628in"
> height="0.3380916447944007in"}

6.  Por ultimo haremos un git push -u origin master

> ![](.//media/image14.png){width="5.291274059492563in"
> height="1.9909908136482939in"}

La primera vez nos pedirá que nos autentiquemos en el Github.

![](.//media/image15.png){width="2.9996620734908137in"
height="2.9692552493438322in"}

1.  Si creamos el README desde el principio no se hará el push
    normalmente debido a que en el repositorio de Github hay un archivo
    que en el repositorio local no. Para solucionar eso tenemos que
    hacer un git pull origin master \--allow-unrelated-histories, esto
    traerá el README de Github al computador, después continuamos desde
    el paso 4.3.

```{=html}
<!-- -->
```
7.  Finalmente ya podremos ver el repositorio de Github con los archivos
    agregados.

> ![](.//media/image16.png){width="5.304347112860892in"
> height="2.0951662292213475in"}

5.  Si quiero tener los archivos de mi repositorio Github en otro
    computador, puedo clonar el repositorio. Se lo puede hacer de dos
    maneras:

    1.  Descargándolo desde la página web de Github

> ![](.//media/image17.png){width="3.3541666666666665in"
> height="1.84375in"}

2.  Desde la terminal haciendo un git clone \[url\] ubicándonos dentro
    de la carpeta destino de los archivos

> ![](.//media/image18.png){width="5.342342519685039in"
> height="1.2786942257217848in"}
>
> ![](.//media/image19.png){width="5.315314960629921in"
> height="0.8494247594050743in"}
>
> ![](.//media/image20.png){width="5.270270122484689in"
> height="1.9687795275590552in"}

3.  Puedo realizar cualquier cambio y subirlo al repositorio
    normalmente.

-   A modo de ejemplo creamos el archivo git clone

> ![](.//media/image21.png){width="3.9479166666666665in"
> height="1.625in"}

-   Ingresamos a la carpeta del repositorio, verificamos el estado del
    repositorio y observamos que el nuevo archivo está en rojo debido a
    que no está añadido al repositorio local.

> ![](.//media/image22.png){width="5.081080489938758in"
> height="1.668251312335958in"}

-   Añadimos el nuevo archivo al repositorio

> ![](.//media/image23.png){width="4.081081583552056in"
> height="1.3842268153980752in"}

-   Realizamos un push al repositorio del Github.

> ![](.//media/image24.png){width="2.063063210848644in"
> height="0.3557010061242345in"}

-   Finalmente ya podemos observar los cambios en el repositorio del
    Github.

> ![](.//media/image25.png){width="5.063063210848644in"
> height="2.3128762029746284in"}

6.  La interfaz de Github es muy grande y completa, pero los elementos
    básicos que debes conocer son los siguientes:

-   En la parte derecha de la interfaz encontramos 4 botones.

![](.//media/image26.png){width="3.8541666666666665in"
height="0.3541666666666667in"}

-   Crear un nuevo archivo, el cual no es muy usado debido a que los
    archivos deben crearse o modificarse desde el ordenador, pero si se
    hace uso de este botón se creará un archivo en blanco al cual
    podemos también añadirle contenido y también hacerle un commit
    debido a que es un cambio.

> ![](.//media/image27.png){width="3.5826093613298338in"
> height="1.1852909011373578in"}
>
> ![](.//media/image28.png){width="4.457898075240595in"
> height="2.0695647419072616in"}

-   Cargar archivos te permite pasar archivos desde el pc al repositorio
    de Github con el respectivo commit.

> ![](.//media/image29.png){width="4.783783902012249in"
> height="1.4040835520559931in"}
>
> ![](.//media/image30.png){width="4.7340277777777775in"
> height="2.407652012248469in"}

-   El botón encontrar archivos te presenta el árbol de directorios de
    todos los archivos contenidos en el proyecto, así mismo implementa
    un buscador para encontrar archivos específicos.

> ![](.//media/image31.png){width="2.423423009623797in"
> height="2.6758639545056866in"}![](.//media/image32.png){width="2.4467377515310584in"
> height="2.386075021872266in"}

-   En la parte izquierda de la interfáz encontramos los botones para
    mostrar las ramas de nuestro proyecto y la solicitud de pull
    request. El primer boton es útil cuando manejamos 2 o más ramas de
    nuestro proyecto.

> Cuando queremos modificar un proyecto que no es nuestro podemos hacer
> un fork para traer una copia de su repositorio al nuestro y una vez
> terminadas nuestras implemetaciones podemos solicitar al dueño del
> repositorio original que añada nuestros cambios a su repositorio, esta
> solicitud se la hace a través de un pull request el cual será revisado
> por el autor y aprobado o declinado dependiendo de su criterio.

![](.//media/image33.png){width="2.34375in"
height="0.3541666666666667in"}

-   Cuando seleccionamos un archivo dentro del Github, se nos presentan
    estas tres opciones:

![](.//media/image34.png){width="2.6458333333333335in"
height="0.34375in"}

-   Raw abre el contenido del documento seleccionado.

> ![](.//media/image35.png){width="3.6354166666666665in"
> height="0.875in"}

-   Blame muestra los cambios del archivo a través del tiempo con los
    respectivos commits.

> ![](.//media/image36.png){width="4.875351049868766in"
> height="0.6936931321084865in"}

-   History muestra mas a detalle los commits realizados, por ejemplo si
    voy a mi primer commit, cuando no tenía agregado el archivo readme,
    este no me aparecerá en mi rama principal debido a que hasta ese
    entonces no existía.

> ![](.//media/image37.png){width="4.873873578302712in"
> height="1.2895363079615048in"}
>
> ![](.//media/image38.png){width="4.342342519685039in"
> height="2.145425415573053in"}
>
> Para salir de este commit basta con seleccionar master dentro del
> botón que muestra las ramas.
>
> ![](.//media/image39.png){width="2.71875in" height="1.71875in"}
>
> ![](.//media/image40.png){width="4.855856299212598in"
> height="2.6010170603674543in"}

7.  Si por cualquier motivo se realizó un cambio en el repositorio de
    Github y quieres que se vea reflejado en el repositorio local, es
    necesario hacer un git pull, este comando traerá los cambios de
    Github al computador.

-   A modo de ejemplo cambiaremos el archivo gitclone.txt y lo
    cambiaremos por un archivo README.md desde el repositorio en Github.

![](.//media/image41.png){width="2.6666666666666665in"
height="0.5833333333333334in"}

![](.//media/image42.png){width="4.513513779527559in"
height="1.354054024496938in"}

-   Llenamos los datos del nuevo commit, ya que es un cambio que debe
    estar registrado.

![](.//media/image43.png){width="5.369368985126859in"
height="2.6891043307086613in"}

-   Una vez realizados los cambios podemos ver ya los archivos
    actualizados en nuestra rama master.

![](.//media/image44.png){width="4.918918416447944in"
height="3.266240157480315in"}

-   Estos cambios fueron realizados desde Github, pero el repositorio
    local de la computadora no refleja automáticamente estos cambios. Es
    aquí cuando el comando git pull nos ayuda a traer estos nuevos
    cambios desde Github hacia el repositorio local.

![](.//media/image45.png){width="4.216216097987751in"
height="1.9155643044619421in"}

![](.//media/image46.png){width="1.1458333333333333in"
height="1.65625in"}![](.//media/image47.png){width="1.1145833333333333in"
height="1.3333333333333333in"}

8.  En el tutorial de git vimos como gestionar las ramas de manera
    local, pero ahora veremos como crearlas y eliminarlas desde nuestro
    Github. Podemos crear las ramas de dos maneras: La primera creando
    la rama desde el git local y luego hacer un push al Github y la
    segunda creando la rama desde el Github y haciendo un pull hacia el
    repositorio local.

-   En el primer ejemplo crearemos una nueva rama desde el git local y
    la trasladaremos al Github.

    -   Añadimos la nueva rama.

> ![](.//media/image48.png){width="2.46875in"
> height="0.5104166666666666in"}

-   Realizamos un cambio en la rama, en este caso modificaré el archivo
    funciones.js.

> ![](.//media/image49.png){width="2.109027777777778in"
> height="2.3958333333333335in"}![](.//media/image50.png){width="2.017361111111111in"
> height="2.364922353455818in"}

-   Guardamos y lo agregamos al repositorio local.

> ![](.//media/image51.png){width="4.8468471128608925in"
> height="0.9618252405949256in"}

-   Hacemos un push pero en vez de hacerlo al origen master lo hacemos
    con el nombre de la rama. Esto creará automáticamente la rama dentro
    de Github con los cambios correspondientes.

> ![](.//media/image52.png){width="4.860352143482065in"
> height="0.35135061242344706in"}
>
> Gihub:
>
> ![](.//media/image53.png){width="1.8541666666666667in"
> height="0.4583333333333333in"}
>
> ![](.//media/image54.png){width="2.84375in" height="2.0625in"}
>
> ![](.//media/image55.png){width="4.215972222222222in"
> height="0.3094291338582677in"}
>
> ![](.//media/image56.png){width="2.1875in" height="3.09375in"}

-   Ahora para unir las ramas, nos dirigimos al repositorio local, y
    haremos un git merge \[Rama\] desde master y realizamos un git push
    -u origin master.

> ![](.//media/image57.png){width="4.945945975503062in"
> height="2.2191830708661415in"}
>
> Github:
>
> ![](.//media/image58.png){width="4.980803805774278in"
> height="0.42342300962379703in"}
>
> ![](.//media/image59.png){width="2.21875in" height="3.03125in"}

-   Finalmente si ya no necesitamos las ramas y queremos borrarlas,
    debemos hacerlo tanto del repositorio local como del Github, pero
    por separado ya que quitar la rama del git local no significa que la
    rama del Github haya sido eliminada.

> ![](.//media/image60.png){width="3.8288287401574803in"
> height="0.6711887576552931in"}
>
> ![](.//media/image61.png){width="3.8541666666666665in"
> height="2.1145833333333335in"}
>
> ![](.//media/image62.png){width="4.882882764654418in"
> height="1.7202624671916011in"}

-   En el segundo ejemplo crearemos la rama desde el Github y su
    contenido la trasladaremos al git local.

    -   Nos ubicaremos en el Github en el botón de despliegue de la
        ramas y en el buscador digitamos el nombre de la nueva rama.

> ![](.//media/image63.png){width="2.6486482939632547in"
> height="1.6186187664041995in"}

-   Automáticamente se creará la nueva rama con todo el contenido de la
    rama master.

> ![](.//media/image64.png){width="4.117117235345582in"
> height="2.5941174540682415in"}

-   Para traer el contenido de esta rama al repositorio local, abrimos
    el git bash en la rama master y creamos una nueva rama con el mismo
    nombre. Es importante que tenga el mismo nombre debido a que si en
    un futuro hacemos push a la rama dará conflictos.

> ![](.//media/image65.png){width="2.6415168416447945in"
> height="0.5585586176727909in"}

-   Si por error creaste la rama con otro nombre, puedes modificarlo
    desde la misma rama mediante el comando git branch -m
    \[NuevoNombre\]

```{=html}
<!-- -->
```
-   Si tenemos una modificación en el Github y queremos traer los
    cambios a la rama local, usamos el git pull origin \[Rama\]

    -   Para ejemplificar este caso, llenaremos el archivo readme de la
        nueva rama con nueva información. Y hacemos el commit.

> ![](.//media/image66.png){width="4.387387357830272in"
> height="2.112694663167104in"}
>
> ![](.//media/image67.png){width="4.3603597987751535in"
> height="2.195049212598425in"}

-   Para traer estos cambios al repositorio local, podemos hacer un git
    pull origin \[Rama\]

> ![](.//media/image68.png){width="4.2972965879265095in"
> height="1.8345767716535433in"}

-   Ya que puedo visualizar los cambios desde mi repositorio local, lo
    puedo agregar a la rama master haciendo un git merge para unirlo en
    el repositorio local y un git push origin master para subirlo al
    Github.

> ![](.//media/image69.png){width="2.6041666666666665in"
> height="1.9791666666666667in"}

-   Ahora ya tengo el commit de la rama caso2 en mi rama master tanto
    del repositorio local como del Github.

> ![](.//media/image70.png){width="4.387387357830272in"
> height="1.1887390638670166in"}
>
> ![](.//media/image71.png){width="4.333333333333333in"
> height="2.3707403762029746in"}
