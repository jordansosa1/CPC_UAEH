"Ya no es lo mismo que ayer, cuando el mundo nos vio florecer..."</em></p>
<p><br>
Sony, debido a la primavera, está planeando aprovechar los tiempos para hacer crecer todas las plantitas que tiene, increíblemente las plantas han logrado crecer 3 veces su tamaño. Dado el tamaño inicial por un entero \(N\), ¿cuál es el tamaño final de la plantita?</p>
<p><br></p>
<h3>Entrada</h3>
<p>Un entero \(N\) \((1 \leq N \leq 1000)\), indicando el tamaño inicial de la plantita.</p>
<p><br></p>
<h3>Salida</h3>
<p>Un entero \(X\), la altura final de la plantita.</p>
<p><br></p>
<h3>Ejemplo</h3>
<hr>
<h4>Entrada</h4>

<pre><code>1</code></pre>
<h4>Salida</h4>

<pre><code>3</code></pre>
<p><br></p>
<h4>Entrada</h4>

<pre><code>50</code></pre>
<h4>Salida</h4>

<pre><code>150</code></pre>
<p><br></p>
<h3>Notas</h3>
<p>En el primer caso, la plantita tiene un tamaño \(1\) inicialmente, terminando con un tamaño \(1 \cdot 3 = 3\).

https://www.cpcjudge.com/problem/plantita

# 26P2D1. Plantita
### Autor: Soria

## Descripción


## Entrada


## Salida


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
#include <bits/stdc++.h>

using namespace std;

int main()
{
    int n;
    cin >> n;
    cout << n * 3;

    return 0;
}
```
