# Portafolio Digital de Aprendizaje – Teoría de la Programación

¡Hola! Este repositorio contiene mi portafolio digital donde registro los aprendizajes, ejercicios y reflexiones de la asignatura **Teoría de la Programación**.

---

<p align="center">
  <img width="450" height="300" alt="image" src="https://github.com/user-attachments/assets/31180891-5d02-4d67-bc77-633e94bd7d96" />

</p>

<h1 align="center">Universidad Nacional de Loja</h1>
<p align="center">
  <b>Facultad de Energía, las Industrias y los Recursos Naturales no Renovables</b><br>
  <span> Carrera de Computación</span> 💻
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Asignatura-Teor%C3%ADa%20de%20la%20Programaci%C3%B3n-blue?style=for-the-badge&logo=github" alt="Asignatura">
  <img src="https://img.shields.io/badge/Periodo-Abril%20--%20Agosto%202026-red?style=for-the-badge" alt="Periodo">
</p>

---

### 👤 Datos del Estudiante

*   **Estudiante:** David Santiago Luna Lara
*   **Docente:** Ing. Lissette López
*   **Ciclo:** Primer Ciclo

---

<details>
  <summary>📂 <b> Unidad 1: Fundamentos de Programación</b></summary>
  <br>
  <blockquote>

## 📘 Unidad 1: Fundamentos de Programación

### Contenidos
- **Algoritmo:** Definimos un algoritmo como una serie de instrucciones lógicas, ordenadas y finitas entre sí, mediante las cuales se soluciona un problema o existe una forma de procesar los datos. Se produce así una ejecución mediante un tipo de entrada (input), que se enfrenta a un conjunto de pasos concretos y que desemboca en una salida (output) del resultado esperado. Se puede entender como la base de todo lo que hace la programación, en el sentido de que se traduce la lógica humana a procesos que puede ejecutar la computadora de forma precisa.
- <img width="1122" height="1402" alt="image" src="https://github.com/user-attachments/assets/be2420c8-9bfd-4d77-a244-a7d30a1401b7" />


- **Pseudocódigo:** El pseudocódigo es el recurso para describir un algoritmo a través de un lenguaje congenial que está justo entre el lenguaje humano y el lenguaje de programación. No se trata de la ejecución de un código, sino de una herramienta de diseño lógico que ayuda a estructurar un proceso que no tiene que estar sujeto a normas técnicas..
- **Diagrama de flujo:** Un diagrama de flujo es la representación gráfica de un algoritmo o proceso, donde se emplean figuras geométricas para especificar y detallar cada uno de los pasos a realizar y flechas para explicar ordenar los pasos de forma lógica. Cada símbolo tiene un significado propio (los óvalos para el inicio/fin y los rombos para las decisiones, etc.) de forma que permite visualizar el camino de la información.
- <img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/4c3e7758-d783-477d-947a-6ea52c459cf2" />
- **Prueba de escritorio:** La prueba de escritorio es una forma de verificar la lógica mediante un proceso manual del algoritmo o del pseudocódigo que se quiere ejecutar, justo antes hacerlo en la computadora. Constituye la forma mediante la cual se elaboran las tablas en las que van figurando las variables y se van ejecutandolas instrucciones del pseudocódigo paso a paso asignando valores reales para ver cómo se producen los cambios. Este método permite detectar fallos de lógica, bucles infinitos, fallos en las condiciones, etc., de forma anticipada, a la vez que rápida y sencilla.
- **Lenguajes de programación:** Un lenguaje de programación es el conjunto de reglas sintácticas y semánticas que permiten a una persona escribir indicaciones precisas que serán ejecutadas por una computadora. Es un traductor que va de la lógica con la que se resuelven problemas a un código que genera una máquina en lenguaje binario, lo que el hardware del sistema entiende.
- **Programación por bloques:** Se trata de un recurso visual que facilita la creación de programas al conectar constituyentes gráficos que denotan instrucciones lógicas, eliminando la necesidad de codificar en un lenguaje de programación textual. En efecto, al conectar unos bloques con otros, como si de un rompecabezas se tratara, se asegura que la sintaxis que se aplica es la correcta y que el flujo es coherente.
  <img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/e21c0c5b-402c-40c9-bdcf-c602b064f3b4" />

### Ejercicio: Estructura Secuencial (presupuesto de pintura)

