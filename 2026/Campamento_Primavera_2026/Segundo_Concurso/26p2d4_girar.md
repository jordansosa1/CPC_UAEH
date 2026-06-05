https://www.cpcjudge.com/problem/girar

# 26P2D4. Girar

## Descripción
*"Otra vez y otra vez y otra vez y otra vez y otra vez y otra vez..."*

Debido a las inundaciones recientes, Chato ha sido encargado de realizar una reparación en la UACH (Universidad Autónoma para Capibaras de Hidalgo), sin embargo, él no cuenta con los conocimientos para hacerla; lo cual no supone un problema, puesto que ha recibido instrucciones para ello. Aún con esto, él tiene el conflicto de una tarea en específico, la cual requiere que él atornille "al llegue". Esto es muy ambiguo ya que los grados necesarios para hacer esto pueden estar entre los $45$ y $60$  grados (inclusive) de giro extra después de que el tornillo oponga resistencia.

Ayuda a Chato a saber a cuántos grados se encuentra del valor más cercano del rango (o sea, cuál es la diferencia mínima respecto al rango), y si ya se encuentra dentro del intervalo, imprime el texto *"ahi mero es"*.

## Entrada
Un entero $A$ $(0 \leq A \leq 360)$, indicando los grados a los que Chato llegó.

## Salida
Un entero positivo $X$, la diferencia mínima de los grados a los cuales Chato está del rango, o en caso de estar dentro del rango, el texto *"ahi mero es"*

## Ejemplo

### Entrada
```
314
```
### Salida
```
254
```

### Entrada
```
53
```
### Salida
```
ahi mero es
```

### Entrada
```
19
```
### Salida
```
26

```

## Notas
En el primer caso, $314$ grados están alejados $254$ grados de $60$.

En el segundo caso, $53$ es mayor que $45$ y menor que $60$, así que ahí mero es.

En el tercer caso, $19$ está $26$ grados abajo de $45$.

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

    int n;
    cin >> n;
    if (n < 45) {
        cout << 45 - n;
    } else if (n >= 45 && n <= 60) {
        cout << "ahi mero es";
    } else {
        cout << n - 60;
    }

    return 0;
}
```
