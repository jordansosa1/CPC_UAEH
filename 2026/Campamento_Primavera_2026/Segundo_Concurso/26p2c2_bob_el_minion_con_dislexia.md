https://www.cpcjudge.com/problem/bobminiondislexia

# 26P2C2. Bob, el minion con dislexia

## Descripción
Bob, el pequeño minion, empezó a ir a la escuela con Agnes y aprendió a escribir textos en español. Escribe sobre perros, sobre zapatos, sobre árboles, sobre la Segunda Guerra Mundial, etc. Y un día, en la escuela le encomendaron hacer varios textos sobre la primavera, los cuales iba a presentar en cada una de sus clases.

Bob escribió el primero de sus textos y lo llevó a clase pero, cuando lo estaba leyendo (no habla español solo lo escribe), se dio cuenta que escribió mal varias palabras debido a la dislexia. Las palabras que escribió mal fueron:

- cilma por clima
- birsa por brisa
- calro por calor
- homirga por hormiga
- abrol por arbol

Como Bob no quiere pasar vergüenza de nuevo con un texto mal escrito, te pidió ayuda para que corrijas su próximo texto. Para corregir el texto de Bob, si una palabra coincide **exactamente** con alguna de las ya descritas, ésta deberá ser corregida.

Bob aún no aprende a escribir letras mayúsculas ni acentos, entonces **todo el texto está escrito en letras minúsculas y sin acentos**.

¿Puedes ayudar a Bob?

## Entrada
En la primera línea un entero $N$ $(1 \leq N \leq 100)$, la cantidad de líneas del texto de Bob.

En las siguientes $N$ líneas una cadena $C_i$ $(1 \leq |C_i| \leq 100)$, la $i-ésima$ línea del texto registrada.

Se garantiza que las cadenas no inician ni terminan con espacios. Las palabras de una cadena están separadas por espacios.

Después de leer $N$, escribe ```cin.ignore();```.

Para leer una línea de texto (texto con espacios) utiliza ```getline(cin, tu_variable_string);```.

## Salida
El texto de Bob corregido.

## Ejemplo

### Entrada
```
3
la homirga oh la homirgaa la quiero mucho
no se como le hace para soportar este calro
lo bueno es que puede vivir bajo un abrol
```
### Salida
```
la hormiga oh la homirgaa la quiero mucho
no se como le hace para soportar este calor
lo bueno es que puede vivir bajo un arbol
```

### Entrada
```
4
en mi casa hay un abrol grande
y una vez vi una ardilla en el
y cuando me acerque
se cayo
```
### Salida
```
en mi casa hay un arbol grande
y una vez vi una ardilla en el
y cuando me acerque
se cayo
```

### Entrada
```
3
las flores son bonitas
pero me gustan mas
los dorilocos con cueritos uf papoi
```
### Salida
```
las flores son bonitas
pero me gustan mas
los dorilocos con cueritos uf papoi
```

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
    cin.ignore();
    for (int i = 0; i < n; i++) {
        string r;
        string s;
        getline(cin, s);
        s.push_back(' ');
        string p;
        for (auto c : s) {
            if (c == ' ') {
                if (p == "cilma") {
                    p = "clima";
                }
                if (p == "birsa") {
                    p = "brisa";
                }
                if (p == "calro") {
                    p = "calor";
                }
                if (p == "homirga") {
                    p = "hormiga";
                }
                if (p == "abrol") {
                    p = "arbol";
                }
                for (auto cc : p) {
                    r.push_back(cc);
                }
                r.push_back(' ');
                p = "";
            } else {
                p.push_back(c);
            }
            
        }
        
        cout << r << '\n';
        
    }

    return 0;
}
```