#### 1. Planteamiento del problema
Un almacén requiere determinar cuánto cobrar por trabajos de pintura. Considere que se cobra por m2. Realice el algoritmo que le permita ir generando presupuestos para cada cliente.

#### 2. Análisis del problema
* **Entradas:** largo (l), altura (h)
* **Proceso:** area <- largo * alto
		totalPagar <- area * costoPorM2
* **Salida:** total a pagar 

#### 3. Diseño del algoritmo
**Pseudocódigo:**
Algoritmo presupuesto
		
		// Definir variables de entrada y c?lculo
		Definir largo, alto, area, costoPorM2, totalPagar Como Real
		Definir nombreCliente Como Cadena
		
		Escribir "--- Generador de Presupuestos de Pintura ---"
		
		// Entrada de datos del cliente
		Escribir "Ingrese el nombre del cliente:"
		Leer nombreCliente
		
		// Entrada de medidas de la superficie
		Escribir "Ingrese el largo de la superficie (en metros):"
		Leer largo
		Escribir "Ingrese el alto de la superficie (en metros):"
		Leer alto
		
		// Entrada del precio unitario
		Escribir "Ingrese el costo por metro cuadrado ($):"
		Leer costoPorM2
		
		// Proceso: Calcular el ?rea y el costo total
		area <- largo * alto
		totalPagar <- area * costoPorM2
	
		// Salida de resultados (Presupuesto) //
		Escribir "        PRESUPUESTO DE PINTURA           "
		Escribir "Cliente: ", nombreCliente
		Escribir "Superficie total: ", area, " m2"
		Escribir "Precio por m2: $", costoPorM2
		Escribir "-----------------------------------------"
		Escribir "TOTAL A COBRAR: $", totalPagar
		Escribir "========================================="
FinAlgoritmo

**Diagrama de flujo:**


<img width="492" height="930" alt="image" src="https://github.com/user-attachments/assets/67d841f5-8e95-4ac8-96fb-9f94df9c3aa4" />


**Codigo fuente  :**
#include <stdio.h>

int main() {
    
    float largo, alto, area, costo, total;
    char nombre[50];

    printf("--- Presupuesto de Pintura ---\n");

    // Entrada de datos
    printf("Nombre del cliente: ");
    scanf("%s", nombre);

    printf("Largo de la pared: ");
    scanf("%f", &largo);

    printf("Alto de la pared: ");
    scanf("%f", &alto);

    printf("Costo por m2: ");
    scanf("%f", &costo);

    // Cálculos
    area = largo * alto;
    total = area * costo;

    // Salida de resultados
    printf("\nCliente: %s\n", nombre);
    printf("Total m2: %.2f\n", area);
    printf("TOTAL A PAGAR: $%.2f\n", total);

    return 0;
}

**Prueva de escritorio :**
<img width="1100" height="500" alt="prueba_escritorio_tabla" src="https://github.com/user-attachments/assets/7e226209-e40d-49a2-91ef-8b4d936ef74a" />
<img width="743" height="236" alt="image" src="https://github.com/user-attachments/assets/d22015e1-353b-4514-8dcc-093dcfc7e921" />


**Principales dificultades :**


Punteros y direcciones de memoria: Es lo que más marea. Tienes que aprender a usar el * y el & para decirle a la compu exactamente dónde guardar los datos, y si te equivocas, el programa explota (el famoso Segmentation Fault).

Sintaxis que no perdona: C es súper especial. Si te falta un punto y coma ; o si pones = en lugar de == en un if, el compilador te lanza mil errores que a veces no se entienden nada y te vuelven loco buscando el fallo.

El lío de los "Strings": En C no puedes simplemente crear un texto; tienes que manejar arreglos de caracteres a mano. Concatenar o comparar palabras es un dolor de cabeza porque tienes que cuidar los índices y el carácter de cierre \0

**Reflexcion Critica  :**



Lo más trascendente que aprendí es que programar no se puede reducir simplemente a tirar código por doquier, sino que hay que saber armar la lógica antes de tratar de tocar el teclado. "Llevar un diagrama o un pseudocódigo a un lenguaje como el C es un salto fuertísimo, sobre todo cuando entran en juego los punteros y la memoria". En cambio, "si haces tus pruebas de escritorio bien, te evitas mil enojos en el compilador". Al fin de cuentas, "se trata de ser ordenados, y sobre todo entender que cada paso cuenta para que el programa no truene".

</details>



