# Algoritmos con C

## Lenguajes de programaci�n
Hay dos tipos de lenguajes de programaci�n que hoy en d�a ya son poco usados:

**Lenguaje de m�quina:** Codigo binario o hexadecimal directamente interpretados por el microprocesador de el computador dif�ciles de leer para una persona.

**Lenguaje ensamblador:** Utiliza instrucciones que son espec�ficas del CPU y que tienen una traducci�n directa al Hardware que lo compone.

Los lenguajes de programaci�n que actualmente son los que se utilizan son:

**Lenguaje de bajo nivel:** Va a ser un lenguaje que est� muy cerca de lo que se interpreta directamente en el computador.

**Lenguaje de alto nivel:** Son con los que estamos programando cosas como la Web, grandes aplicaciones, etc.

**Notas:**

- Las computadoras trabajan con 0 y 1, donde los transistores pueden tener diferentes estados por ser materiales semi conductores. Esto es utilizado por medio de electr�nica para que los circuitos combinen y puedan funcionar haciendo operaciones.

- Si tratamos de ver desde el procesador las operaciones que se ejecutan en la computadora, ser�a nada comprensible, tendr�amos que hacer una serie de c�digos binarios y hexadecimales (lenguaje m�quina) que hoy en d�a ya nadie hace.

- El lenguaje ensamblador lo proporciona el fabricante del microcontrolador.

- El chip de un Arduino se puede programar todav�a con un ensamblador.

- Entre m�s bajo se el nivel de un lenguaje de programaci�n, m�s directo va a ser para trabajar con el Hardware.

- Los lenguajes de alto nivel permiten a los programadores tener una interacci�n mucho m�s f�cil con equipos, son lenguajes que son mucho m�s parecidos al ingl�s.

- Los lenguajes de alto nivel est�n muy alejados del Hardware, por lo que casi siempre van a contar con un int�rprete que se va a encargar de traducirlo al lenguaje ensamblador o al c�digo m�quina, que va a ser el c�digo final que se va a ejecutar en nuestros equipos.

- Existen lenguajes de programaci�n que no son tipados, es decir, no van a tener ning�n tipo de dato dentro de su estructura.

- Lo que sucede con un lenguaje de programaci�n que no tiene tipo de datos es que no va a ser tan f�cil optimizar el uso de recursos.

## Algoritmo
Un algoritmo es un conjunto de instrucciones finitas que nos permiten resolver un problema dado paso a paso y sin generar ambig�edades.

## User defined data types: Estructuras de datos y custom data types
En algunas ocasiones, cuando estamos programando, no nos basta con los tipos de datos definidos por el lenguaje previamente, para esto podemos ir definiendo nosotros un tipo de dato propio que vayamos a estar usando en nuestro proyecto.

**Ejemplo:** En el lenguaje de programaci�n de ``Java``, esto se conoce como clases. As� mismo en el lenguaje de ``C++`` o ``C`` se conoce como estructuras.

### Razones por las que podemos crear nuestro propio tipo de dato:
Se tiene mucha m�s flexibilidad en el proyecto.
Permite tener un mejor uso de memoria, porque estamos definiendo al programa una serie de pasos en los que no va a tener que procesar nada.

### �Qu� son las estructuras de datos?
Las estructuras de datos son una manera eficiente de organizar y almacenar la informaci�n que estamos recibiendo.

### Estructuras de datos comunes:
+ Listas
+ Arreglos
+ Listas ordenadas
+ �rboles

**Tipos de datos abstractos:** Tipo de datos definido por el usuario con un operador que se va a utilizar en aplicaciones.

## Estructuras de control y estructuras de control secuenciales
Nos van a permitir definir el flujo de nuestro programa, ejecutar acciones en la parte del proceso correcta.

### Tipos de Estructuras de Control:

+ **Estructuras Secuenciales:** Son las m�s b�sicas, funciona como su nombre lo dice, en secuencia. El programa ejecuta los pasos ordenadamente uno tras otro hasta obtener el resultado y termina.

+ **Estructuras de control selectivas:** Nos van a permitir que nuestro algoritmo o el programa tome decisiones en el caso de ejecutar un pedazo de c�digo o un segmento de c�digo o no con base en una condici�n espec�fica que debemos verificar si se cumple, y si se cumple ejecutamos la condici�n y si no, se va colocando lo siguiente de nuestro c�digo.

    + Si, **if**. Aqu� vamos a tener una condici�n, y en caso de que la condici�n se cumpla vamos a ejecutar un pedazo de c�digo. En caso de que la condici�n no se cumpla vamos a saltar ese pedazo de c�digo.

    + Si - sino, **if - else**. Nos permite una condici�n y bifurcar el camino para dos rutas distintas, es decir, si la condici�n se cumple, ejecutamos una acci�n y si la condici�n no se cumple ejecutamos otra acci�n diferente.

    + Si, sino entonces� sino, **if, else if, else**. Aqu� vamos a poder verificar la primera condici�n, en caso de que esta primera no se cumpla, podemos verificar una segunda condici�n y en caso de que esta segunda no se cumpla, podemos tener _n_ condiciones. Si este n�mero _n_ que hayamos determinado no se cumplen, al final se ejecutar� else (sino).

+ **Estructuras de control repetitivas:** Est�s nos van a permitir crear bucles donde nuestros programas va a estar repiti�ndose hasta que una condici�n les indique lo contrario o mientras una condici�n les indique que hagamos eso.

    + Mientras, **while**. Mientras una condici�n se cumpla, nosotros vamos a ejecutar todo el c�digo que est� dentro de este ciclo y vamos a repetirlo.

    + Haz mientras, **do while**. Esta instrucci�n nos permite entrar por lo menos una vez a ejecutar el c�digo que est� dentro de esta instrucci�n y si la condici�n se cumple , entonces repetimos, pero si la condici�n no se cumple salimos del c�digo.

    + Para, **for**. Se utiliza cuando necesitamos repetir una serie de veces definida un c�digo.

## C�mo comparar algoritmos y ritmo de crecimiento
Debemos saber que existen buenas y malas m�tricas para comparar algoritmos.

**Malas m�tricas:**

+ **Tiempo de ejecuci�n:** El tiempo de ejecuci�n va a variar dependiendo del equipo donde se ejecute el algoritmo.
+ **N�mero de instrucciones ejecutadas:** Una vez tenemos un algoritmo hecho, debemos llevarlo a un lenguaje de programaci�n, lo que significa que va a depender del lenguaje que estemos, el n�mero de l�neas de c�digo (instrucciones) que vamos a utilizar.

_**Para hacer un an�lisis del ritmo de crecimiento, siempre vamos a tomar el t�rmino de mayor peso.**_

---

## Enlaces de inter�s

+ [Documentaci�n de C](https://devdocs.io/c/)

