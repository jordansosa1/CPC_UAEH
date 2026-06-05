https://www.cpcjudge.com/problem/ushvf

# 26P1C4F. ush ush ush (Versión fácil)

## Descripción
Luego de superar los obstaculos con la fuerte neblina, Maullín, en su recorrido por el bosque, se encuentra cara a cara con un lobo que lo mira con hambre.

El gato apenas conoce este lugar, así que no puede simplemente huir en cualquier dirección, debe quedarse dentro del bosque o se perdería para siempre.

El bosque se representa como una cuadrícula de tamaño $n \cdot m$, donde cada celda es transitable.

Tanto Maullín como el lobo pueden moverse en las **4 direcciones** (arriba, abajo, izquierda y derecha), siempre que la celda destino esté dentro de los límites del bosque.

**Todos están obligados a moverse en cada turno**, ninguno puede quedarse quieto.

Cada minuto ocurre lo siguiente:

- Primero, Maullín se mueve a una de las $4$ celdas vecinas de la celda donde él se encuentra.
- Después, el lobo (viendo hacia dónde se movió el gato) se mueve a una de las $4$ celdas vecinas de la celda donde se encuentra.

Si al final del minuto el lobo termina en la misma celda que Maullín, el gato es cazado (yiyi).

Lo sé, la primavera suele representarse con días soleados y un buen ambiente, pero los lobos cazan de noche y aun así sigue siendo primavera jeje.

Ayuda a Maullín a saber si puede huir del lobo para siempre dentro del bosque, o si tarde o temprano será atrapado.

## Entrada
En la primer linea, dos enteros $n$ y $m$ $(2 \leq n, m \leq 1000)$, las dimensiones del bosque.
En la segunda linea $M_i$ y $M_j$, $(1 \leq M_i \leq n)$ $(1 \leq M_j \leq m)$ la posición inicial de Maullín.
En la tercer linea $L_i$ y $L_j$, $(1 \leq L_i \leq n)$ $(1 \leq L_j \leq m)$ la posición inicial del lobo.

Se garantiza que las posiciones son distintas y están dentro del bosque. 

## Salida
Imprime ```ay maullin``` si Maullín puede escapar indefinidamente, o ```jeje``` si el lobo terminará por atraparlo.

## Ejemplo

### Entrada
```
2 2
1 1
1 2
```
### Salida
```
ay maullin
```
### Entrada
```
2 2
1 1
2 2
```
### Salida
```
jeje
```
### Entrada
```
8 8
2 2
7 4
```
### Salida
```
ay maullin
```

## Notas
En el primer caso, Maullín tiene dos formas de sobrevivir cada minuto:

1. Moverse a la diagonal opuesta del lobo. Desde ahí, sin importar a cuál de sus dos vecinas se mueva el lobo, nunca coincidirá con la celda del gato.
2. Moverse a la propia celda del lobo. Como el lobo está obligado a abandonarla en su turno, Maullín queda solo y a salvo.

En el segundo caso, sin importar hacia dónde corra Maullín, el lobo lo atrapará en el primer movimiento ya que prácticamente sus 2 opciones son las casillas vecinas del lobo.

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
