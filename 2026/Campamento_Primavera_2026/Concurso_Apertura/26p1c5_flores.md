https://www.cpcjudge.com/problem/flores

# 26P1C5. Flores

## Descripción
*"Sembré una flor sin interés... yo la regaba con agua que cae del cielo"*

Honey está lista para otra gran jornada de trabajo polinizando flores y, como en cualquier trabajo, debe de cumplir con una cuota todos los días, que equivale a $X$ unidades de polen. Para lograrlo, ella dispone de $N$ flores puestas en fila.

Honey se encuentra cansada, así que cumplirá con **exactamente** esa cantidad si y solo si es posible que recolectar todo ese polen siguiendo una estrategia. Honey volará sobre flores específicas, haciendo un único recorrido desde una flor $L$ hasta la flor $R$, siendo $1 \leq L \leq R \leq N$, recolectando todo el polen dispuesto en ese intervalo.

Como te darás cuenta, el trabajo aún así es cansado, así que Honey necesitará de motivación, ayuda a Honey a saber de cuántas formas puede lograr recolectar la cantidad deseada de $X$ unidades de polen siguiendo su estrategia.


## Entrada
Dos enteros $N$ $(1 \leq N \leq 2*10^5)$ y $X$ $(1 \leq X \leq 10^9)$ , la cantidad de flores, y la cantidad de polen que necesita recolectar Honey respectivamente.
Seguido por $N$ enteros $A_1, A_2, A_3, ..., A_N$, donde $(1 \leq A_i \leq 10^9)$ indica la cantidad de polen de la flor $i$.

## Salida
Un entero, todas las formas en que Honey puede completar su estrategia.

## Ejemplo

### Entrada
```
5 7
2 4 1 2 7
```
### Salida
```
3
```
### Entrada
```
7 1
1 1 1 1 1 1 1
```
### Salida
```
7
```
### Entrada
```
10 19
2 4 10 12 15 12 8 16 12 1
```
### Salida
```
0
```

## Notas
En el primer caso, es posible tomar las flores en los rangos $[1, 3]$, $[2, 4]$ y $[5, 5]$, de forma que cumpla con **exactamente** las $7$ unidades esperadas.

En el segundo caso, tomar cualquier flor de forma individual basta para recolectar el polen requerido.

En el tercer caso, lamentablemente Honey no tiene forma de recolectar de forma exacta la cantidad necesaria.

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
