https://www.cpcjudge.com/problem/quienesbenitov2

# 26P2C3D. ¿Quién es benito? 👀 (versión 2)

## Descripción
Benito es un gato que lleva un buen rato jugando ajedrez. Ya van varias partidas y se le están acumulando los pendientes.

A Benito le gusta empezar a hacer otras cosas cuando el momento sea "múltiplo de tres".

Entonces se le ocurrió sumar todos los segundos desde que empezó a jugar hasta el segundo en el que está ahora.

Si esa suma es múltiplo de tres, deja el tablero y se va a sus pendientes. Si no, juega otro ratito de ajedrez.

Es decir si la suma de todos los enteros en el rango $[a, b]$ (incluyendo ambos extremos) es **múltiplo de tres** o no.

## Entrada
Una línea con dos enteros $a$ y $b$  $(1 \leq a \leq b \leq 10^{18})$, el segundo en el que Benito empezó a jugar y el segundo actual.

## Salida
Imprime ```ya estuvo``` si la suma del rango es múltiplo de tres, o ```otro ratito``` si no lo es.

## Ejemplo

### Entrada
```
1 3
```
### Salida
```
ya estuvo
```

### Entrada
```
2 3
```
### Salida
```
otro ratito
```

## Notas
En el primer caso sumamos $1 + 2 + 3 = 6$, que es múltiplo de tres. Benito se levanta y se va a hacer sus cosas.

En el segundo caso la suma es $2 + 3 = 5$, no es múltiplo de tres. Le toca seguir moviendo piezas otro rato.

## Temas identificados
### Matemáticas
- 

### Programación
- 

## Propuesta de solución


## Implementación


### C++


```cpp
#include <iostream>
#include <bits/stdc++.h>

using namespace std;

long long int gauss(long long int n);

int main()
{
    cin.tie(0); ios::sync_with_stdio(false);

    long long int a, b;
    cin >> a >> b;
    
    a %= 3;
    b %= 3;
    
    long long int s = gauss(b) - gauss(a - 1);
    if (s % 3 == 0) {
        cout << "ya estuvo";
    } else {
        cout << "otro ratito";
    }

    return 0;
}

long long int gauss(long long int n) {
    long long int gaus = (n * (n + 1)) / 2;
    return gaus;
}
```
