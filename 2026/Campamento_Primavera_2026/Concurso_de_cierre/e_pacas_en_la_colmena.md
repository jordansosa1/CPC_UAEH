# C. Pacas en la colmena

## Descripción

Últimamente Honey ha notado que en su colmena hay un gran desorden de recursos, especialmente hay un gran desorden en la bodega donde hay unidades de ***cera*** y ***propóleo***, dos de los principales materiales de construcción de las abejas obreras, la organización de las abejas las ha llevado a formar una fila de materiales conforme fueron llegando a la bodega, sin embargo Honey ha concluido que una forma más conveniente de guardar estos recursos es colocándolos en pacas y a su vez.

Cada paca debe tener exactamente dos unidades de algún recurso, para lograr llevar un control sobre el almacenamiento Honey decidió que cada paca debe tener un sólo tipo de material guardado y para hacer más rápido el proceso de guardado ha planeado que un grupo de abejas le ayude a completar esta labor.

Honey quiere calcular cuántas pacas de ambos materiales podría empacar una abeja al ponerla en algún segmento de la fila de materiales y usar estos datos para planear mejor su estrategia de acomodado.

## Entrada
Un número $N$ $(2 \leq N \leq 10^6)$ que representa la cantidad de materiales que salieron por la banda y un número $Q$ $(1 \leq Q \leq 10^6)$ que representa la cantidad de segmentos en los que Honey quiere calcular.

Una línea con $N$ numeros $a_i$ $(a_i \in {1, 2})$ donde $a_i$ representa el tipo de material. $1$ ***para cera*** y 2 ***para propóleo***.

$Q$ líneas, cada una con dos números $l$ y $r$ $(1 \leq l &lt; r \leq N)$  que representan la posicion en que empieza el segmento y la posición en la que termina.

## Salida

$Q$ líneas, cada una con un número que represente la cantidad de pacas armadas en total en el rango especificado.

## Ejemplos

### Entrada
```
10 3
2 1 1 2 2 1 2 1 2 2 
1 10
3 6
8 9
```
### Salida
```
5
2
0
```

### Entrada
```
5 2
1 2 1 2 1
1 2
3 4
```
### Salida
```
0
0
```

## Notas
En el primer caso:
- En la primer prueba se consideró toda la secuencia de materiales con un total de $5$ pacas armadas ($2$ de cera y $3$ de propóleo)
- En la segunda prueba se consideró la secuencia {1, 2, 2, 1} por lo que se armó un total de $2$ pacas ($1$ de cera y $1$ de propóleo)
- En la tercera prueba se consideró la secuencia {1, 2} por lo que no se armó ninguna paca al no poder completar alguna.

## Temas identificados


## Propuesta de solución


## Implementación


### C++

