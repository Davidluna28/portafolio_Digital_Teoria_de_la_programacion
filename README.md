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



## unidad 2

## unidad 3