<details>
  <summary>📂 <b>Unidad 2: Estructuras Condicionales y Repetitivas</b></summary>
  <br>
  <blockquote>
## 📘 Unidad 2: Estructuras Condicionales y Repetitivas

### Estructuras Condicionales.

- **Condicional Simple (if):** El condicional simple if (al que en idioma español le daríamos una traducción muy literal como "si..." de condición) es la estructura de control más básica de la programación. Se utiliza para que el programa tome una decisión en función de una única condición.
Básicamente le dice al programa: "evalúa esto. Si me devuelves 'verdadero' ejecuta esto. Si me devuelves 'falso' simplemente lo omites y continúas con lo tuyo".
<img width="402" height="241" alt="image" src="https://github.com/user-attachments/assets/880695bc-0316-46b0-b845-dc59cff4c84a" />

### Psudonimo

<img width="837" height="469" alt="image" src="https://github.com/user-attachments/assets/3a9dba88-7c95-4f43-8d2a-358d6fecb1fb" />




- **Condicional Doble (if else):** El condicional doble (if - else) es la estructura de control que nos da la opción de tomar una decisión entre un par de caminos posibles. A diferencia del if simple (donde solo hacíamos algo si se llegaba a dar la condición), aquí le obligamos al programa a hacer algo si la respuesta es verdadera y hacer otra cosa si es falsa.
En español se puede traducir como: "Si se da la condición, haz la Acción A; SI NO (else), haz la Acción B".
<img width="1024" height="614" alt="image" src="https://github.com/user-attachments/assets/e24b0c96-93ae-4ddc-a8ae-8e2a26649e3f" />

### Psudonimo

<img width="841" height="527" alt="image" src="https://github.com/user-attachments/assets/b0ec74da-8b62-4a53-a9ca-af3c67673c44" />




- **Condicional Múltiple (switch):** El Condicional Múltiple (switch) es el tipo de control que empleamos cuando una única variable puede ser evaluada para distintos valores y hacer un camino alternativo en cada caso.Lejos de encadenar diez bloques de if- else if lo que haría que el código fuese larguísimo y superdificil de leer , el switch evalúa la variable en una sola ocasión saltando directamente al "case" que coincida con el valor dado.
 <img width="1024" height="614" alt="image" src="https://github.com/user-attachments/assets/1065a472-5468-426a-977a-6a8ac53d0c5d" />


 ### Psudonimo


<img width="849" height="517" alt="image" src="https://github.com/user-attachments/assets/ad38b0d0-76bd-4de7-8f42-33ba208087e3" />


 



 ### Estructuras Repetitivas

 - **Ciclo Mientras (While):** El Ciclo Mientras (While) se presenta como una estructura de control repetitiva (o también denominada bucle) que permite la ejecución de un segmento de código repetidamente siempre que una condición dada mantenga su valor verdadero.
Dicho ciclo se denomina también como una estructura de "pre-condición" pues el programa es un poco "desconfiado", pues lo primero que debe hacer antes de cada vuelta es comprobar si la condición de para de bucle se cumple. Si desde el inicio mismo la condición resulta falsa, el programa no desarrollará el ciclo ni tan siquiera una vez, sino que lo eludirá.
<img width="1024" height="1024" alt="image" src="https://github.com/user-attachments/assets/9b49a951-8174-400f-b8b4-ebbe9768e31a" />

### Psudonimo


<img width="801" height="461" alt="image" src="https://github.com/user-attachments/assets/cb56d359-afc5-4e45-984d-dfed7a43cab2" />







- **Ciclo Hacer - Mientras (Do - While):** El proceso Hacer - Mientras (Do - While) es un tipo de control repetido que provoca la obligación en el programa de ejecutar el bloque de código en cuestión al menos una vez, y tras ello proceder a la evaluación de si ha de seguir ejecutándose o no.
A la inversa del ciclo While (que comprueba la condición antes de entrar), el Do - While es una estructura de post-condición. En este caso, el programa es "atrevido": primero realiza la acción y a continuación pregunta.Se traduce, literalmente, por "Hacer estas operaciones y en el siguiente instante evaluar si mientras la condición sea verdadera se vuelve a ejecutar".
<img width="1024" height="1024" alt="image" src="https://github.com/user-attachments/assets/f27770c6-34cb-4d84-8343-60e22f66a405" />


### Psudonimo



<img width="807" height="428" alt="image" src="https://github.com/user-attachments/assets/3ce3e303-908b-4aa9-af8a-246accb249ef" />






