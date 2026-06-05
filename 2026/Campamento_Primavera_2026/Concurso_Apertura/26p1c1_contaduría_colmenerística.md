https://www.cpcjudge.com/problem/contadorabeja

# 26P1C1. Contaduría colmenerística

## Descripción
Desde que empezó la primavera las abejas han andado de aquí para allá, hay mucho trabajo por hacer y casi no hay tiempo para descansar, pero están bien con eso. Sin embargo hay una de ellas que no está del todo a gusto, la abeja reina. Hay tanta miel en la colmena que ya no hay espacio para las abejas e incluso se fuga de los contenedores donde se guarda y es necesario ampliar el espacio o construir una nueva colmena para expandir sus capacidades de almacenamiento.

Claro que no todo es tan fácil, aunque es la reina, el mundo ha empezado a cambiar y las abejas han formado un concejo que representa la opinión de todas las abejas, y no sólo eso, ahora votan en conjunto para aprobar o rechazar las decisiones de la reina, incluida la decisión sobre mover la miel excedente a un nuevo lugar, por lo que tiene que esperar a su aprobación. Ahora el concejo solicita una auditoría contable para contar la miel que ha ingresado a los almacenes y la miel con la que se cuenta antes de su traslado y así evitar malentendidos. Por ello, la abeja contadora está en apuros, ayúdale a ver que todo esté en orden!

Honey es la abeja encargada de esta auditoría y, aunque es muy lista, esta tarea la rebasa. Necesita darle resultados al concejo antes de que la miel siga aumentando y toda la colmena esté inundada en ella. Además, entre tanto alboroto y tanta miel, es probable que alguien haya robado parte de las reservas del reino, o incluso que se haya ingresado miel sin reportar, por lo que tiene que saber si falta miel, sobra, o todo está en orden. Afortunadamente Honey cuenta con los registros de la miel que ha sido ingresada a los almacenes y la cantidad de ésta, pero aún falta comprobar la coherencia de lo registrado con la miel que se tiene.

## Entrada
En la primera línea un número flotante $C$ $(0 \lt C \leq 10^5)$ que indica la cantidad de miel almacenada.

En la segunda línea un número entero $N$ $(1 \leq N \leq 10^6)$ que indica la cantidad de registros de ingreso de miel.

En la tercera línea $N$ números flotantes $a_i$ $(0 \lt a_i \leq 10^5)$ separados por un espacio que indican la cantidad de miel ingresada en esa ocasión.

## Salida
Imprime un número $F$ que indique la diferencia entre los registros de miel y la cantidad de miel existente.

La respuesta será considerada correcta si su error absoluto o relativo no excede $10^{-6}$

Para imprimir la respuesta con $6$ decimales, debes:

- Agregar la librería ```<iomanip>```
- Imprimir la respuesta así ```cout << fixed << setprecision(6) << respuesta;```

## Ejemplo

### Entrada
```
10.65
2
6.7 4
```
### Salida
```
0.05
```
### Entrada
```
190.345
8
6 25 32 12 27 0.4 19.6 8
```
### Salida
```
-60.345
```
### Entrada
```
53.123456
2
0.123456 53
```
### Salida
```
0.0
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
