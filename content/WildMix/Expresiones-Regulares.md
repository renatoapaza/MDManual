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
