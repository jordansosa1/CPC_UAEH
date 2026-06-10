https://www.cpcjudge.com/problem/chesscarlosyangelica

# G. Ajedrez Primaveral
### Autor: Kaarlarax

## Descripción
Durante las cálidas tardes de primavera, Carlos y Angélica aprovechan el clima soleado para disfrutar su tiempo de ocio al aire libre. Después de pasar horas estudiando programación y algoritmos, deciden darle un descanso a sus mentes y relajarse bajo un árbol florecido jugando al ajedrez. Inspirados por la frescura de la temporada, deciden inventar un nuevo reto basado en un problema clásico.
Casi todo el mundo conoce el dilema de colocar ocho reinas en un tablero de ajedrez de $8 \times 8$ de manera que ninguna reina pueda capturar a otra. Sin embargo, Carlos y Angélica quieren ir más allá: desean saber el número máximo de piezas de ajedrez de un solo tipo que se pueden colocar en un tablero de dimensiones $m \times n$ de tal forma que ninguna pieza ataque a otra.

Como es bastante difícil calcular la solución a mano mientras intentan disfrutar de su tarde primaveral, te han pedido ayuda para programar la solución. No necesitan saber la respuesta para todas las piezas del juego. Los peones les parecen bastante aburridos y, de todas formas, Angélica perdió los alfiles entre las flores del jardín. Solo quieren saber cuántas Torres, Caballos, Reinas o Reyes se pueden colocar en el tablero sin que se ataquen entre sí.


## Entrada
La primera línea de entrada contiene un entero $T$, el número de casos de prueba.

<p>Cada caso de prueba consiste en una línea que contiene un carácter del conjunto { $r$, $k$, $Q$, $K$ }, que representan respectivamente las piezas Torre (Rook), Caballo (Knight), Reina (Queen) o Rey (King). El carácter es seguido por los enteros $m$ $(4 \le m \le 10)$ y $n$ $(4 \le n \le 10)$, que indican el número de filas y el número de columnas del tablero de ajedrez.

La casilla inferior izquierda es $(1, 1)$.

## Salida
Para cada caso de prueba, imprime el número máximo de piezas **de ese tipo** que se pueden poner en un tablero con las dimensiones dadas, de modo que no estén en posición de atacar a ninguna otra pieza.

## Ejemplo

### Entrada
```
2
r 6 7 
k 8 8
```
### Salida
```
6
32
```

## Temas identificados
### Matemáticas
- Adhoc

### Programación
- Ciclos
- Condicionales

## Propuesta de solución
Solo se piden 4 piezas distintas, por cada una de las piezas se puede hacer una simulación con el tablero dado o se pueden aplicar fórmulas para calcular la cantidad de piezas que caben en el tablero dado. Para explicar las fórmulas encontradas, voy a poner un ejemplo con un tablero de $5 \times 6$, con la solución para todas las piezas y con las fórumlas preparadas para trabajar con variables enteras:

- Para torres ```r```:

```
r . . . .
. r . . .
. . r . .
. . . r .
. . . . r
. . . . .
```
Observamos que para maximizar el número de piezas lo mejor es colocarlas en diagonal desde un borde hasta el otro, por lo que la diagonal va a ser tan grande como el lado más corto.

La fórmula encontrada es $\min${ $n,m$ }.

- Para reinas ```Q```:

```
. . . Q .
Q . . . .
. . Q . .
. . . . Q
. Q . . .
. . . . .
```
Observamos que las reinas tienen un acomodo parecido a los movimientos de un caballo, pero si hacemos casos, no daremos cuenta que pueden caber tantas reinas como torres, debido a su naturaleza ortogonal, por lo que de igual forma, caben tantas reinas como el lado más corto.

La fórmula encontrada es $\min${ $n,m$ }.

- Para reyes ```K```:

```
K . K . K
. . . . .
K . K . K
. . . . .
K . K . K
. . . . .
```
Observamos que los reyes se acomodan en una cuadrícula, pues cada uno puede atacar a sus 8 casillas adyacentes, se puede dejar solo un espacio entre cada uno, por lo que caben tantos reyes como la mitad del lado $n$, multiplicado por la mitad del lado $m$, pero hay que notar que si el lado es par, la división es correcta, pero si el lado es impar, el resultado de la división se desvía por 0.5 de la cantidad real,  por lo que hay que sumar una unidad a $m$ y a $n$, para luego dividir y redondear hacia abajo.

La fórmula encontrada es $\left(\frac{n+1}{2}\right)\left(\frac{m+1}{2}\right)$.

- Para caballos ```k```:

```
k . k . k
. k . k .
k . k . k
. k . k .
k . k . k
. k . k .
```
Observamos que los caballos siempre atacan a una casilla del color contrario al que están, por lo que podemos acomodar caballos en todas las casillas de un solo color sin que se ataquen, cabrán tantos coaballos como la cantidad de casillas dividido entre $2$, p

La fórmula encontrada es $\frac{n \cdot m + 1}{2}$.

## Implementación

```mermaid

```

### C++


```cpp
#include <bits/stdc++.h>

using namespace std;

int main() {
    cin.tie(0); ios::sync_with_stdio(false);

  	int q;
  	cin >> q;
  
  	for (int i = 0; i < q; i++) {
        char pieza;
        int n, m;
        cin >> pieza >> n >> m;

        switch(pieza) {
            case 'r':
                cout << min(n, m) << '\n';
                break;
            case 'Q':
                cout << min(n, m) << '\n';
                break;
            case 'K':
                cout << ((n + 1) / 2) * ((m + 1) / 2) << '\n';
                break;
            case 'k':
                cout << ((n * m) + 1) / 2 << '\n';
                break;
        }
  	}
}
```
