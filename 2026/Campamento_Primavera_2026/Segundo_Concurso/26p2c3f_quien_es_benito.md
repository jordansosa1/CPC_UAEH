https://www.cpcjudge.com/problem/quienesbenito

# 26P2C3F. ¿Quién es benito? 👀

## Descripción
Benito es un gato que lleva un buen rato jugando ajedrez. Ya van varias partidas y se le están acumulando los pendientes.

A Benito le gusta empezar a hacer otras cosas cuando el momento sea "par".

Entonces se le ocurrió sumar todos los segundos desde que empezó a jugar hasta el segundo en el que está ahora.

Si esa suma es par, deja el tablero y se va a sus pendientes. Si es impar juega otro ratito de ajedrez.

Es decir si la suma de todos los enteros en el rango $[a, b]$ (incluyendo ambos extremos) es **par** o **impar**.

## Entrada
Una línea con dos enteros $a$ y $b$  $(1 \leq a \leq b \leq 10^{9})$, el segundo en el que Benito empezó a jugar y el segundo actual.

## Salida
Imprime ```ya estuvo``` si la suma del rango es par, o ```otro ratito``` si es impar.

## Ejemplo

### Entrada
```
1 4
```
### Salida
```
ya estuvo
```

### Entrada
```
2 4
```
### Salida
```
otro ratito
```

## Notas
En el primer ejemplo sumamos \(1 + 2 + 3 + 4 = 10\), que es par. Benito se levanta y se va a hacer sus cosas.

En el segundo la suma es \(2 + 3 + 4 = 9\), impar. Le toca seguir moviendo piezas otro rato.

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
    cin.tie(0); ios::sync_with_stdio(false);
    long long int l, r;
    cin >> l >> r;
    long long int s = (r * (r + 1)) / 2 - ((l - 1) * (l)) / 2;

    if (s % 2 == 0)
        cout << "ya estuvo";
    else
        cout << "otro ratito";

    return 0;
}

```
