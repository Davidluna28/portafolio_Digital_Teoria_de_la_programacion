# Portafolio Digital de Aprendizaje – Teoría de la Programación

¡Hola! Este repositorio contiene mi portafolio digital donde registro los aprendizajes, ejercicios y reflexiones de la asignatura **Teoría de la Programación**.

---

## 📋 Carátula
<img width="1241" height="1755" alt="UNIVERSIDAD NACIONAL DE LOJA CARATULA_page-0001" src="https://github.com/user-attachments/assets/808f15e2-1b91-4113-9a5f-9090963e5584" />

---

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



## 📘 unidad 2

##Estructuras Condicionales.

- **Condicional Simple (if):**El condicional simple if (al que en idioma español le daríamos una traducción muy literal como "si..." de condición) es la estructura de control más básica de la programación. Se utiliza para que el programa tome una decisión en función de una única condición.
Básicamente le dice al programa: "evalúa esto. Si me devuelves 'verdadero' ejecuta esto. Si me devuelves 'falso' simplemente lo omites y continúas con lo tuyo".
<img width="402" height="241" alt="image" src="https://github.com/user-attachments/assets/880695bc-0316-46b0-b845-dc59cff4c84a" />

- **Condicional Doble (if else):**El condicional doble (if - else) es la estructura de control que nos da la opción de tomar una decisión entre un par de caminos posibles. A diferencia del if simple (donde solo hacíamos algo si se llegaba a dar la condición), aquí le obligamos al programa a hacer algo si la respuesta es verdadera y hacer otra cosa si es falsa.
En español se puede traducir como: "Si se da la condición, haz la Acción A; SI NO (else), haz la Acción B".
<img width="1024" height="614" alt="image" src="https://github.com/user-attachments/assets/e24b0c96-93ae-4ddc-a8ae-8e2a26649e3f" />

- **Condicional Múltiple (switch):**El Condicional Múltiple (switch) es el tipo de control que empleamos cuando una única variable puede ser evaluada para distintos valores y hacer un camino alternativo en cada caso.Lejos de encadenar diez bloques de if- else if lo que haría que el código fuese larguísimo y superdificil de leer , el switch evalúa la variable en una sola ocasión saltando directamente al "case" que coincida con el valor dado.
 <img width="1024" height="614" alt="image" src="https://github.com/user-attachments/assets/1065a472-5468-426a-977a-6a8ac53d0c5d" />



 ##Estructuras Repetitivas

 - **Ciclo Mientras (While):**El Ciclo Mientras (While) se presenta como una estructura de control repetitiva (o también denominada bucle) que permite la ejecución de un segmento de código repetidamente siempre que una condición dada mantenga su valor verdadero.
Dicho ciclo se denomina también como una estructura de "pre-condición" pues el programa es un poco "desconfiado", pues lo primero que debe hacer antes de cada vuelta es comprobar si la condición de para de bucle se cumple. Si desde el inicio mismo la condición resulta falsa, el programa no desarrollará el ciclo ni tan siquiera una vez, sino que lo eludirá.
<img width="1024" height="1024" alt="image" src="https://github.com/user-attachments/assets/9b49a951-8174-400f-b8b4-ebbe9768e31a" />

- **Ciclo Hacer - Mientras (Do - While):**El proceso Hacer - Mientras (Do - While) es un tipo de control repetido que provoca la obligación en el programa de ejecutar el bloque de código en cuestión al menos una vez, y tras ello proceder a la evaluación de si ha de seguir ejecutándose o no.
A la inversa del ciclo While (que comprueba la condición antes de entrar), el Do - While es una estructura de post-condición. En este caso, el programa es "atrevido": primero realiza la acción y a continuación pregunta.Se traduce, literalmente, por "Hacer estas operaciones y en el siguiente instante evaluar si mientras la condición sea verdadera se vuelve a ejecutar".
<img width="1024" height="1024" alt="image" src="https://github.com/user-attachments/assets/f27770c6-34cb-4d84-8343-60e22f66a405" />

- **Ciclo Para (For):**El ciclo Para (For) es aquella estructura de control repetitiva que empleamos cuando sabemos de antemano cuántas veces queremos que se ejecute un bloque de código, es decir, exactamente el número de veces.
Por otro lado, a diferencia de, el While o el Do-While que se ven sometidos a una condición que podría cambiar en el transcurrir del tiempo, el ciclo For está hecho para llevar una cuenta matemática correcta. Para ello, en su estructura agrupa tres elementos importantes en una sola línea:
La inicialización: Crea una variable "contador" (comúnmente nombrada como i) y le asigna un valor inicial (ej. i = 0).
La condición: El límite que le dice al ciclo cuando detenerse (ej. mientras i < 10).
El incremento/decremento: El incremento o decremento que le hacemos al contador en cada vuelta (ej. sumarle 1 a i: i++).
<img width="1024" height="1024" alt="image" src="https://github.com/user-attachments/assets/fca5e59d-8631-496d-a29b-6f0ae637846e" />

##Ejercicio Practico:structura condicional y repetitiva.

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









 

 































## unidad 3
