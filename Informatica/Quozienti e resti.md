# Moltiplicazione egizia
```
21  *  19
10  |  38 | via perché è pari
5   |  76
2   | 152 | via perché è pari
1   | 304
0   |

poi sommo
19 + 76 + 304 = 399 = 21*19
```

funziona perché è una moltiplicazione in base 2
```
21 | 1 |  1
10 | 0 |  2
5  | 1 |  4
2  | 0 |  8
1  | 1 | 16

Poi presi al contrario, dal basso all'alto, 10101
```
e poi
```
21 | 1 *  1 * 19
10 | 0 *  2 * 19 | numero pari -> *0
 5 | 1 *  4 * 19
 2 | 0 *  8 * 19 | numero pari -> *0
 1 | 1 * 16 * 19
```
# Algoritmo di Euclide
```
MCD(133, 91)     
|                | 133
|                |  91
133 %  91 =   42 |  42
 91 %  42 =    7 |   7 = MCD
 42 %   7 =    0 |   0
```
dividi sempre gli ultimi 2, e prendi il penultimo numero
e tra l'altro, ogni coppia è con MCD 7.