- **Ciclo Para (For):** El ciclo Para (For) es aquella estructura de control repetitiva que empleamos cuando sabemos de antemano cuántas veces queremos que se ejecute un bloque de código, es decir, exactamente el número de veces.
Por otro lado, a diferencia de, el While o el Do-While que se ven sometidos a una condición que podría cambiar en el transcurrir del tiempo, el ciclo For está hecho para llevar una cuenta matemática correcta. Para ello, en su estructura agrupa tres elementos importantes en una sola línea:
La inicialización: Crea una variable "contador" (comúnmente nombrada como i) y le asigna un valor inicial (ej. i = 0).
La condición: El límite que le dice al ciclo cuando detenerse (ej. mientras i < 10).
El incremento/decremento: El incremento o decremento que le hacemos al contador en cada vuelta (ej. sumarle 1 a i: i++).
<img width="1024" height="1024" alt="image" src="https://github.com/user-attachments/assets/fca5e59d-8631-496d-a29b-6f0ae637846e" />


### Psudonimo


<img width="798" height="464" alt="image" src="https://github.com/user-attachments/assets/78ee7ec1-6ffd-4e44-8bdb-95ba9b15f1d6" />




## Ejercicio Practico:structura condicional y repetitiva.

#### 1. Planteamiento del problema
Escribe un programa en C que solicite al usuario ingresar un número que esté obligatoriamente en el rango de 10 a 20 (inclusive). Si el usuario ingresa un número fuera de este rango, el programa debe mostrar un error y volver a pedir el número hasta que sea válido. Una vez ingresado un número correcto, el programa debe mostrar una cuenta regresiva desde ese número hasta el 0. Finalmente, debe calcular y mostrar en pantalla la suma de todos los números que formaron parte de esa cuenta regresiva.

#### 2. Análisis del problema
| **Etapa**              | **Actividad**           | **Detalle**                                                                                                  |
| ---------------------- | ----------------------- | ------------------------------------------------------------------------------------------------------------ |
| **Entrada**            | Ingreso de dato         | El usuario introduce un número entero.                                                                       |
| **Validación**         | Verificación del rango  | Se comprueba que el número esté entre 10 y 20, inclusive.                                                    |
| **Control de errores** | Solicitud de nuevo dato | Si el número está fuera del rango permitido, se muestra un mensaje de error y se vuelve a pedir otro número. |
| **Procesamiento**      | Cuenta regresiva        | Se realiza una cuenta regresiva desde el número válido hasta 0, disminuyendo de uno en uno.                  |
| **Procesamiento**      | Acumulación de suma     | Cada número de la cuenta regresiva se agrega a una variable acumuladora para obtener la suma total.          |
| **Salida**             | Mensaje de error        | Se muestra únicamente cuando el usuario ingresa un número fuera del rango permitido.                         |
| **Salida**             | Secuencia de números    | Se imprimen todos los valores de la cuenta regresiva.                                                        |
| **Salida**             | Resultado final         | Se muestra la suma total de los números incluidos en la cuenta regresiva.                                    |

#### 3. Diagrama de flujo
<img width="1271" height="936" alt="image" src="https://github.com/user-attachments/assets/7ae4cfa4-ae1b-4f1b-8e42-dd2497881a18" />

#### 4. Codigo fuente

#include <stdio.h>
int main() {
     int numero ,s=0;

     do{
        printf ("ingtrese un numero de 10 a 20\n");
        scanf("%i",&numero);

        if (numero<10 || numero>20){
            printf("numero fuera del rango permitido");
        } 
     } while (numero<10 || numero>20);
     printf("el numero sera decrecido:%i\n",numero);
     for (int a=numero;a>=0;a--){
        printf("%i\n",a);
        s=s+a;  
        
     }
     printf("la suma es %i\n",s);
     
    return 0;
}


#### 5. Prueva de escritorio 

