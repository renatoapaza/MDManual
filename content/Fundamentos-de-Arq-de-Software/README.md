# Fundamentos de Arquitectura de Software

>_"La estructura del sistema, compuesta por elementos de software, sus propiedades visibles y sus relaciones"_

**Ley de Conway***

>_"Cualquier pieza de software refleja la estructura organizacional que la produjo.""_

## 1. El proceso de desarrollo de software

### Etapas del proceso de desarrollo de software

El proceso de desarrollo tradicional tiene etapas muy marcadas, que tienen entradas, procesos y salidas que funcionan como entradas de la siguiente etapa.

+ **An�lisis de requerimientos**: Todo nace de un disparador que nos crea la necesidad de crear un artefacto o un sistema. Necesitamos entender cu�l es el problema que queremos resolver. Hay requerimientos de negocio, requerimientos funcionales, requerimientos no funcionales.

    + **Requerimientos funcionales** son todos aquellos servicios o cosas que debe hacer la aplicaci�n o sistema que se esta creando.

    + **Requerimientos no funcionales** son requerimientos que no son relacionados directamente al objeto del sistema como puede ser fiabilidad, estabilidad del sistema, capacidad de almacenamiento, tiempo de respuesta etc.

+ **Dise�o de la soluci�n**: An�lisis profundo de los problemas para trabajar en conjunto y plantear posibles soluciones. El resultado de esto debe ser el detalle de la soluci�n, a trav�s de requerimientos, modelado, etc.

+ **Desarrollo y evoluci�n**: Implementaci�n de la soluci�n, para garantizar que lo que se esta construyendo es lo que se espera. Al finalizar esta etapa tendremos un artefacto de software.

+ **Despliegue**: Aqu� vamos a necesitar de infraestructura y de roles de operaci�n para poder poner el artefacto a disponibilidad.

+ **Mantenimiento y evoluci�n**: Desarrollo + despliegue + mantenimiento, en esta etapa estamos atentos a posible mejoras que se hacen al sistema. En esta etapa el software se mantiene hasta que el software ya deja de ser necesario.

![image](https://raw.githubusercontent.com/wlizama/MDManual/master/assets/images/proceso-de-desarrollo-software.jpg "Etapas del proceso de desarrollo de software")

### Dificultades en el desarrollo de software

En la etapa de **Dise�o y Desarrollo** estamos concentrados en encontrar cu�les son los problemas que queremos resolver. Estos problemas los podemos dividir en dos grandes tipos de problemas.

**Esenciales**: Los podemos dividir en 4.

  1. **La complejidad**, cu�ndo lo que tenemos que resolver es complejo en si mismo. En el caso de adiciones y todas las acciones que conlleven al sistema a ser m�s complejo.

       _Manejo del problema de complejidad_: No desarrollar: Comprar - OSS
  
  2. **La conformidad**, en qu� contexto se usa el software y c�mo debe adecuarse al mismo. Se incluyen todo lo que le compete. _Ej_: Ambiente, conectividad, impuestos, etc.

       _Manejo del problema de complejidad_: Prototipado r�pido, feedback y ciclos r�pidos para soluciones peque�as.
  
  3. **Tolerancia al cambio**, posibilidad del cambio en el mismo y que sea responsivo a diferentes contextos.
       
       _Manejo del problema de complejidad_: Desarrollo Evolutivo, desarrollos peque�os. Paso a paso pero de manera firme e ir haciendo crecer el software.
  
  4. **Invisibilidad**, problemas de tangibilidad nula.

       _Manejo del problema de complejidad_: Grandes dise�adores, Arquitectos que saben abtraer el problema y que realiza soluciones elegantes, de manera simple, con la mejor calidad posible en los componentes que lo necesitan.

**Accidentales**: Est� relacionado con la plataforma que vamos a implementar, tecnolog�a, lenguajes, frameworks, integraciones, etc, tienen 3 entornos:

  1. **Lenguajes de alto nivel**, son las complicaciones que surgen al lidiar con los lenguajes que se escogieron para el desarrollo del proyecto. 
  
  2. **Multi-procesamiento**, es la necesidad de resolver o atender a varios problemas en un mismo momento.
  
  3. **Entornos de programaci�n**, son los problemas que devienen de las herramientas que hemos usado para resolver los problemas enti�ndase frameworks compilados librar�as etc.

> "Concidero a la especificaci�n, dise�o y comprobaci�n del concepto la parte dif�cil de hacer software. (...) Si esto es cierto, hacer software siempre ser� dif�cil. No existe la bala de plata."
>
> Del libro _No Silver Bullet_ (Frederick P. Brooks Jr., 1986)

### Roles

Es importante que diferenciemos el ROL del puesto de trabajo, hay roles que pueden ser desarrollados por la misma persona.

**Experto del dominio (stakeholders)** En una metodologia tradicional, es la persona a la que acudimos para entender las necesidades del negocio. En metodologias Agiles.

**Analista** funcional/de negocio, la persona responsable de definir los requerimientos que van a llevar al software a u buen puerto. En el caso de Agiles el due�o del producto es quien arma las historias y que nos acompa�a en el proceso de construcci�n del software.

**Administrador de sistemas / DevOps** Es el rol de operaciones y desarrollo, son las personas responsables de la infraestructura que alojara nuestra aplicaci�n.

**Equipo de desarrollo**  QA / Testing se encargan de la evaluaci�n de nuestro software, comprobar que lo que se esta haciendo es lo que se espera que se haga. Desarrolladores involucrados en la construcci�n del software. Arquitecto, dise�a la soluci�n y analisis de los requerimientos, es un papel mas estrategico. La arquitectura emerja del trabajo de un equipo bien gestionado.

**Gestor del proyecto / facilitador** Llevan al equipo a trav�s del proceso iterativo e incremental, entender lo que pasa con el equipo y motivar el avance en el desarrollo del producto.

## 2. Introducci�n a la arquitectura de software

### Objetivos del arquitecto

Cada uno de los stakeholder tiene que ser conectado por el Arquitecto con sus requerimientos.

**Stakeholder -> Arquitecto -> Requerimientos = Implementaci�nes en el Sistema.**

Los Requerimientos de cada stakeholder afectan de forma �nica el sistema.

**Cliente**: Entrega a tiempo y dentro del presupuesto.

**Manager**: Permite equipos independientes y comunicaci�n clara.

**Dev**: Que sea f�cil de implementar y de mantener.

**Usuario**: Es confiable y estar� disponible cuando lo necesite.

**QA**: Es f�cil de comprobar.

La uni�n de todos estos requerimientos (funcionales o no funcionales) van a llevar al arquitecto a tomar decisiones que impacten sobre el sistema.