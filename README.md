# EmacsCFG

Emacscfg es mi configuración personal para Emacs. La que utilizo diariamente. Es una recopilación de paquetes, configurados a mi gusto. El propósito es tener un backup de mi configuración en la nuve. Y si a alguien le gusta, que la aproveche.

## Instalación

* Clonar el repositorio en cualquier lugar de tu sistema.

	<pre>
	git clone --recursive https://github.com/francescarpi/emacscfg.git
	</pre>

* Activar configuración:

	<pre>
	ln -s ~/path-de-tu-emacscfg/emacs ~/.emacs
	ln -s ~/path-de-tu-emacscfg/paquetes ~/.emacs.d/
	</pre>


## Combinaciones de teclas

Combinaciones de teclas que más uso. Mi chuleta.

### Ventanas y buffers

| Combinación   | Descripción                                   |
| ------------- | --------------------------------------------- |
| C+x 0         | Cerrar la ventana actual                      |
| C+x 1         | Maximizar la ventana actual                   |
| C+x 2         | Dividir la ventana horizontalmente            |
| C+x 3         | Dividir la ventana verticalmente              |
| C+x o         | Ir a la ventana siguiente                     |
| C+x b         | Cambio de buffer por nombre                   |
| C+x C+b       | Se abre la ventana de buffers.                |
| C+x k         | Mata el buffer actual                         |
| C+x <right>   | Ir a buffer siguiente                         |
| C+x <left>    | Ir a buffer anterior                          |
| C+x x <right> | Ir a la ventana de la derecha (custom)        |
| C+x x <down>  | Ir a la ventana de abajo                      |
| C+x x <left>  | Ir a la ventana de la izquierda               |
| C+x x <up>    | Ir a la ventana de arriba                     |


### Ficheros

| Combinación   | Descripción                                   |
| ------------- | --------------------------------------------- |
| C+x C+f       | Abrir fichero                                 |
| C+x C+s       | Guardar fichero                               |

* Buscar ficheros en un directorio:
<pre>
A+x find-dired RET seleccionar carpeta padre RET -name "*.py" RET
</pre>
* Buscar dentro de una carpeta
<pre>
A+x helm-do-grep RET <seleccionar carpeta> C+u RET <indicar extensión ficheros> RET <indicar patron a buscar dentro de los ficheros>
</pre>

### Generales

| Combinación   | Descripción                                   |
| ------------- | --------------------------------------------- |
| C+x C+c       | Salir de Emacs                                |
| C+g           | Deshacer operación actual.                    |
| A+x ansi-term | Abrir un shell del sistema                    |
| A+x shell     | Abrir shell propio de emacs. Escrito en lisp  |
| A+!           | Ejecutar un comando en el shell               |
| C+x u         | Abrir árbol de undo                           |


### Navegación

| Combinación   | Descripción                                   |
| ------------- | --------------------------------------------- |
| C+l           | Centrar scroll vertical                       |
| C+k           | Borrar linea actual                           |
| C+a           | Ir al principio de una linea                  |
| C+e           | Ir al final de una linea                      |
| C+f           | Avanzar carácter                              |
| C+b           | Retroceder carácter                           |
| A+f           | Avanzar palabra                               |
| A+b           | Retroceder palabra                            |
| C+n           | Linea siguiente                               |
| C+p           | Linea anterior                                |
| C+v           | Página siguiente                              |
| A+v           | Página anterior                               |
| A+>           | Ir al final del documento                     |
| A+<           | Ir al principio del documento                 |
| A+w           | Copiar al portapapeles                        |
| C+y           | Pegar desde el portapapeles                   |
| C+w           | Cortar hacia el portapapeles                  |
| C+_           | Deshacer                                      |
| C+g C+_       | Rehacer                                       |
| C+s           | Buscar + buscar siguiente                     |
| C+r           | Buscar + buscar anterior                      |
| A+g A+g       | Ir a una linea concreta                       |
| C+c C+j       | Ir a una definición (clase, método, etc)      |
| C+d           | Borrar un carácter                            |
| A+0..9        | Seguido de un comando, lo ejecuta n veces     |
| A+a           | Saltar a definición interior                  |
| A+e           | Saltar a definición siguiente                 |
| A+m           | Saltar al principio de la identación          | 
| C-c n         | Modo multi cursor. Seleccionar siguiente      |
| C-c p         | Modo multi cursor. Seleccionar anterior       |
| C-c a         | Modo multi cursor. Seleccionar todos          |

### Rope

Combinaciones de teclas para Rope

| Combinación   | Descripción                                   |
| ------------- | --------------------------------------------- |
| C+c g         | Rope. Saltar definición dentro proyecto       |
| C+x p o       | Abrir un proyecto                             |
| C+x p k       | Cerrar un proyecto                            |
| C+x p f       | Buscar fichero en proyecto                    |
| C+x p c       | Abre fichero configuración del proyecto       |


### Selección

Relacionado con el modo visual, selección.

| Combinación   | Descripción                                   |
| ------------- | --------------------------------------------- |
| C+espacio     | Se activa modo visual                         |
| C+>           | Selección similar siguiente                   |
| C+<           | Selección similar anterior                    |
| C+c C+<       | Selección similar todas                       |
| Mayus+A+f     | Seleccionar una palabra                       |
| C+c >         | Identar la selección hacia la derecha         |
| C+c <         | Identar la selección hacia la izquierda       |
| Mayus+A+<der> | Tabular selección hacia la derecha            |
| Mayus+A+<izq> | Tabular selección hacia la izquierda          |
| C+c l         | Seleccionamos toda la linea                   |
| C+x h         | Seleccionamos todo el documento               |

