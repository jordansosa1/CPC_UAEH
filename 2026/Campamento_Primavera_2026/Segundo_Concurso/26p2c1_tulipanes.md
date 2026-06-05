https://www.cpcjudge.com/problem/tulipanes

# 26P2C1. Tulipanes

## Descripción
Hoy es $27$ de mayo y una rana profundamente enamorada cumple un mes más de noviazgo con su querida novia. Esta rana no tiene dinero, pero está dispuesta a hacer lo que sea por conseguir un detalle para celebrar este día.

Mientras iba de camino a la Universidad de las Ranas, se topó un invernadero cuya puerta estaba abierta...

La rana entró silenciosamente y analizó el perímetro, NO HABÍA NADIE!

Amapolas, Girasoles, Anturios, y más flores/plantas se encontraban en este enorme invernadero de $N$ filas por $M$ columnas, pero había una de interés especial para la rana, el Tulipán.

Su intención era **robar la mayor cantidad de Tulipanes** para regalar a su novia pero, a pesar de lo solitario de este lugar, era probable que pronto volviera un encargado, por lo que la rana debía darse prisa.

Para no demorar mucho, la rana decidió robar únicamente los Tulipanes de una columna, así que te pidió ayuda para que le indiques hacia que columna correr para robar **solo los Tulipanes** y después escapar.

## Entrada
En la primera línea dos enteros $N$ y $M$ $(1 \leq N, M \leq 100)$, la cantidad de filas y columnas respectivamente.

En las siguientes $N$ líneas, $M$ carácteres, donde:

- indica una flor
- indica una planta
- indica un tulipán
- indica un espacio vacío

## Salida
En caso de que no haya ningún Tulipán, deberás imprimir "Bro..." (sin comillas).

En caso contrario, imprimir dos enteros $C$ y $T$, la columna a la que debe ir y la cantidad de tulipanes que puede robar en dicha columna, respectivamente.
  
Si hay varias soluciones, imprimir la menor columna.

## Ejemplo

### Entrada
```
5 5
FFP..
T..T.
T...T
T.PPP
T.F..
```
### Salida
```
1 4
```

### Entrada
```
6 4
.P.T
...T
F.T.
PP..
..T.
FFPF
```
### Salida
```
3 2
```

### Entrada
```
3 7
FFP...F
P..F..F
....PPF
```
### Salida
```
Bro...
```

## Notas
En el primer caso, la rana debe robar los tulipanes de la primera columna, así conseguirá robar $4$ tulipanes.

Si la rana optara por la cuarta o quinta columna, solo robaría un tulipán.


En el segundo caso, la rana puede robar tanto en la tercera como en la cuarta columna, así conseguirá robar $2$ tulipanes en ambas.

Dadas las restricciones de la salida, la rana debe robar en la tercera columna.

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
