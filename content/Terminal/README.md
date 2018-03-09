# Introducci�n a la Terminal

Comandos b�sicos para terminales UNIX.

## Navegaci�n entre directorios y listado de archivos

+ **``pwd``** Muestra la ubicaci�n, la ruta del directorio donde se encuentra posicionado.

+ **``~``** Es la "Home" del usuario. _Ejm_: /home/wilder

+ **``/``** Es la "Raiz" del Sistema Operativo

+ **``ls``** Lista los archivos o carpetas (del directorio donde se encuentra al momento de ejecutar el comando)
    
    + **``-l``** Esta bandera lista los archivos de un directorio como una lista y muestra algunos detalles importantes, como por ejemplo: Tipo de archivo (d, -, l), permisos, propietario, tama�o, fechas de creaci�n, etc.

    + **``-t``** Esta nos ordena los archivos desde los m�s recientes hasta los m�s viejos (seg�n su fecha de creaci�n).

    + **``-r``** Esta bandera revierte las funciones de las banderas anteriores, por ejemplo: -ltr listar�a los archivos y directorios desde el m�s antiguo al m�s reciente.

    + **``-h``** Esta bandera ("legible humanamente") nos muestra el tama�o de los archivos en Bites, Kilobytes, Megabytes, etc.


    + **``-S``** Esta bandera ordena los archivos y/o directorios desde el m�s pesado al menos pesado, un buen uso ser�a: **``-lhS``** de esta forma estar�as listando, mostrando el tama�o de una forma legible (para un humano) y ordenandolos.


+ **``cd``** Nos ayuda a movernos entre directorios, con ``TAB`` podemos ver los archivos o directorios existentes (en la ubicaci�n).

+ **``du -h``** Muestra el peso total de los directorios.

>_Nota: Las banderas se pueden concatenar (no en todos los comandos funcionan) escribiendo desp�es del gui�n (-) las banderas, por ejemplo: **``-lt``**_


## Creaci�n de directorios, mover, copiar, y renombrar archivos

+ **``mkdir``** Crea un nuevo directorio.

+ **``touch``** Abre el archivo y lo cierra, tambi�n con este comando se puede crear un archivo (incluso hasta se le puede a�adir la extensi�n), por ejemplo: touch index.html

+ **``mv``** Mueve un archivo o un directorio. _Ejm_: **``mv ../photo.jpg /.``**

+ **``cp``** Copia un archivo o un directorio. _Ejm_: **``cp ./photo.jpg ../``**

>_Nota: Colocar un * (asterisco) seguido de una extensi�n nos ayuda a ejecutar un comando a todos los archivos con esa extensi�n, puede ser, moverlos, copiarlos, borrarlos, etc._



