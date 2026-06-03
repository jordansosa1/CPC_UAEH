https://www.cpcjudge.com/problem/stuartminiondislexia

# M. Stuart, el otro minion con dislexia

## Descripción
Stuart, el hermano de Bob, empezó a ir a la misma escuela que él y aprendió a escribir textos en español. Como le dejaban la misma tarea que Bob, debía hacer varios textos sobre la primavera.

Stuart escribió el primero de sus textos y fue más inteligente que Bob, porque prefirió revisar sus textos antes de llevarlos a clase, sin embargo, resultó que Stuart escribe peor que Bob...

Stuart posee una dislexia severa, esto significa que no tiene errores mínimos, sino que reorganiza las letras de una palabra de forma aleatoria. Las palabras que Stuart escribe mal son las siguientes:

- nube
- queso
- libro
- mesa
- lapiz

Por ejemplo, si Stuart quiere escribir nube, puede escribir "nube", "unbe", "enbu", "uenb", etc... En todos esos casos, deberás corregirlo a "nube".

Así con las demás palabras que escribe mal.

Como Stuart no quiere pasar vergüenza presentando un texto mal escrito, te pidió ayuda para que corrijas su próximo texto.

Stuart tampoco ha aprendido a escribir letras mayúsculas ni acentos, entonces **todo el texto está escrito en letras minúsculas y sin acentos**.

¿Puedes ayudar a Stuart? 😈

## Entrada
En la primera línea un entero $N$ $(1 \leq N \leq 100)$, la cantidad de líneas del texto de Stuart.

En las siguientes $N$ líneas una cadena $C_i$ $(1 \leq |C_i| \leq 100)$, la $i$-$ésima$ línea del texto registrada.

Se garantiza que las cadenas no inician ni terminan con espacios. Las palabras de una cadena están separadas por espacios.

Después de leer $N$, escribe ***cin.ignore();***.
Para leer una línea de texto (texto con espacios) utiliza ***getline(cin, tu_variable_string)***;.

## Salida
El texto de Stuart corregido.

## Ejemplos

### Entrada
```
2
bob te quiero pero
me perdiste mi lpiza
```
### Salida
```
bob te quiero pero
me perdiste mi lapiz
```

### Entrada
```
4
bob mi lapiz donde esta
quiero mi pizla por favor
tengo que contestar mi birlo
de ingles bro
```
### Salida
```
bob mi lapiz donde esta
quiero mi lapiz por favor
tengo que contestar mi libro
de ingles bro
```

### Entrada
```
4
deje el sequo sobre la sema
y mi orlib en la silla
ahora no encuentro mi ueoqs
ni mi ibrol ni mi silla
```
### Salida
```
deje el queso sobre la mesa
y mi libro en la silla
ahora no encuentro mi queso
ni mi libro ni mi silla
```

## Temas identificados
- Ciclos
- Manejo de cadenas
- Condicionales

## Propuesta de solución


## Implementación

### C++

```cpp
#include <iostream>
#include <bits/stdc++.h>

using namespace std;

int main() {
    cin.tie(0); ios::sync_with_stdio(false);
    
    int num;
    cin >> num;
    cin.ignore();

    for (int k = 0; k < num; k++) {
        string frase;
        getline(cin, frase);
        frase.push_back(' ');
        string resultado = "";
        string palabra = "";

        int n = 0, u = 0, b = 0, e = 0, q = 0, s = 0, o = 0, l = 0, i = 0, r = 0, m = 0, a = 0, p = 0, z = 0;

        for (char c : frase) {
            switch(c) {
                case ' ':
                    if (n == 1 && u == 1 && b == 1 && e == 1 && palabra.length() == 4) {
                        palabra = "nube";
                    }
                    if (q == 1 && u == 1 && e == 1 && s == 1 && o == 1 && palabra.length() == 5) {
                        palabra = "queso";
                    }
                    if (l == 1 && i == 1 && b == 1 && r == 1 && o == 1 && palabra.length() == 5) {
                        palabra = "libro";
                    }
                    if (m == 1 && e == 1 && s == 1 && a == 1 && palabra.length() == 4) {
                        palabra = "mesa";
                    }
                    if (l == 1 && a == 1 && p == 1 && i == 1 && z == 1 && palabra.length() == 5) {
                        palabra = "lapiz";
                    }
                    resultado += palabra + " ";
                    
                    n = 0, u = 0, b = 0, e = 0, q = 0, s = 0, o = 0, l = 0, i = 0, r = 0, m = 0, a = 0, p = 0, z = 0;
                    palabra = "";
                    break;
                case 'n':
                    palabra.push_back(c);
                    n++;
                    break;
                case 'u':
                    palabra.push_back(c);
                    u++;
                    break;
                case 'b':
                    palabra.push_back(c);
                    b++;
                    break;
                case 'e':
                    palabra.push_back(c);
                    e++;
                    break;
                case 'q':
                    palabra.push_back(c);
                    q++;
                    break;
                case 's':
                    palabra.push_back(c);
                    s++;
                    break;
                case 'o':
                    palabra.push_back(c);
                    o++;
                    break;
                case 'l':
                    palabra.push_back(c);
                    l++;
                    break;
                case 'i':
                    palabra.push_back(c);
                    i++;
                    break;
                case 'r':
                    palabra.push_back(c);
                    r++;
                    break;
                case 'm':
                    palabra.push_back(c);
                    m++;
                    break;
                case 'a':
                    palabra.push_back(c);
                    a++;
                    break;
                case 'p':
                    palabra.push_back(c);
                    p++;
                    break;
                case 'z':
                    palabra.push_back(c);
                    z++;
                    break;
                default:
                    palabra.push_back(c);
                    break;
            }
        }
        cout << resultado << '\n';
    }

    return 0;
}
```
