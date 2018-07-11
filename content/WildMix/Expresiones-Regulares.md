# Expresiones Regulares

Las expresiones regulares intentan solucionar problemas del d�a a d�a. Se intenta buscar la forma en que ciertos datos son presentados, por ejemplo un n�mero de tel�fono dependiendo de pa�s y zona, tiene determinada cantidad de n�meros, a veces separados con guiones o puntos, pero la estructura siempre es la misma

Otro ejemplo de uso de expresiones regulares ser�a intentar cambiar en un _.csv_ los precios de modo europeo a modo americano

Un d�gito se puede expresar con ``/d``

Caracter de palabra: ``/w``

**Cadena de Caracteres**: Es un car�cter _ASCII_ generalmente, seguido de otro car�cter y de otro. No todos son visibles, el espacio por ejemplo. Cada car�cter es un car�cter.

## El caracter (.)

Encuentra todo lo que sea un car�cter, coincide con cualquier car�cter excepto fin de linea.

## Las clases predefinidas y constru�das

Las b�squedas en las expresiones regulares funcionan en m�ltiplos de la cantidad de caracteres que expl�citamente indicamos

**D�gitos:**

Encuentra todos los d�gitos de 0 a 9.
    
``\d`` es equivalente a poner [0-9].
    
Si en vez de ``\d``, usamos por ejemplo ``[0-2]`` nos encontrar� solamente los d�gitos de 0 a 2.

Podemos usar ``\D`` para encontrar justo lo contrario, todo lo que no son d�gitos.

**Palabras:**

Encuentra todo lo que puede ser parte de una palabra, tanto letras (min�sculas o may�sculas) como n�meros.

``\w`` es equivalente a poner ``[a-zA-Z0-9_]``.

Si en vez de ``\w``, usamos por ejemplo ``[a-zA-Z]`` nos encontrar� solamente las letras.

Podemos usar ``\W`` para encontrar justo lo contrario, todos los caracteres que no son parte de palabras.

**Espacios:**

``\s`` encuentra todos los espacios (los saltos de l�nea tambi�n son espacios).

Podemos usar ``\S`` para encontrar justo lo contrario, todo lo que no son espacios.

## Los delimitadores: \+, \*, ?

``*`` Cero o muchos

``+`` Uno o muchos

``?`` Cero o uno

Ejemplos:

- ``\d+[a-z]``  Encuentra todo lo que tenga uno o m�s d�gitos y al final tiene una letra.

- ``\d*[a-z]``  Encuentra todo lo que teniendo d�gitos o no, al final tiene una letra.

## Los Contadores {n,m}

Donde ``n`` y ``m`` son enteros positivos y ``n <= m``. Coincide con al menos ``n`` y no m�s de ``m`` ocurrencias de la expresi�n. Si se omite ``m``, no tiene limite de m�ximo.

Por ejemplo, ``/a{1,3}/`` no coincide con "**cndy**", pero s� con la '**a**'' en "**candy**", las primeras 2 a en "**caandy**" y las primeras 3 a en "**caaaaaaandy**". Note que en "**caaaaaaandy**", la coincidencia es "**aaa**", aunque la cadena contenga m�s a en ella.

## El caso de (?) como delimitador

Busca el car�cter precedente 0 (cero) o 1 (una) vez. Es equivalente a ``{0,1}``.

Por ejemplo, la expresi�n ``/e?le?/`` encontrar� la subcadena '**el**' en la cadena "**angel**" y la subcadena '**le**' en la cadena "**abominable**" y tambi�n el car�cter '**l**' en la cadena "**muslo**".

Si se utiliza inmediatamente despu�s que cualquiera de los cuantificadores ``*, +, ?, o {}``, hace que el cuantificador no sea expansivo _(encontrando la menor cantidad posible de caracteres), en comparaci�n con el valor predeterminado, que s� es expansivo (encontrando tantos caracteres como le sea posible)_. Por ejemplo, aplicando la expresi�n ``/\d+/`` a la cadena "123abc" encuentra "123". Pero aplicando la expresi�n ``/\d+?/`` a la misma cadena, encuentra solamente el car�cter "**1**".

Tambi�n se utiliza en coincidencias previsivas.

## Principio (^) y final de linea ($)

``^`` Coincide con el comienzo de la cadena, o el comienzo de una l�nea si la bandera multil�nea **(m)** est� habilitada

``$`` Coincide con el final de la cadena, o al final de una l�nea si la bandera multil�nea **(m)** est� habilitada


---

## Enlaces de inter�s

+ [Leer, construir y testear expresiones regulares](https://regexr.com/)

+ [Testear online expresiones regulares](https://regex101.com/)

+ [Expresiones regulares https://developer.mozilla.org](https://developer.mozilla.org/es/docs/Web/JavaScript/Guide/Regular_Expressions)