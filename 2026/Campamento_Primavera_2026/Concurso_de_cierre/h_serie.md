https://www.cpcjudge.com/problem/serie

# C. Dopamina

## Descripción
*"Fue todo, ¿no es así?"*
Después de mucho esfuerzo, Felipe por fin está a punto de terminar su semestre, pero existe un pequeño detalle que aún debe resolver: el proyecto final de su clase "Fundamentos Electrónicos".
Debido a esto él crea un pequeño circuito usando el módulo amplificador LM358, el cual duplica el voltaje que recibe. Felipe decide realizar una pequeña prueba primero, por lo que crea un circuito donde conecta las señales de 10 de estos amplificadores y una señal inicial de $1V$ que llega desde el úlitmo al primero, sumando el voltaje de ciertos módulos. Dada una cadena conformada de $1$ y $0$ significando que Felipe toma o no el voltaje del amplificador $i$ determinar la suma final del voltaje.

## Entrada
Una cadena $S$ $(|S| = 10)$ conformada por $1$ o $0$ donde, si el caracter $S_i$ es igual a $1$ significa Felipe suma el voltaje del modulo $i$

## Salida

Un entero $X$ la suma total del voltaje.

## Ejemplo

### Entrada
```
0000000011
```
### Salida
```
3
```

### Entrada
```
0110011110
```
### Salida
```
414
```

### Entrada
```
0000010011
```
### Salida
```
19
```
### Entrada
```
1111111111
```
### Salida
```
1023
```

## Notas

- En el primer caso, el voltaje del último módulo es de $1V$ el penúltimo, entonces, otorga $2 * 1V = 2V$, siendo la suma final de $3V$.
- En el tercer caso, la suma de todos los voltajes son $512 + 256 + 128 + 64 + 32 + 16 + 8 + 4 + 2 + 1 = 1023$ siendo la suma del último al primer módulo.

## Temas identificados

## Propuesta de solución



## Implementación



```mermaid

```

### C++

```cpp

```
