
https://www.cpcjudge.com/problem/comidaapuros

# I. Comida en apuros

## Descripción
La primavera ha llegado a nuestro lado del mundo y con ella ha empezado esa época en la que solemos ver a la naturaleza renovarse y vemos cosas maravillosas como plantas floreciendo, abejas polinizando intensamente, muchos animales empezando a criar y algunos otros despiertan de un largo descanso.
Lamentablemente, no son todo maravillas y es que la comida se echa a perder más rápido, adquiere mal sabor, mal olor, las bacterias se reproducen mucho más rápido debido al calor y hasta crece moho. Afortunadamente alguien, el señor doctor profesor Bactriperr tiene un solución para todos estos problemas! o bueno, al menos uno de ellos.

Tras observar mucho tiempo la descomposición de la comida ha descubierto un patrón en el crecimiento de las colonias de moho y ahora necesita de tu ayuda para seguir desarrollando una solución a esto.

Bactriperr ha desarrollado un compuesto casi maravilloso capaz de acabar con todo tipo de moho y las sustancias dañinas que producen al mismo tiempo, aunque por el momento sólo funciona en líquidos y al mezclarse. Es un gran avance, el único problema es que tiene que ser aplicado en dosis demasiado exactas, poca cantidad de esta sustancia podría hacer que el moho genere resistencia y un exceso podría afectar negativamente a la comida. Bactriperr te ha contado lo mucho que le cuesta seguir el crecimiento del moho y como gran amigo y programador que eres te ofreces a desarrollar una solución que le diga **cuánto ha crecido el moho** después de cierto tiempo, así que te dice los detalles del crecimiento:

1. Una colonia puede estar compuesta de esporas, hifas jóvenes e hifas maduras al mismo tiempo.
2. Siempre aparece **una sóla** hifa joven **al inicio** de la contaminación, en el primer segundo.
3. Las **esporas se vuelven hifas jovenes al pasar un segundo**.
4. Las **hifas jovenes se vuelven hifas maduras al pasar un segundo**.
5. Cada hifa madura suelta una sola espora cada segundo** (incluído el segundo en el que madura).

Podemos determinar el **tamaño de una colonia de moho al sumar la cantidad de esporas, hifas jóvenes e hifas maduras** que hay en cierto momento.

Es una pena que aún tengamos que guardar los alimentos en el refrigerador, pero dejemos al señor doctor profesor trabajar, seguro con tu ayuda pronto resolverá este problema.

## Entrada

Un sólo número $S$ $(1 \leq S \leq 90)$ que indica el segundo en el que Bactriperr quiere obtener el tamaño de la colonia.

## Salida

Un sólo número $T$ que indica el tamaño de la colonia en el momento dado.

## Ejemplos

### Entrada
```
2
```
### Salida
```
2
```

### Entrada
```
3
```
### Salida
```
3
```

### Entrada
```
43
```
### Salida
```
701408733
```

## Notas

- En el primer ejemplo el resultado es $2$ debido a que en el primer segundo habia una hifa joven, en el siguiente segundo se convirtio en hifa madura y en el mismo segundo suelta una espora, por lo que el tamaño de la colonia es de $2$, la espora y la hifa madura.
- En el segundo ejemplo el resultado es $3$ retomando el segundo $2$ del primer ejemplo, la espora se convierte en hifa joven, y la hifa madura suelta una espora, por lo que el tamaño de la colonia es de $3$, la hifa madura, la hifa joven y la nueva espora.

## Temas identificados


## Propuesta de solución


```mermaid

```

### C++

```cpp

```
