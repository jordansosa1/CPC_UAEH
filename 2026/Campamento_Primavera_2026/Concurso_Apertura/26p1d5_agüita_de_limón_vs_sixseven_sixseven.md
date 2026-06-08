https://www.cpcjudge.com/problem/

# 26P1D5. Agüita de limón vs sixseven sixseven

## Descripción
El calor nos está matando de sed y, a pesar de que todo el mundo carga su botella de agua, ésta no dura más de \(5\) minutos.
Tú quieres aprovechar la situación y comienzas a vender agüita de limón a \(X\) pesos el vaso para así probar suerte y hacerte millonario.

Un día, el meme sixseveeeeeen sixseveeeeeen se hizo tan viral que comenzaste a odiar todo lo que tuviera que ver con un \(6\) o un \(7\).

Es tanto tu odio que si atiendes un grupo de \(C_i\) personas y \(C_i\) es divisible entre \(6\) o \(7\), prefieres no venderles.

En caso contrario, les venderás \(C_i\) vasos de agüita de limón.

Desgraciadamente, mientras vendías agüita de limón, te dio un golpe de calor y no recuerdas cuánto dinero ganaste, pero si recuerdas a los \(N\) grupos que atendiste.

Como eres programador, escribirás un programa que calcule tu ganancia total.
<p></p>
<p><br></p>
<h3>Ejemplos</h3>
<hr>
<h4>Entrada</h4>

<pre><code>3 10
5 6 7</code></pre>
<h4>Salida</h4>

<pre><code>50</code></pre>
<p><br></p>
<h4>Entrada</h4>

<pre><code>6 2
10 11 12 10 14 42</code></pre>
<h4>Salida</h4>

<pre><code>62</code></pre>
<p><br></p>
<h4>Entrada</h4>

<pre><code>5 100
42 18 21 84 36</code></pre>
<h4>Salida</h4>

<pre><code>0</code></pre>
<h3>Notas</h3>
<hr>
<p>En el primer caso, la ganancia se calcula de la siguiente forma:</p>
<ul>
<li>Tu ganancia = \(0\)</li>
<li>Llegó un grupo de \(5\) personas, y \(5\) no es divisible entre \(6\) ni \(7\), por lo tanto vendes \(5\) vasos
ganaste \(5 \cdot 10 = 50\) pesos, ganancia = 50</li>
<li>Llegó un grupo de \(6\) personas, y \(6\) es divisible entre \(6\), no vendes nada</li>
<li>Llegó un grupo de \(7\) personas, y \(7\) es divisible entre \(7\), no vendes nada
Tu ganancia total es de \(50\) pesos.</li>
</ul>
<p><br>
En el segundo caso, únicamente le vendes a los grupos de \(10\), \(11\) y \(10\) personas.
Tu ganancia total es de \((10 \cdot 2)+(11 \cdot 2)+(10 \cdot 2) = 20+22+20 = 62\) pesos.

## Entrada
En la primera línea dos enteros \(N\) \((1 \leq N \leq 1000)\) y \(X\) \((1 \leq X \leq 100)\), la cantidad de grupos y el precio por vaso, respectivamente.

En las siguientes \(N\) líneas un entero \(C_i\) \((1 \leq C_i \leq 100)\), la cantidad de personas del \(i\)-\(ésimo\) grupo.

## Salida
Tu ganancia total.

## Ejemplo

### Entrada
```

```
### Salida
```

```

## Notas


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
