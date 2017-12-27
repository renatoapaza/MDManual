# Introducci�n al Lenguaje C

**Notas:**

+ El lenguaje ``C`` fue una revoluci�n en su �poca ya que en ese entonces se utilizaba todav�a el lenguaje ensamblador para acceder al lenguaje m�quina o para trabajar directamente con el hardware.

+ Lo incre�ble de este lenguaje era que ten�a la capacidad de trabajar a nivel hardware y adem�s estaba optimizado pues era un lenguaje de alto nivel.

+ El lenguaje es hoy en d�a todav�a el lenguaje de programaci�n m�s utilizado en sistemas embebidos y en sistemas de bajos recursos de hardware donde necesitamos el acceso al hardware y donde se necesita tener muy alto rendimiento.

+ El lenguaje ``C`` tard� varios a�os en estandarizarse.

+ Un est�ndar en ``C`` significa una serie de gu�as y directivas que se deben de seguir al momento de escribir tu c�digo que est�n respaldadas por una asociaci�n (ANSI).

+ La programaci�n estructurada es un m�todo de programaci�n o un paradigma que dice que vamos a ejecutar el c�digo de forma secuencial, l�nea tras l�nea, del inicio al fin.

+ ``C`` es un lenguaje de programaci�n compilado.

+ ``C`` es un lenguaje tipado.


## Caracter�sticas importantes de C
+ N�cleo del lenguaje simple que opera con bibliotecas.

+ Lenguaje flexible que soporta la programaci�n.

+ Acceso a memoria de bajo nivel con punteros.

+ Utiliza un conjunto reducido de palabras clave.

+ Pasaje de par�metros por valor y referencia.

## Tipos de errores y datos en C
Existen 4 tipos principales de errores en C:

+ **Sint�cticos:** Todo lenguaje tiene una estructura definida de instrucciones que vamos a utilizar para indicarle al programa lo que nosotros queremos hacer. Estos errores son cuando escribimos mal en el c�digo estas instrucciones ya definidas.

+ **En el enlace:** Cuando enlazamos las librer�as con nuestro c�digo inicial, puede ocurrir que invoquemos mal una funci�n o no insertemos la librer�a que necesit�bamos, esto a la hora de compilar nos va a arrojar un error.

+ **De ejecuci�n:** Este sucede cuando por alguna raz�n, mientras el programa est� corriendo, alguno de los valores que vamos a utilizar en una variable, genera que haya una operaci�n inv�lida.

+ **Sem�nticos:** Es mucho m�s complicado detectarlos, ya que son los errores que tenemos cuando nuestros programa funciona bien, se ejecuta bien, corre sin problemas t�cnicos pero no est� teniendo el resultado que nosotros est�bamos esperando y la soluci�n no est� bien implementada.


## Identificadores
Es el nombre que identifica una constante, variable o funci�n.

Reglas para los identificadores:

+ Longitud ilimitada, pero se recomienda usar nombres descriptivos pero cortos.

+ Deben comenzar con una letra o gui�n bajo.

+ No se puede usar n�meros.

+ No se puede usar caracteres especiales.

+ Deben ser �nicos en el programa.

+ �nfasis en la diferencia entre may�sculas y min�sculas.

+ No puede coincidir con una palabra reservada del lenguaje o con una funci�n de biblioteca.


## Tipos de datos en C
+ **char** Caracter

+ **int** N�mero entero

+ **float** N�mero real de precisi�n simple

+ **double** N�mero real de precisi�n doble


## Variables en C
Las variables son una posici�n de memoria donde se almacena un dato.

Hay dos cosas que se deben definir en una variable:

**Nombre:** Esto nos sirve para poder recuperar su valor en cualquier parte del programa que estemos desarrollando.

**Tipo:** Es el l�mite que le damos de almacenamiento de valores.


## Operadores y expresiones
Son s�mbolos espec�ficos que van a tener una funci�n definida.

Los operadores se dividen en 4 tipos:

**Operadores de Asignaci�n ( = ):** Este nos permite asignarle el resultado de una expresi�n a una variable dada. Es importante recordar que la expresi�n debe de usar los mismo tipos de datos que vamos a guardar en la variable.

**Operadores Aritm�ticos:** Estos operadores van a tener un orden o jerarqu�a en la que se resuelven, los par�ntesis nos van a ayudar a que este orden se cumpla para llegar al resultado que se espera.

**Operadores Relacionales:** Estos nos van a servir para establecer una relaci�n entre dos n�meros y evaluarla o hacer una comparaci�n.

**Operadores L�gicos:**

a) Siempre nos van a devolver valores en verdadero o falso, los cuales son denominados valores booleanos.

b) En el lenguaje de programaci�n de C no existen los valores booleanos, por lo que as� se definen:

- **Valor verdadero.** Cualquier n�mero que sea distinto a cero.

- **Valor falso.** Cero.

- Lo convencional es que se utilice **1 para verdadero y 0 para falso.**

**Importante:**

+ Los operadores l�gicos o booleanos son empleados para comparar dos valores.

+ Los operadores l�gicos o booleanos denotan una relaci�n entre dos valores.

+ Los operadores l�gicos o booleanos tienen el mismo nivel de prioridad.
