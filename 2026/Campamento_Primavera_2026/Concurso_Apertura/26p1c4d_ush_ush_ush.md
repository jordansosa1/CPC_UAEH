https://www.cpcjudge.com/problem/ush

# 26P1C4D. ush ush ush

## Descripción
Luego de superar los obstaculos con la fuerte neblina, Maullín, en su recorrido por el bosque, se encuentra cara a cara con un lobo que lo mira con hambre.

El gato apenas conoce este lugar, así que no puede simplemente huir en cualquier dirección, debe quedarse dentro del bosque o se perdería para siempre.

El bosque se representa como una cuadrícula de tamaño ***n · m***, donde cada celda contiene cualquier cosa del bosque representado por (```*```). Como Maullín no está para ponerse estricto, atraviesa los obstáculos sin problema con tal de escapar.

Hay celdas especiales: la posición inicial de Maullín, marcada con ```M```, y las posiciones de los lobos, marcadas con ```L```.
Tanto Maullín como los lobos pueden moverse en las **4 direcciones** (arriba, abajo, izquierda y derecha), siempre que la celda destino esté dentro de los límites del bosque.

**Todos están obligados a moverse en cada turno**, ninguno puede quedarse quieto.

Cada minuto ocurre lo siguiente:

- Primero, Maullín se mueve a una de las **4** celdas vecinas de la celda donde él se encuentra.
- Después, cada lobo (viendo hacia dónde se movió el gato) se mueve a una de las **4** celdas vecinas de la celda donde ese lobo se encuentra.

Si al final del minuto algún lobo termina en la misma celda que Maullín, el gato es cazado (yiyi).

Lo sé, la primavera suele representarse con días soleados y un buen ambiente, pero los lobos cazan de noche y aun así sigue siendo primavera jeje.

Ayuda a Maullín a saber si puede huir de los lobos para siempre dentro del bosque, o si tarde o temprano será atrapado.

## Entrada
En la primera línea, dos enteros ***n*** y ***m*** $(2 \leq n, m \leq 1000)$, las dimensiones del bosque.

Las siguientes ***n*** líneas contienen ***m*** caracteres cada una, que representan el bosque. Cada celda es uno de los siguientes caracteres:

- ```*``` representa una celda transitable.
- ```M``` representa la posición inicial de Maullín.
- ```L``` representa la posición inicial de un lobo.

Se garantiza que hay exactamente una ```M``` y al menos una ```L``` en el mapa.

## Salida
Imprime ```ay maullin``` si Maullín puede escapar indefinidamente, o ```jeje``` si los lobos terminarán por atraparlo.

## Ejemplo

### Entrada
```
2 2
M L
* *
```
### Salida
```
ay maullin
```
### Entrada
```
2 2
M *
* L
```
### Salida
```
jeje
```
### Entrada
```
5 5
* * * * L
* * * * *
* * M * *
* * * * L
L * * * *
```
### Salida
```
jeje
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