### Registros

Los registros son un tema muy interesante. Podemos almacenar posiciones del cursor, bufers, etc, en un número de registro y luego volver a él.

Guardar registro: C+x r <espacio> <numero_registro>
Ir a registro: C+x rj <numero_registro>

### Html - Mode

| Combinación   | Descripción                                   |
| ------------- | --------------------------------------------- |
| C+c /         | Cierra un tag                                 |
| C+x TAB       | Oculta tags, dejando sólo cadenas             |
| C+c <left>    | Ir al principio del tag                       |
| C+c <right>   | Ir al final del tag                           |
| C+j           | Ejecuta Emmet                                 |

### Otros
| Combinación   | Descripción                                   |
| ------------- | --------------------------------------------- |
| C+c C+c m     | Renderiza en html el fichero Markdown.        |
| C+c C+c p     | Compila markdown y abre previsualización      |


### Dired Mode

Es una ventana de navegación de ficheros, donde podemos borrarlos, renombrarlos, etc. Al hacer **C+x C+f**, si tenemos seleccionada una carpeta, pulsar **C+d** para abrir dired-mode.

Acciones disponibles dentro del dm.

| Combinación   | Descripción                                   |
| ------------- | --------------------------------------------- |
| g             | Refrescar vista                               |
| s             | Cambiar ordenación entre fecha y nombre       |
| d             | Marcar un fichero para borrar                 |
| u             | Desmarcar un fichero marcado para borrar      |
| x             | Borrar ficheros marcados                      |
| o             | Abrir fichero en una ventana nueva            |
| R             | Renombrar fichero                             |
| Intro         | Abrir fichero en ventana actual               |
| +             | Crear un directorio                           |

Para crear un fichero en dired mode, se puede hacer ejecutando un comando de shell: **A+!** + **touch <nombrefichero>**. Luego un **g** en el dired mode para refrescar la ventana

### Helm Find File Mode

Cuando estamos en la navegación de ficheros que se dispara mediante C+x C+f

| Combinación   | Descripción                                   |
| ------------- | --------------------------------------------- |
| C+s           | Grep recursivo                                |
| A+e           | Salta al Eshell                               |
| A+i           | Abre un tooltip con información del fichero   |
| C+c /         | Find a partir de la carpeta donde estés       |
| A+p           | Historial de directorios recientes            |
| C+c h         | Historial archivos recientes                  |

Para configurar helm, ejecutar **helm-configuration**. Allí podemos modificar la recursividad del comando helm-grep, entre muchas otras cosas.

### Buffer mode

Cuando estamos en la ventana de gestión de buffers

| Combinación   | Descripción                                   |
| ------------- | --------------------------------------------- |
| A+<espacio>   | Marcar                                        |
| A+D           | Kill buffers marcados                         |

### Mu4e

Cliente de correo integrado en emacs

| Combinación   | Descripción                                   |
| ------------- | --------------------------------------------- |
| C             | Redactar un correo                            |
| j             | Saltar a una carpeta                          |
| m             | Mover email                                   |
| D             | Marcar mensaje para borrar                    |
| A             | Acciones sobre attachtment                    |
| a             | Otras acciones, como ver en PDF               |
| e             | Guardar un attachtment                        |
| t             | Menú con opciones para marcar el mensaje      |
| C+c C+u       | Sincronizar imap                              |
| R             | Responder correo                              |
| C+u e         | Más opciones para descargar adjuntos          |



### Snippets

A parte de los snippets que ya llevan los paquetes instalados, he añadido algunos nuevos que detallo a continuación:

**html-mode**

| Disparador | Descripción                                                                   |
| ---------- | ----------------------------------------------------------------------------- |
| block      | Bloque de django {% block <nombre> %}{% endblock %}                           |
| trans      | Traducción {% trans "" %}                                                     |
| url        | Reverse de url {% url "" %}                                                   |
| ext        | Añade un {% extnds "" %}                                                      |
| inc        | Añade un {% include "" %}                                                     |

**js-mode**

| Disparador | Descripción                                                                   |
| ---------- | ----------------------------------------------------------------------------- |
| jqplug     | Estructura básica de un plugin jQuery, vacío. Para empezar a trabajarlo       |
| log        | Añade un console.log()                                                        |

**python-mode**

| Disparador | Descripción                                                                   |
| ---------- | ----------------------------------------------------------------------------- |
| cm         | Bloque de comentario multilinea, para el docstring de una clase nueva         |
| sbu        | Coloca el intérprete de python y la codificación utf-8 al inicio del doc      |
| mchar      | Model CharField.                                                              |
| mfor       | Model ForeignKey                                                              |
| mmany      | Model ManyToManyField                                                         |
| mfloat     | Model FloatField                                                              |
| mint       | Model PositiveIntegerField                                                    |
| metao      | Class Meta con un ordering                                                    |
| verbb      | Bloque de verbose_name y verbose_name_plural                                  |

## Acciones, funciones personalizadas

* **Alt+x cdsitepackages**: Nos permite escoger un entorno virtual y abre helm-find-files situado en la carpeta del site-packages.
* **Alt+x cdvirtualenv**: Lo mismo, pero se situa en la raíz del entorno virtual.

## Pendiente a resolver

Listado de puntos pendientes de investigar y mejorar

* En el listado de buffers, si los ficheros abiertos tienen paths muy largos, no veo en que carpeta están...
