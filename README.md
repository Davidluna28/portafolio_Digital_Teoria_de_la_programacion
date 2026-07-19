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





---

## 📑 Tabla de contenidos

| # | Unidad | Contenido |
|---|--------|-----------|
| 1 | [Fundamentos de Programación](#unidad-1) | Algoritmos, pseudocódigo, diagramas de flujo, prueba de escritorio |
| 2 | [Estructuras Condicionales y Repetitivas](#unidad-2) | `if`, `if-else`, `switch`, `while`, `do-while`, `for` |
| 3 | [Modularidad y Arreglos](#unidad-3) | Paso por valor/referencia, arreglos 1D, 2D y 3D |
| — | [Conclusiones generales](#conclusiones) | Aprendizajes integrados del curso |
| — | [Bibliografía](#bibliografia) | Referencias por unidad |
| — | [Uso de la IA](#uso-ia) | Declaración de transparencia |

---

<a id="unidad-1"></a>
<details open>
<summary><h2 style="display:inline">📘 Unidad 1 — Fundamentos de Programación</h2></summary>

### Contenidos teóricos

**Algoritmo**
Serie de instrucciones lógicas, ordenadas y finitas mediante las cuales se resuelve un problema o se procesa información. Recibe una entrada (*input*), la somete a un conjunto de pasos concretos, y produce una salida (*output*) con el resultado esperado. Es la base de toda la programación: traduce la lógica humana en procesos que la computadora puede ejecutar con precisión.

<img width="700" alt="Concepto de algoritmo" src="https://github.com/user-attachments/assets/be2420c8-9bfd-4d77-a244-a7d30a1401b7" />

**Pseudocódigo**
Recurso para describir un algoritmo mediante un lenguaje intermedio entre el lenguaje humano y el de programación. No es código ejecutable, sino una herramienta de diseño lógico que ayuda a estructurar un proceso sin estar sujeto a reglas sintácticas estrictas.

**Diagrama de flujo**
Representación gráfica de un algoritmo mediante figuras geométricas (óvalos para inicio/fin, rombos para decisiones, rectángulos para procesos) conectadas por flechas que indican el orden lógico de ejecución.

<img width="700" alt="Diagrama de flujo" src="https://github.com/user-attachments/assets/4c3e7758-d783-477d-947a-6ea52c459cf2" />

**Prueba de escritorio**
Verificación manual de la lógica de un algoritmo antes de programarlo. Consiste en elaborar una tabla con las variables y ejecutar el pseudocódigo paso a paso, asignando valores reales para observar cómo cambian. Permite detectar bucles infinitos, errores de condición y fallos lógicos de forma anticipada.

**Lenguajes de programación**
Conjunto de reglas sintácticas y semánticas que permiten escribir instrucciones precisas para que una computadora las ejecute — el puente entre la lógica de solución de problemas y el código binario que entiende el hardware.

**Programación por bloques**
Recurso visual que permite construir programas conectando piezas gráficas que representan instrucciones lógicas, sin necesidad de escribir código textual. Al encajar los bloques se garantiza automáticamente una sintaxis correcta y un flujo coherente.

<img width="700" alt="Programación por bloques" src="https://github.com/user-attachments/assets/e21c0c5b-402c-40c9-bdcf-c602b064f3b4" />

---

### 🧮 Ejercicio: estructura secuencial (presupuesto de pintura)

**Planteamiento del problema**
Un almacén necesita calcular el presupuesto de un trabajo de pintura, cobrando por metro cuadrado. Se debe generar un presupuesto por cliente.

**Análisis del problema**

| Elemento | Detalle |
|---|---|
| Entradas | Largo (`l`), alto (`h`) |
| Proceso | `area <- largo * alto` <br> `totalPagar <- area * costoPorM2` |
| Salida | Total a pagar |

**Pseudocódigo**
```text
Algoritmo presupuesto

    Definir largo, alto, area, costoPorM2, totalPagar Como Real
    Definir nombreCliente Como Cadena

    Escribir "--- Generador de Presupuestos de Pintura ---"

    Escribir "Ingrese el nombre del cliente:"
    Leer nombreCliente

    Escribir "Ingrese el largo de la superficie (en metros):"
    Leer largo
    Escribir "Ingrese el alto de la superficie (en metros):"
    Leer alto

    Escribir "Ingrese el costo por metro cuadrado ($):"
    Leer costoPorM2

    area <- largo * alto
    totalPagar <- area * costoPorM2

    Escribir "        PRESUPUESTO DE PINTURA           "
    Escribir "Cliente: ", nombreCliente
    Escribir "Superficie total: ", area, " m2"
    Escribir "Precio por m2: $", costoPorM2
    Escribir "-----------------------------------------"
    Escribir "TOTAL A COBRAR: $", totalPagar
    Escribir "========================================="
FinAlgoritmo
```

**Diagrama de flujo**

<img width="400" alt="Diagrama de flujo del presupuesto" src="https://github.com/user-attachments/assets/67d841f5-8e95-4ac8-96fb-9f94df9c3aa4" />

**Código fuente (C)**
```c
#include <stdio.h>

int main() {

    float largo, alto, area, costo, total;
    char nombre[50];

    printf("--- Presupuesto de Pintura ---\n");

    printf("Nombre del cliente: ");
    scanf("%s", nombre);

    printf("Largo de la pared: ");
    scanf("%f", &largo);

    printf("Alto de la pared: ");
    scanf("%f", &alto);

    printf("Costo por m2: ");
    scanf("%f", &costo);

    area = largo * alto;
    total = area * costo;

    printf("\nCliente: %s\n", nombre);
    printf("Total m2: %.2f\n", area);
    printf("TOTAL A PAGAR: $%.2f\n", total);

    return 0;
}
```

**Prueba de escritorio**

<img width="700" alt="Tabla de prueba de escritorio" src="https://github.com/user-attachments/assets/7e226209-e40d-49a2-91ef-8b4d936ef74a" />
<img width="500" alt="Prueba de escritorio - resultado" src="https://github.com/user-attachments/assets/d22015e1-353b-4514-8dcc-093dcfc7e921" />

> [!WARNING]
> **Principales dificultades**
> - **Punteros y direcciones de memoria**: es lo que más confunde al inicio. Hay que aprender a usar `*` y `&` para indicarle a la computadora exactamente dónde guardar los datos; un mal uso provoca el clásico *segmentation fault*.
> - **Sintaxis que no perdona**: C es muy estricto. Olvidar un `;` o escribir `=` en lugar de `==` en un `if` genera decenas de errores de compilación difíciles de interpretar.
> - **El manejo de cadenas (strings)**: en C no se crea texto de forma directa, hay que manejar arreglos de caracteres manualmente. Concatenar o comparar palabras exige cuidar los índices y el carácter de cierre `\0`.

> [!TIP]
> **Reflexión crítica**
> Lo más importante que aprendí es que programar no se reduce a escribir código sin más: primero hay que construir la lógica. Llevar un diagrama o un pseudocódigo hasta un lenguaje como C implica un salto considerable, sobre todo cuando entran en juego los punteros y la memoria. En cambio, una buena prueba de escritorio evita muchos dolores de cabeza frente al compilador. En definitiva, se trata de ser ordenado y entender que cada paso cuenta para que el programa no falle.

<div align="right"><a href="#top">⬆ Volver arriba</a></div>

</details>

---

<a id="unidad-2"></a>
<details>
<summary><h2 style="display:inline">📘 Unidad 2 — Estructuras Condicionales y Repetitivas</h2></summary>

### Estructuras condicionales

**Condicional simple (`if`)**
La estructura de control más básica. Evalúa una condición: si es verdadera, ejecuta un bloque de instrucciones; si es falsa, simplemente lo omite y continúa.

<img width="400" alt="if simple" src="https://github.com/user-attachments/assets/880695bc-0316-46b0-b845-dc59cff4c84a" />

*Pseudocódigo:*

<img width="500" alt="Pseudocódigo if" src="https://github.com/user-attachments/assets/3a9dba88-7c95-4f43-8d2a-358d6fecb1fb" />

**Condicional doble (`if... else`)**
Ofrece dos caminos posibles: ejecuta la Acción A si la condición es verdadera, o la Acción B si es falsa.

<img width="700" alt="if else" src="https://github.com/user-attachments/assets/e24b0c96-93ae-4ddc-a8ae-8e2a26649e3f" />

*Pseudocódigo:*

<img width="500" alt="Pseudocódigo if else" src="https://github.com/user-attachments/assets/b0ec74da-8b62-4a53-a9ca-af3c67673c44" />

**Condicional múltiple (`switch`)**
Se utiliza cuando una misma variable puede tomar distintos valores, cada uno con un camino alternativo. En lugar de encadenar múltiples `if-else if` (lo que vuelve el código largo y difícil de leer), el `switch` evalúa la variable una sola vez y salta directamente al `case` correspondiente.

<img width="700" alt="switch" src="https://github.com/user-attachments/assets/1065a472-5468-426a-977a-6a8ac53d0c5d" />

*Pseudocódigo:*

<img width="500" alt="Pseudocódigo switch" src="https://github.com/user-attachments/assets/ad38b0d0-76bd-4de7-8f42-33ba208087e3" />

### Estructuras repetitivas

**Ciclo mientras (`while`)**
Estructura de **pre-condición**: verifica la condición antes de cada vuelta. Si desde el inicio la condición es falsa, el ciclo no se ejecuta ni una sola vez.

<img width="500" alt="while" src="https://github.com/user-attachments/assets/9b49a951-8174-400f-b8b4-ebbe9768e31a" />

*Pseudocódigo:*

<img width="500" alt="Pseudocódigo while" src="https://github.com/user-attachments/assets/cb56d359-afc5-4e45-984d-dfed7a43cab2" />

**Ciclo hacer-mientras (`do-while`)**
Estructura de **post-condición**: ejecuta el bloque de código al menos una vez y luego evalúa si debe repetirse. A diferencia del `while`, aquí primero se actúa y después se pregunta.

<img width="500" alt="do while" src="https://github.com/user-attachments/assets/f27770c6-34cb-4d84-8343-60e22f66a405" />

*Pseudocódigo:*

<img width="500" alt="Pseudocódigo do while" src="https://github.com/user-attachments/assets/3ce3e303-908b-4aa9-af8a-246accb249ef" />

**Ciclo para (`for`)**
Se utiliza cuando se conoce de antemano cuántas veces debe ejecutarse un bloque de código. Reúne en una sola línea tres elementos: inicialización (`i = 0`), condición de parada (`i < 10`) e incremento/decremento (`i++`).

<img width="500" alt="for" src="https://github.com/user-attachments/assets/fca5e59d-8631-496d-a29b-6f0ae637846e" />

*Pseudocódigo:*

<img width="500" alt="Pseudocódigo for" src="https://github.com/user-attachments/assets/78ee7ec1-6ffd-4e44-8bdb-95ba9b15f1d6" />

---

### 🧮 Ejercicio: estructuras condicional y repetitiva combinadas

**Planteamiento del problema**
Escribir un programa en C que solicite un número entre 10 y 20 (inclusive), validando la entrada hasta que sea correcta. Una vez ingresado, debe mostrarse una cuenta regresiva desde ese número hasta 0, y al final la suma total de los valores recorridos.

**Análisis del problema**

| Etapa | Actividad | Detalle |
|---|---|---|
| Entrada | Ingreso de dato | El usuario introduce un número entero |
| Validación | Verificación del rango | Se comprueba que esté entre 10 y 20 |
| Control de errores | Solicitud de nuevo dato | Si está fuera de rango, se muestra un error y se vuelve a pedir |
| Procesamiento | Cuenta regresiva | Desde el número válido hasta 0, disminuyendo de uno en uno |
| Procesamiento | Acumulación de suma | Cada valor de la cuenta regresiva se suma a un acumulador |
| Salida | Mensaje de error | Solo si el número está fuera de rango |
| Salida | Secuencia de números | Se imprime cada valor de la cuenta regresiva |
| Salida | Resultado final | Suma total de los números recorridos |

**Diagrama de flujo**

<img width="700" alt="Diagrama de flujo ejercicio unidad 2" src="https://github.com/user-attachments/assets/7ae4cfa4-ae1b-4f1b-8e42-dd2497881a18" />

**Código fuente (C)**
```c
#include <stdio.h>

int main() {
    int numero, s = 0;

    do {
        printf("Ingrese un numero de 10 a 20\n");
        scanf("%i", &numero);

        if (numero < 10 || numero > 20) {
            printf("Numero fuera del rango permitido\n");
        }
    } while (numero < 10 || numero > 20);

    printf("El numero sera decrecido: %i\n", numero);

    for (int a = numero; a >= 0; a--) {
        printf("%i\n", a);
        s = s + a;
    }

    printf("La suma es %i\n", s);

    return 0;
}
```

**Prueba de escritorio**

| Iteración | Instrucción | `a` (contador) | Condición `a ≥ 0` | `s` (suma acumulada) | Pantalla |
|---|---|---|---|---|---|
| — | `printf("...decrecido:12");` | — | — | 0 | El numero sera decrecido: 12 |
| 1 | `int a = numero;` | 12 | Verdadero | 12 | 12 |
| 2 | `a--` | 11 | Verdadero | 23 | 11 |
| 3 | `a--` | 10 | Verdadero | 33 | 10 |
| 4 | `a--` | 9 | Verdadero | 42 | 9 |
| 5 | `a--` | 8 | Verdadero | 50 | 8 |
| 6 | `a--` | 7 | Verdadero | 57 | 7 |
| 7 | `a--` | 6 | Verdadero | 63 | 6 |
| 8 | `a--` | 5 | Verdadero | 68 | 5 |
| 9 | `a--` | 4 | Verdadero | 72 | 4 |
| 10 | `a--` | 3 | Verdadero | 75 | 3 |
| 11 | `a--` | 2 | Verdadero | 77 | 2 |
| 12 | `a--` | 1 | Verdadero | 78 | 1 |
| 13 | `a--` | 0 | Verdadero | 78 | 0 |
| Final | `a--` | -1 | Falso → termina `for` | 78 | — |
| — | `printf("la suma es...");` | -1 | — | 78 | **la suma es 78** |

<img width="500" alt="Salida del programa unidad 2" src="https://github.com/user-attachments/assets/d079fc1b-5966-4694-b9c7-258aad6ca015" />

> [!WARNING]
>
> 
> **Principales dificultades**
> - **El bucle infinito y la computadora congelada**: en `while` y `do-while` hay que recordar modificar siempre la variable de control dentro del ciclo. Si se olvida, la condición nunca se vuelve falsa y el programa corre indefinidamente.
> - **La "caída libre" del `switch` por el `break`**: si se omite el `break` al final de un `case`, el compilador no avisa nada — simplemente continúa ejecutando los casos siguientes, generando resultados inesperados y difíciles de depurar.
> - **Elegir el ciclo equivocado (`while` vs `do-while`)**: usar un `while` en una validación de menú puede hacer que el programa nunca entre si la condición falla desde el inicio; usar un `do-while` donde no corresponde ejecuta código no deseado al menos una vez.
> - **El desfase por uno (*off-by-one error*) en el `for`**: es fácil equivocarse en el límite (usar `<=` en lugar de `<`), lo que provoca una vuelta de más o de menos, especialmente problemático al trabajar con posiciones exactas.

> [!TIP]
>
> 
> **Reflexión crítica**
> Aprender estas estructuras confirma que programar exige construir la lógica antes de escribir código. Llevar un diagrama de flujo o un pseudocódigo hacia condicionales y ciclos anidados implica un salto importante, sobre todo cuando un `if` queda dentro de un `for` y la lógica empieza a complicarse. Elaborar bien los diagramas de flujo y ejecutar pruebas de escritorio a mano —evaluando qué ocurre si la condición es verdadera o falsa— evita muchos errores de ejecución. Al final, se trata de ser ordenado, elegir la estructura que el problema realmente necesita, y entender que cada decisión o repetición cuenta para que el programa no falle.

<div align="right"><a href="#top">⬆ Volver arriba</a></div>

</details>

---

<a id="unidad-3"></a>
<details>
<summary><h2 style="display:inline">📘 Unidad 3 — Modularidad y Arreglos</h2></summary>

### Modularidad

La **modularidad** es un paradigma de diseño de software que consiste en descomponer un sistema complejo en unidades funcionales discretas y autónomas, llamadas **módulos**. Estas unidades deben cumplir dos criterios de diseño fundamentales:

- **Alta cohesión**: cada módulo contiene únicamente los elementos lógicos y funcionales necesarios para una tarea específica, manteniéndose enfocado.
- **Bajo acoplamiento**: los módulos mantienen una interdependencia mínima entre sí, comunicándose mediante interfaces bien definidas y estables.

Esta estructura permite la **encapsulación de la lógica**, facilita el desarrollo paralelo, la reutilización de componentes y una gestión de errores más granular. En ingeniería de software, la modularidad es el pilar que permite la escalabilidad y la mantenibilidad a largo plazo, ya que posibilita modificar secciones aisladas del código sin comprometer la integridad del programa completo.

**Ventajas**

| Ventaja | Descripción |
|---|---|
| Facilidad de mantenimiento y depuración | Un fallo puede aislarse y corregirse dentro de un módulo específico sin alterar el sistema completo |
| Reutilización de código | Los módulos funcionan como piezas independientes que pueden reutilizarse en otros proyectos |
| Desarrollo paralelo | Distintos desarrolladores pueden trabajar en módulos diferentes de forma simultánea |
| Legibilidad y comprensión | Reduce la carga cognitiva al permitir enfocarse en un componente a la vez |
| Escalabilidad y flexibilidad | Nuevas funcionalidades se agregan como módulos adicionales, sin romper lo existente |
| Mejora en las pruebas (*testing*) | Permite realizar pruebas unitarias sobre módulos independientes antes de integrarlos |

### Tipos de paso de parámetros

#### Paso por valor:
Se crea una copia del valor del argumento y se asigna a la variable local de la función.

- **Comportamiento**: los cambios dentro de la función no afectan a la variable original.
- **Uso**: método por defecto en C para tipos primitivos (`int`, `float`, `char`).
- **Ventaja**: seguridad — los datos originales quedan protegidos de efectos secundarios.
- **Desventaja**: puede ser ineficiente con estructuras de gran tamaño, por el costo de copiar los datos.

<img width="700" alt="Paso por valor" src="https://github.com/user-attachments/assets/1989aa8c-b9d3-4d53-9f34-00589da03351" />

#### Paso por referencia:
En lugar del valor, se pasa la dirección de memoria donde reside el dato.

- **Comportamiento**: la función opera directamente sobre la ubicación de memoria del argumento original, por lo que los cambios sí persisten.
- **Uso**: se implementa mediante punteros — se pasa `&variable` y se recibe en un puntero `*ptr`.
- **Ventaja**: alta eficiencia, sin necesidad de copiar datos voluminosos; permite que una función "devuelva" varios valores modificando sus parámetros.
- **Desventaja**: mayor riesgo de efectos secundarios inesperados si la lógica no está bien controlada.

<img width="700" alt="Paso por referencia" src="https://github.com/user-attachments/assets/9945344e-5d00-40f0-a2fb-94a1f9550842" />

**Tabla comparativa**

| Característica | Paso por valor | Paso por referencia |
|---|---|---|
| ¿Qué se envía? | Una copia del dato | La dirección de memoria |
| Efecto en el original | No hay cambios | Los cambios persisten |
| Memoria | Consume espacio adicional (copia) | Ahorra memoria |
| Velocidad | Más lenta con datos grandes | Más rápida |
| Seguridad | Mayor protección de datos | Menor protección (efectos secundarios) |

### Arreglos

En ingeniería de software, un **arreglo** (o *array*) es una estructura de datos estática que organiza una colección finita de elementos de tipo homogéneo en posiciones de memoria contiguas. Esta combinación de contigüidad y homogeneidad es lo que permite el acceso directo a cualquier elemento sin recorrer la estructura.

- **Tipado homogéneo**: todos los elementos comparten el mismo tipo de dato y ocupan un número fijo de bytes, lo que permite al compilador reservar un bloque de memoria regular y predecible.
- **Adyacencia en memoria**: al ubicarse de forma secuencial, el sistema calcula la dirección de cualquier elemento con una fórmula aritmética simple:

$$\text{Dirección del elemento} = \text{Dirección base} + (\text{índice} \times \text{tamaño del tipo de dato})$$

  Por ejemplo, en un arreglo de enteros (4 bytes) con dirección base 1000, el elemento en el índice 3 se ubica en `1000 + (3 × 4) = 1012`, sin inspeccionar los elementos anteriores.
- **Acceso aleatorio en tiempo constante**: cualquier posición es alcanzable en tiempo $O(1)$, sin importar el tamaño del arreglo.
- **Tamaño fijo (estático)**: en C, el tamaño debe definirse en tiempo de compilación, por lo que la memoria reservada es inmutable durante la ejecución. Esta restricción es justamente lo que permite el rendimiento superior descrito arriba, a costa de menor flexibilidad frente a estructuras dinámicas como las listas enlazadas.

**Ventajas**

- **Acceso directo — $O(1)$**: cualquier elemento es accesible de forma inmediata conociendo su índice.
- **Eficiencia en el uso de memoria**: sin punteros adicionales por elemento, la sobrecarga de memoria es mínima.
- **Gestión predecible**: al tener tamaño fijo, el compilador calcula exactamente cuánta memoria reservar.
- ***Cache friendly* (localidad de referencia)**: al estar contiguos en memoria, el procesador aprovecha mejor el caché de la CPU.
- **Simplicidad de manipulación**: sintaxis intuitiva para recorrer (`for`) y ordenar datos.

### Tipos de arreglos

#### Arreglos unidimensionales (vectores):
Se comportan como una secuencia lineal de elementos — como una lista de compras o una serie de temperaturas registradas en una hora. Solo se necesita una coordenada (el índice) para identificar un valor. El compilador reserva un bloque contiguo de tamaño `N * sizeof(tipo)`, y acceder al elemento `i` implica saltar `i` posiciones desde la dirección base.

<img width="600" alt="Arreglo unidimensional" src="https://github.com/user-attachments/assets/0bb47d9d-19de-4eb8-afe5-7f8116c8f729" />

#### Arreglos bidimensionales (matrices):
Se estructuran como una tabla de dos dimensiones. Aunque en la memoria física los datos se almacenan de forma lineal, el lenguaje los mapea lógicamente en filas y columnas — ideal para hojas de cálculo, imágenes en escala de grises o un tablero de ajedrez. Se organizan en formato *row-major order* (primero una fila completa, luego la siguiente): para acceder a `matriz[i][j]`, el compilador calcula `Dirección_base + (i * número_de_columnas + j) * tamaño_dato`.

<img width="700" alt="Arreglo bidimensional" src="https://github.com/user-attachments/assets/f9d52de5-bf6d-4f6f-95eb-b338b089c059" />

#### Arreglos multidimensionales (3D o superior):
Añaden profundidad a la matriz: si un arreglo 2D es una "página" de datos, uno 3D es un "libro" completo de páginas. Se utilizan para representar datos más complejos, como imágenes a color RGB (ancho, alto y canal de color) o simulaciones físicas tridimensionales. La complejidad de direccionamiento aumenta, y el tamaño total del arreglo crece de forma multiplicativa según sus dimensiones ($N_1 \times N_2 \times N_3 \dots$).

<img width="600" alt="Arreglo tridimensional" src="https://github.com/user-attachments/assets/2bcc7cf2-cbf9-4c8f-a5b9-533a16f4cc06" />



> ### Principales dificultades en la aplicación de los contenidos:


> Durante el desarrollo de este trabajo sobre modularidad y arreglos, el mayor obstáculo fue asimilar la distinción real entre pasar un parámetro por valor y pasarlo por referencia. En un primer momento no lograba explicarme por qué, si en apariencia ambos mecanismos "entregaban" el mismo dato a la función, solo uno de ellos terminaba modificando la variable original. Fue necesario ejecutar distintos casos y seguir su comportamiento línea por línea para notar que todo dependía de qué se estaba enviando en realidad: una copia del contenido o la dirección donde ese contenido vive en memoria. A partir de ese momento entendí con más sentido por qué, cuando se busca que una función altere directamente la variable original, resulta indispensable recurrir al operador `&`.
>
> Respecto a los arreglos, no fueron los de una sola dimensión los que representaron un reto, dado que su comportamiento resulta casi natural de entender (una simple secuencia de valores localizables mediante un índice). El verdadero desafío apareció con las matrices y, más adelante, con las estructuras de tres dimensiones. Al operar con arreglos bidimensionales tuve que ensayar repetidamente con bucles anidados, ya que en un principio no tenía claro el orden correcto para recorrer filas y columnas, lo que me llevaba a dejar espacios sin asignar valor o a consultar posiciones equivocadas. Ese nivel de dificultad se incrementó al incorporar una tercera dimensión, pues ahí ya no bastaba con pensar en una tabla: había que representarse mentalmente varios planos o capas superpuestas, una imagen bastante más difícil de construir que la de un vector simple o una matriz plana.



> ### Reflexión crítica:



> La modularidad y los arreglos son contenidos que se entrelazan de forma constante en la práctica real de programar, dado que resulta habitual que las funciones reciban arreglos como parte de sus parámetros. En ese contexto, dominar la diferencia entre el paso por valor y por referencia deja de ser un simple detalle teórico, porque transferir un arreglo completo por valor implicaría un gasto de memoria innecesario y poco eficiente. La posibilidad de poner en práctica estos ejercicios durante las clases demostró que conocer la teoría no basta por sí sola: hace falta programar, equivocarse y corregir el rumbo para llegar a comprender de verdad cómo se comportan los parámetros y de qué manera se recorren los distintos tipos de arreglos. En síntesis, fue la práctica sostenida la que marcó la diferencia entre memorizar conceptos de forma superficial y realmente apropiarse de ellos.

<div align="right"><a href="#top">⬆ Volver arriba</a></div>

</details>

---

<a id="conclusiones"></a>
<details>
<summary><h2 style="display:inline">🧭 Conclusiones generales</h2></summary>



> Uno de los primeros aprendizajes que este proceso me dejó fue la importancia de analizar el problema antes de sentarme a programar. Apoyarme en pseudocódigo y en diagramas de flujo me permitió entender con claridad qué se esperaba resolver antes de escribir una sola línea de código, y la prueba de escritorio se convirtió en una especie de control de calidad previo: gracias a ella pude confirmar que mi razonamiento era correcto y detectar fallos antes de llegar a la versión final del programa.

A partir de esa base, comencé a trabajar con las **estructuras secuenciales**, lo que me permitió visualizar con claridad el orden en que la computadora ejecuta cada instrucción, una detrás de otra. Pasar de trabajar con bloques visuales a escribir código directamente me resultó bastante natural, y eso facilitó acostumbrarme rápido a la sintaxis y resolver sin mayor problema los ejercicios propuestos en clase.

El siguiente paso fue comprender las **estructuras condicionales**, la pieza clave que le da a un programa la capacidad de decidir entre distintos caminos —de forma simple, doble o múltiple— según se cumpla o no determinada condición. Sobre esa base avancé hacia las **estructuras repetitivas**, es decir los bucles o ciclos, que reducen considerablemente el tamaño y la complejidad de un programa al repetir automáticamente un mismo conjunto de instrucciones. Al recorrer el proceso completo —desde el diseño inicial hasta la validación mediante prueba de escritorio— en ejercicios que combinaban condicionales con ciclos, logré construir un razonamiento más sólido antes de programar.

Con esas bases de control de flujo ya asentadas, avancé hacia dos contenidos fundamentales para organizar programas más grandes: la **modularidad** y los **arreglos**. Reconocí que dividir un programa en módulos o funciones aporta mucho más que orden visual: permite aislar responsabilidades, de modo que cada parte del código se pueda probar, corregir o reutilizar sin revisar el programa completo. De manera paralela, entendí que los arreglos son una herramienta esencial para manejar varios datos relacionados bajo un mismo nombre, accediendo a la información mediante índices y recorriéndola con ciclos — la base para representar desde listas simples hasta estructuras más complejas como matrices o tablas de datos.

<div align="right"><a href="#top">⬆ Volver arriba</a></div>

</details>

---

<a id="bibliografia"></a>
<details>
<summary><h2 style="display:inline">📚 Bibliografía</h2></summary>

**Unidad 1**
1. O. Cairó Battistutti, *Metodología de la programación: Algoritmos, diagramas de flujo y programas*, 3.ª ed. México, D.F.: Alfaomega, 2005.
2. L. Joyanes Aguilar, *Fundamentos de programación: Algoritmos, estructura de datos y objetos*, 4.ª ed. Madrid: McGraw-Hill, 2008.
3. J. G. Brookshear, *Introducción a la computación*, 11.ª ed. Madrid: Pearson Educación, 2012.
4. M. Resnick, *Cultivar la creatividad: El aprendizaje a través de proyectos, la pasión, los compañeros y el juego*. Programamos, 2019.

**Unidad 2**




5. L. Joyanes Aguilar, *Fundamentos de programación: Algoritmos, estructura de datos y objetos*, 4.ª ed. Madrid: McGraw-Hill, 2008.
6. O. Cairó Battistutti, *Metodología de la programación: Algoritmos, diagramas de flujo y programas*, 3.ª ed. México, D.F.: Alfaomega, 2005.
7. S. McConnell, *Code Complete: A Practical Handbook of Software Construction*, 2.ª ed. Redmond, WA: Microsoft Press, 2004.

**Unidad 3**
1. B. W. Kernighan y D. M. Ritchie, *The C Programming Language*, 2.ª ed. Englewood Cliffs, NJ, EE. UU.: Prentice Hall, 1988.
2. P. J. Deitel y H. M. Deitel, *C: How to Program*, 8.ª ed. Hoboken, NJ, EE. UU.: Pearson, 2016.
3. R. Sedgewick y K. Wayne, *Algorithms*, 4.ª ed. Boston, MA, EE. UU.: Addison-Wesley Professional, 2011.
4. S. G. Kochan, *Programming in C*, 4.ª ed. Upper Saddle River, NJ, EE. UU.: Addison-Wesley, 2015.

<div align="right"><a href="#top">⬆ Volver arriba</a></div>

</details>

---

<a id="uso-ia"></a>
<details>
<summary><h2 style="display:inline">🤖 Uso de la IA</h2></summary>

> [!NOTE]


> Declaro que para la elaboración de este portafolio digital se utilizaron herramientas de inteligencia artificial —como ChatGPT, Gemini y NotebookLM— como apoyo en la redacción, corrección de estilo y organización del contenido. El análisis, la resolución de ejercicios, la elaboración de diagramas de flujo y el desarrollo de código fueron realizados por mi persona.

<div align="right"><a href="#top">⬆ Volver arriba</a></div>

</details>