| Iteración | Línea de código                          | **a (Contador)** | **Condición: ¿a ≥ 0?**            | **s (Suma acumulada)** | **Pantalla **                |
| --------- | ---------------------------------------- | ---------------- | --------------------------------- | ---------------------- | ---------------------------- |
| —         | `printf("el numero sera decrecido:12");` | —                | —                                 | 0                      | el numero sera decrecido: 12 |
| 1         | `int a = numero;`                        | 12               | Verdadero (12 ≥ 0)                | 0 + 12 = **12**        | 12                           |
| 2         | `a--`                                    | 11               | Verdadero (11 ≥ 0)                | 12 + 11 = **23**       | 11                           |
| 3         | `a--`                                    | 10               | Verdadero (10 ≥ 0)                | 23 + 10 = **33**       | 10                           |
| 4         | `a--`                                    | 9                | Verdadero (9 ≥ 0)                 | 33 + 9 = **42**        | 9                            |
| 5         | `a--`                                    | 8                | Verdadero (8 ≥ 0)                 | 42 + 8 = **50**        | 8                            |
| 6         | `a--`                                    | 7                | Verdadero (7 ≥ 0)                 | 50 + 7 = **57**        | 7                            |
| 7         | `a--`                                    | 6                | Verdadero (6 ≥ 0)                 | 57 + 6 = **63**        | 6                            |
| 8         | `a--`                                    | 5                | Verdadero (5 ≥ 0)                 | 63 + 5 = **68**        | 5                            |
| 9         | `a--`                                    | 4                | Verdadero (4 ≥ 0)                 | 68 + 4 = **72**        | 4                            |
| 10        | `a--`                                    | 3                | Verdadero (3 ≥ 0)                 | 72 + 3 = **75**        | 3                            |
| 11        | `a--`                                    | 2                | Verdadero (2 ≥ 0)                 | 75 + 2 = **77**        | 2                            |
| 12        | `a--`                                    | 1                | Verdadero (1 ≥ 0)                 | 77 + 1 = **78**        | 1                            |
| 13        | `a--`                                    | 0                | Verdadero (0 ≥ 0)                 | 78 + 0 = **78**        | 0                            |
| Final     | `a--`                                    | -1               | Falso (-1 ≥ 0) → termina el `for` | **78**                 | —                            |
| —         | `printf("la suma es %i\n", s);`          | -1               | —                                 | **78**                 | **la suma es 78**            |




<img width="695" height="435" alt="image" src="https://github.com/user-attachments/assets/d079fc1b-5966-4694-b9c7-258aad6ca015" />


#### Principales dificultades

El bucle infinito y la computadora congelada: Es lo que más marea en las estructuras repetitivas. En el while y el do-while tienes que acordarte sí o sí de modificar la variable de control adentro del ciclo (el famoso contador o acumulador). Si te descuidas y lo olvidas, la condición nunca se vuelve falsa y el programa se queda corriendo para siempre hasta que te explota la memoria o se te tilda la computadora.

El "caída libre" del switch por culpa del break: El switch se ve súper limpio, pero es traicionero. Si te olvidas de poner la palabra break al final de un caso, el compilador no te avisa nada; simplemente se pasa de largo y te ejecuta las instrucciones de los casos de abajo como si fueran parte del mismo. Te vuelves loco buscando por qué te salen tres respuestas al mismo tiempo.

Elegir el ciclo equivocado (while vs do-while): Confundir cuándo usar cuál es un dolor de cabeza. Si pones un while en una validación de menú, a veces el programa ni entra porque la condición falló desde el inicio. Y si pones un do-while donde no debías, te ejecuta un código intruso al menos una vez antes de darse cuenta de que la condición era falsa, rompiendo toda la lógica.

El desfase por uno (Off-by-one error) en el for: En el ciclo for manejas tres cosas en una sola línea (inicio, límite y paso). Es facilísimo equivocarse en el límite y poner un <= en lugar de <. Al final, el ciclo te da una vuelta de más o una de menos, y cuando trabajas con posiciones exactas, el programa truena.

#### Reflexion critica 

Lo más trascendente de aprender estas estructuras es entender que programar no se puede reducir simplemente a tirar código por doquier, sino que hay que saber armar la lógica antes de tratar de tocar el teclado. Llevar un diagrama de flujo o un pseudocódigo a las condicionales y ciclos es un salto fuertísimo, sobre todo cuando empiezas a anidar un if dentro de un for y todo se empieza a enredar como un espagueti.

En cambio, si haces tus diagramas de flujo bien y tiras tus pruebas de escritorio a mano (evaluando qué pasa si la condición da verdadero o falso), te evitas mil enojos con el programa corriendo mal. Al fin de cuentas, se trata de ser ordenados, entender que no hay que usar la estructura que mejor te caiga sino la que el problema necesita, y saber que cada decisión o cada vuelta cuenta para que el programa no se rompa.



