https://www.cpcjudge.com/problem/sillas

# 26P1C3. Sillas

## Descripción
Al momento de organizar un evento masivo, un aspecto crucial es acomodar los asientos de las personas. Para ello, los organizadores crearon una regla que debe cumplirse sin excepción:

- No se puede sentar a ninguna persona junto a otra.

Esto se debe a que las personas son tan platicadoras que terminan arruinando por completo el evento, quitándole todo el sentido.

Inicialmente, los organizadores habían distribuido invitaciones considerando cierta capacidad. Sin embargo, debido a un recorte presupuestal inesperado, ahora necesitan **reducir la cantidad total de asistentes**.

Dado este recorte, tu tarea es determinar, para cada fila, cuál es la **mínima** cantidad de personas que debes sentar (incluyendo las ya sentadas) cumpliendo que:

1. No haya personas en sillas consecutivas.
2. No sea posible agregar una persona más sin romper la regla.
   
Cabe mencionar que cada fila se analiza de manera independiente.

## Entrada
En la primera línea un entero $F$ $(1 \leq F \leq 10^4)$, indicando el número de filas de sillas en el evento.
Para cada $i$-$ésima$ fila:

Un entero $N_i$ $(1 \leq N_i \leq 2 \cdot 10^5)$, la cantidad de sillas en la $i$-$ésima$ fila.
En la siguiente línea una cadena $C_i$ $(1 \leq |C_i| \leq 2 \cdot 10^5)$, donde:

- **0** representa un lugar disponible.
- **1** representa un lugar ya ocupado.

Se garantiza que la suma total de sillas no excede $2 \cdot 10^5$ y que no existe ningún par consecutivo de sillas ocupadas; es decir, ningún par rompe la regla mencionada.

## Salida
Por cada fila, imprimir un único entero: la **mínima** cantidad de personas que debes sentar para que sea imposible sentar a más gente.

## Ejemplo

### Entrada
```
4
3
000
4
0000
5
01000
8
01010101
```
### Salida
```
1
2
2
4
```

## Notas
Para la primera fila, el único acomodo válido es **010** porque ya no permite que se sienten más personas. El acomodo **101** tampoco permite que se sienten más personas, sin embargo, no es la cantidad mínima. Por lo tanto, la respuesta es **1**.

Para la segunda fila, un acomodo válido es **0101**. Se puede demostrar que no existe un acomodo con menos personas, por lo que la respuesta es **2**.
Para la cuarta fila, no existe lugar disponible, por lo que la respuesta es **4**.

## Temas identificados
### Matemáticas
- 

### Programación
- 

## Propuesta de solución


## Implementación


### C++


```cpp

```

### Java


```java

```

### Python


```python

```

### Kotlin


```kotlin

```
