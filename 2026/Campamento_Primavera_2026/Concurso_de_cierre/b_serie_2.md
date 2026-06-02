# B. Serie 2

## Descripción
*"¿No es así? Eso fue todo"*

Después de mucho esfuerzo, Felipe por fin está a punto de terminar su semestre, pero existe un pequeño detalle que aún debe resolver: el proyecto final de su clase "Fundamentos Electrónicos". Debido a esto él crea un pequeño circuito usando el módulo amplificador LM358, el cual duplica el voltaje que recibe.

Después de realizar las pruebas, Felipe comienza a trabajar con la versión final de su proyecto. Ahora construye **$N$** circuitos distintos, cada uno compuesto por señales de **$30$** módulos amplificadores, donde cada uno recibe ***1V*** desde el último al primero.

Para comprobar el funcionamiento, Felipe conecta varios circuitos a un bus de sincronización. Cada posición del bus corresponde a uno de los módulos del circuito, por lo que múltiples señales pueden llegar simultáneamente a la misma posición.

Por lo tanto:

- Si una posición recibe una cantidad impar de señales, el bus encenderá el módulo de esta posición.
- Si una posición recibe una cantidad par de señales, el bus apagará el módulo de esta posición.

Felipe hará $Q$ pruebas sobre el uso de este bus. En cada una seleccionará todos los circuitos en el rango de $L$ y $R$, conectándolos al bus. Él debe verificar sus resultados, ayúdalo a conocer cuánto será el voltaje final producido por el bus en cada prueba.

## Entrada
Dos enteros $N$ y $Q$ $(1 \leq N, Q \leq 2*10^5)$, la cantidad de circuitos y las pruebas a realizar.
Seguido por $N$ cadenas $S_1, S_2, S_3, ..., S_N$, donde $(|A_i| = 30)$, indica los módulos encendidos en el circuito $i$. Si el carácter $A_{ij}$ es $1$, significa que el amplificador $j$ del circuito $i$ está encendido.
Después $Q$ líneas, donde cada una se conforma por $2$ enteros $L$ y $R$, donde $(1 \leq L \leq R \leq N)$, indica una prueba que se realiza desde el circuito $L$ hasta el $R$.

## Salida
$Q$ enteros, el voltaje que tendrá el bus de sincronización en cada prueba.

## Ejemplo

### Entrada
```
5 1
001111101011001100011001001001
110100001011101110001100101111
111101100010011010001111001111
010011110000010001111110110000
010101110010101001100100001010
1 5
```
### Salida
```
19
```

## Notas
En el caso de ejemplo, la única consulta da como resultado 19, puesto que las posiciones $30$, $29$ y $26$ reciben una cantidad de $3$, $3$ y $1$ señales respectivamente, siendo las únicas impares, dando como resultado $1V + 2V + 16V = 19V$.

## Temas identificados


## Propuesta de solución


## Implementación

```mermaid

```

### C++



```cpp

```