</details>

 

 


<details>
  <summary>📂 <b>Unidad 3:Modularidad Y Arreglos </b></summary>
  <br>
  <blockquote>


## unidad 3 Modularidad Y Arreglos

### Modularidad :
La **modularidad** es un paradigma de diseño de software que fundamenta la descomposición de un sistema complejo en unidades funcionales discretas y autónomas, denominadas **módulos**. Estas unidades deben cumplir con dos criterios de diseño fundamentales:

* **Alta cohesión:** Cada módulo debe contener únicamente los elementos lógicos y funcionales necesarios para realizar una tarea específica, garantizando que el componente esté altamente enfocado.
* **Bajo acoplamiento:** Los módulos deben presentar una interdependencia mínima entre sí, comunicándose a través de interfaces bien definidas y estables.

Esta estructura permite la **encapsulación de la lógica**, lo que facilita el desarrollo paralelo, la reutilización de componentes y una gestión de errores más granular. En el contexto de la ingeniería de software, la modularidad es el pilar que permite la escalabilidad del sistema y la mantenibilidad a largo plazo, ya que permite modificar o actualizar secciones aisladas del código sin comprometer la integridad estructural del programa completo.

### Ventajas:
 * **Facilidad de Mantenimiento y Depuración**: Al estar el código fragmentado en módulos, el aislamiento de errores se vuelve mucho más sencillo. Si surge un fallo, es posible localizarlo y corregirlo dentro de un módulo específico sin tener que realizar cambios profundos en el sistema central o afectar áreas no relacionadas.

* **Reutilización de Código**: Los módulos bien diseñados funcionan como componentes independientes (como "piezas de Lego"). Esto permite que, una vez que una funcionalidad ha sido implementada y probada, pueda ser reutilizada en otros proyectos o en diferentes secciones del mismo programa, evitando la duplicidad de esfuerzos.

* **Desarrollo Paralelo**: En equipos de trabajo, la modularidad permite que diferentes desarrolladores trabajen en módulos distintos simultáneamente. Como la comunicación entre módulos se realiza a través de interfaces estandarizadas, el avance de un integrante no depende necesariamente de la finalización del trabajo de otro.

* **Legibilidad y Comprensión**: Un sistema modular es mucho más fácil de entender para nuevos integrantes o para el mismo autor después de un tiempo. Reduce la carga cognitiva, ya que permite al programador enfocarse en la lógica específica de un solo componente en lugar de intentar procesar todo el sistema de una sola vez.

* **Escalabilidad y Flexibilidad**: La modularidad permite extender las funcionalidades de un software de manera controlada. Si necesitas agregar una nueva característica, puedes desarrollar un nuevo módulo e integrarlo al sistema existente, lo que minimiza el riesgo de que la nueva implementación rompa la estructura funcional anterior.

* **Mejora en las Pruebas (Testing)**: Es mucho más eficiente realizar pruebas unitarias sobre módulos independientes. Esto garantiza que cada pequeño componente funcione según lo previsto de forma aislada antes de integrarse al conjunto, asegurando una mayor robustez global.

### Tipos de pases de parametros:

#### Paso por valor:
En este método, se crea una copia del valor del argumento original y se le asigna a la variable local de la función llamada.

* Comportamiento: Cualquier modificación que la función realice sobre el parámetro no afecta a la variable original en el ámbito de la función que la llamó.

* Uso: Es el método por defecto en lenguajes como C para tipos de datos primitivos (int, float, char).

* Ventaja: Seguridad, ya que los datos originales están protegidos contra efectos secundarios no deseados.

* Desventaja: Puede ser ineficiente si los datos son estructuras de gran tamaño, debido al consumo de memoria y tiempo requerido para realizar la copia.

### Ejemplo:
<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/1989aa8c-b9d3-4d53-9f34-00589da03351" />


#### Paso por referencia:
En lugar de pasar el valor del dato, se pasa la dirección de memoria (o una referencia) donde reside dicho dato.

* Comportamiento: La función llamada opera directamente sobre la ubicación de memoria del argumento original. Por lo tanto, cualquier cambio realizado dentro de la función sí afecta a la variable original.

* Uso : Se implementa mediante el uso de punteros. Pasas la dirección (&variable) y la función la recibe en un puntero (*ptr).

* Ventaja: Alta eficiencia, ya que no es necesario copiar datos voluminosos. Además, permite que una función devuelva múltiples valores modificando los parámetros recibidos.

