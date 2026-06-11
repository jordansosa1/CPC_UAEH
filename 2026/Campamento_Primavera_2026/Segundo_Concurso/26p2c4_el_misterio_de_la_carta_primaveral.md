https://www.cpcjudge.com/problem/carlosysandroprimave

# 26P2C4. El Misterio de la Carta Primaveral

## Descripción
Durante las cálidas tardes de primavera, Sandro y Carlos aprovechan el clima para entrenar al aire libre. Sus días comienzan con horas de algoritmos y código, por lo que pronto terminan exhaustos. Para darle un descanso a sus mentes y disfrutar de la brisa primaveral bajo los árboles, les gusta jugar a las cartas en sus ratos libres.

El juego de cartas que inventaron funciona de la siguiente manera:

El valor de una carta se define por su primer carácter. Si muestra un dígito entre el $2$ y el $9$, ese es su valor. De lo contrario (cartas cuyo primer carácter es T, J, Q, K, A), su valor es $10$. Inicialmente, se tiene un mazo de $52$ cartas boca abajo.

- Toman las $25$ cartas superiores del mazo y las guardan en su mano.
- Establecen una variable $Y = 0$.
- Luego, ejecutan el siguiente proceso exactamente tres veces:
  - Toman la carta superior del mazo restante y determinan su valor. Sea $X$ el valor de esta carta.
  - Suman $X$ a $Y$.
  - Descartan esta carta junto con las siguientes $(10 - X)$ cartas de la parte superior del mazo.
- Finalmente, toman las $25$ cartas que tenían guardadas en la mano y las vuelven a colocar en la parte superior del mazo.

El objetivo del juego es determinar cuál es la $Y-ésima$ carta del mazo, contando desde abajo hacia arriba.

Sandro y Carlos conocen el orden inicial de las cartas antes de empezar, por lo que asumen que pueden deducir mentalmente cuál es la $Y-ésima$ carta sin mirar el mazo. Sin embargo, con el cansancio de la primavera, a menudo se equivocan. ¡Tu tarea es escribir un programa que encuentre la carta correcta por ellos!

## Entrada
En la primera línea un entero $Q$ $(1 \le Q \le 1000)$, el número de casos de prueba.

Cada caso de prueba consta de $52$ cartas separadas por espacios, representando el orden inicial del mazo **desde la parte inferior hasta la parte superior**.

El formato de cada carta es una cadena de $2$ caracteres: el primer carácter indica el valor ($2-9$, T, J, Q, K, A) y el segundo carácter indica el palo (C, D, H, S).

## Salida
Para cada caso de prueba, imprime la carta objetivo (la $Y-ésima$ carta desde la parte inferior).

## Ejemplo

### Entrada
```
2
AC KC QC JC TC 9C 8C 7C 6C 5C 4C 3C 2C AD KD QD JD TD 9D 8D 7D 6D 5D 4D 3D 2D AH KH QH JH TH 9H 8H 7H 6H 5H 4H 3H 2H AS KS QS JS TS 9S 8S 7S 6S 5S 4S 3S 2S
AC KC QC JC TC 9C 8C 7C 6C 5C 4C 3C 2C AD KD QD JD TD 9D 8D 7D 6D 5D 4D 3D 2D AH KH QH JH TH 9H 8H 7H 6H 5H 4H 3H 2H AS KS QS JS TS 9S 8S 7S 6S 5S 4S 3S 2S

```
### Salida
```
8H
8H
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

int main() {
    cin.tie(0); ios::sync_with_stdio(false);

	int q;
	cin >> q;

	for (int i = 0; i < q; i++) {
        for (int i = 1; i <= 52; i++) {
            string carta;
            cin >> carta;
            if (i == 33) {
                cout << carta << '\n';
            }
        }
	}
}
```

```cpp
#include <bits/stdc++.h>

using namespace std;

int main() {
    cin.tie(0); ios::sync_with_stdio(false);

	int q;
	cin >> q;

	for (int i = 0; i < q; i++) {
        int y = 0;
        vector<string> mazo;
        for (int j = 1; j <= 27; j++) {
            string s;
            cin >> s;
            mazo.push_back(s);
        }
        for (int j = 0; j < 3; j++) {
            int num = mazo.back()[0] == 'A' ||
                           mazo.back()[0] == 'J' ||
                           mazo.back()[0] == 'K' ||
                           mazo.back()[0] == 'Q' ||
                           mazo.back()[0] == 'T'? 10 : mazo.back()[0] - '0';
            for (int k = 1; k <= 11 - num; k++) {
                mazo.pop_back();
            }
            y += num;
        }
        for (int j = 1; j <= 25; j++) {
            string s;
            cin >> s;
            mazo.push_back(s);
        }
        cout << mazo[y - 1] << '\n';
	}
}
```