* Desventaja: Mayor riesgo de errores (efectos secundarios inesperados) si la lógica no está bien controlada, ya que la integridad de los datos originales puede verse comprometida.

### Ejemplo:
<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/9945344e-5d00-40f0-a2fb-94a1f9550842" />


### Tabla Comparativa:

| **Característica**    | **Paso por Valor**                 | **Paso por Referencia**                 |
| --------------------- | ---------------------------------- | --------------------------------------- |
| ¿Qué se envía?        | Una copia del dato.                | La dirección de memoria.                |
| Efecto en el original | No hay cambios.                    | Los cambios persisten.                  |
| Memoria               | Consume espacio adicional (copia). | Ahorra memoria.                         |
| Velocidad             | Más lento con datos grandes.       | Más rápido.                             |
| Seguridad             | Mayor protección de datos.         | Menor protección (efectos secundarios). |

### Arreglos:
En el ámbito de la ingeniería de software, un arreglo (o array) es una estructura de datos estática que organiza una colección finita de elementos de tipo homogéneo en posiciones de memoria contiguas. Esta combinación de contigüidad y homogeneidad es lo que le permite ofrecer acceso directo a cualquier elemento sin necesidad de recorrer la estructura.
Desde una perspectiva técnica, se define por las siguientes características:

* **Tipado homogéneo**: todos los elementos comparten el mismo tipo de dato y, por lo tanto, ocupan un número fijo y conocido de bytes. Esta uniformidad es la que permite al compilador reservar un bloque de memoria regular y predecible, y es la condición necesaria para que el direccionamiento aritmético (ver punto siguiente) sea posible.
* **Adyacencia en memoria**: al ubicarse de forma secuencial dentro del bloque asignado, el sistema puede calcular la dirección física de cualquier elemento mediante una
* **fórmula aritmética simple**:
$$\text{Dirección del elemento} = \text{Dirección base} + (\text{índice} \times \text{tamaño del tipo de dato})$$
Por ejemplo, en un arreglo de enteros (int, 4 bytes) cuya dirección base es 1000, el elemento en el índice 3 se ubica en 1000 + (3 × 4) = 1012, sin necesidad de inspeccionar los elementos anteriores.
* **Acceso aleatorio en tiempo constante**: gracias a la fórmula anterior, cualquier posición es alcanzable en tiempo O(1)O(1)
O(1), independientemente del tamaño del arreglo o de la posición solicitada.
* **Tamaño fijo (estático)**: en su forma básica en lenguaje C, el tamaño del arreglo debe definirse en tiempo de compilación, por lo que la memoria reservada permanece inmutable durante la ejecución. Esta restricción es precisamente lo que hace posible el rendimiento superior descrito arriba: al no poder crecer ni reubicarse, el compilador puede garantizar contigüidad y direccionamiento constante. La contrapartida es una menor flexibilidad frente a estructuras dinámicas como las listas enlazadas.

### Ventajas:

* **Acceso directo (Tiempo constante $O(1)$)**: Gracias a su disposición contigua en memoria, puedes acceder a cualquier elemento de forma inmediata si conoces su índice. No necesitas recorrer los elementos anteriores, a diferencia de lo que ocurre en una lista enlazada.

* **Eficiencia en el uso de memoria**: Al no requerir punteros adicionales por cada elemento (como ocurre en estructuras dinámicas como las listas enlazadas), los arreglos tienen una sobrecarga de memoria mínima; solo ocupan el espacio estricto de los datos almacenados.
* **Gestión predecible**: Al ser estructuras de tamaño fijo definido en tiempo de compilación, el compilador puede calcular exactamente cuánta memoria necesita, lo que mejora el rendimiento y facilita la optimización del código.
* **Cache Friendly (Localidad de referencia)**: Debido a que los elementos están ubicados uno al lado del otro en la memoria, los procesadores pueden aprovechar el caché de la CPU de manera muy eficiente. Al cargar un elemento, es muy probable que los siguientes ya estén en el caché, lo que acelera drásticamente las operaciones de lectura.
* **Simplicidad en la manipulación**: Proporcionan una sintaxis intuitiva y directa para tareas comunes, como el recorrido mediante bucles (for) y la ordenación de datos, lo que los convierte en la herramienta base para implementar algoritmos fundamentales.

### Tipos de arreglos:

#### Arreglos Unidimensionales (Vectores):
Se comportan como una secuencia lineal de elementos. Es la estructura más básica para representar conjuntos de datos donde el orden importa pero no existe una relación jerárquica compleja.

* Lógica: Imagina una lista de la compra o una serie de mediciones de temperatura tomadas a lo largo de una hora. Solo necesitas una coordenada (el índice) para identificar un valor.

* Técnica: En memoria, el compilador reserva un bloque contiguo de tamaño N * sizeof(tipo_de_dato). Para acceder al elemento en la posición i, el procesador simplemente salta i posiciones desde la dirección base.

### Ejemplo:
<img width="1200" height="1524" alt="arreglo_unidimensional" src="https://github.com/user-attachments/assets/0bb47d9d-19de-4eb8-afe5-7f8116c8f729" />


#### Arreglos Bidimensionales (Matrices)
Se estructuran como una tabla de dos dimensiones. Aunque en la memoria física (RAM) los datos se almacenan de forma lineal, el lenguaje de programación los mapea lógicamente en filas y columnas.

* Lógica: Ideal para representar datos tabulares, como las celdas de una hoja de cálculo, los píxeles de una imagen en escala de grises o los movimientos en un tablero de ajedrez.

* Técnica: Se organizan usualmente en formato Row-Major Order (primero una fila completa, luego la siguiente). Para acceder a matriz[i][j], el compilador realiza una operación aritmética: Dirección_base + (i * número_de_columnas + j) * tamaño_dato.
 
### Ejemplo:

<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/f9d52de5-bf6d-4f6f-95eb-b338b089c059" />



#### Arreglos Multidimensionales (3D o superior)
Son estructuras que añaden profundidad a la matriz. Mientras un arreglo 2D es una "página" de datos, un arreglo 3D es un "libro" (un conjunto de páginas).
* Lógica: Se utilizan para representar datos de mayor complejidad. Un ejemplo clásico es el procesamiento de imágenes a color (RGB), donde la primera dimensión es el ancho, la segunda el alto y la tercera los canales de color (Rojo, Verde, Azul). También son comunes en simulaciones físicas o modelos matemáticos tridimensionales.
* Técnica: La complejidad de direccionamiento aumenta. El compilador calcula la dirección basándose en el producto de las dimensiones anteriores. A mayor dimensión, más cuidado debe tener el programador con el consumo de memoria, ya que el tamaño total del arreglo crece de forma exponencial ($N_1 \times N_2 \times N_3 \dots$).

### Ejemplo:

<img width="1200" height="1804" alt="arreglo_tridimensional (1)" src="https://github.com/user-attachments/assets/2bcc7cf2-cbf9-4c8f-a5b9-533a16f4cc06" />













</details>




<details>
  <summary>📂 <b>Concluciones:</b></summary>
  <br>
  <blockquote>








</details>






<details>
  <summary>📂 <b>Bibliografia:</b></summary>
  <br>
  <blockquote>

	  
#### Unidad1 
	  
 Cairó Battistutti, O. (2005). Metodología de la programación: Algoritmos, diagramas de flujo y programas (3ra ed.). Alfaomega.
 
Joyanes Aguilar, L. (2008). Fundamentos de programación: Algoritmos, estructura de datos y objetos (4ta ed.). McGraw-Hill

Brookshear, J. G. (2012). Introducción a la computación (11va ed.). Pearson Educación.

Resnick, M. (2019). Cultivar la creatividad: El aprendizaje a través de proyectos, la pasión, los compañeros y el juego. Programamos.

#### Unidad2


Joyanes Aguilar, L. (2008). Fundamentos de programación: Algoritmos, estructura de datos y objetos (4ta ed.). McGraw-Hill.

Cairó Battistutti, O. (2005). Metodología de la programación: Algoritmos, diagramas de flujo y programas (3ra ed.). Alfaomega.

McConnell, S. (2004). Code Complete: A Practical Handbook of Software Construction (2da ed.). Microsoft Press.







  </details>





<details>
  <summary>📂 <b>Uso de la IA:</b></summary>
  <br>
  <blockquote>


Declaro que para la elaboración de este portafolio digital se utilizaron herramientas de inteligencia artificial como ChatGPT, Gemini y NotebookLM como apoyo en la redacción, corrección de estilo y organización del contenido. El análisis, resolución de ejercicios, elaboración de diagramas de flujo y desarrollo de código fueron realizados por mi persona.




 </details>
  

