In tutta questa pagina viene usato $n$ per indicare il numero di elementi in $k$ "cassetti".
# Risoluzione dei problemi

| Importa l'ordine? | Il numero di posti è uguale al numero di elementi? | Gli elementi si ripetono? | Nome                              |
| ----------------- | -------------------------------------------------- | ------------------------- | --------------------------------- |
| ✅                 | ✅                                                  | ✅                         | [[#Permutazioni con ripetizioni]] |
| ✅                 | ✅                                                  | ❎                         | [[#Permutazioni semplici]]        |
| ✅                 | ❎                                                  | ✅                         | [[#Disposizioni con ripetizioni]] |
| ✅                 | ❎                                                  | ❎                         | [[#Disposizioni semplici]]        |
| ❎                 | //                                                 | ✅                         | [[#Combinazioni con ripetizioni]] |
| ❎                 | //                                                 | ❎                         | [[#Combinazioni semplici]]        |

# Combinazioni
Ricordando che:
$$\binom{a}{b}=\frac{a!}{b!(a-b)!}$$
## Combinazioni semplici
$$C_{n,k}=\binom{n}{k}=\frac{n!}{k!(n-k)!}$$
## Combinazioni con ripetizioni
$$C^*_{n,k}=\binom{n+k-1}{k}=\frac{n+k-1!}{k!(n+k-1-k)!}=\frac{n+k-1!}{k!(n-1)!}$$
# Disposizioni
## Disposizioni semplici
$$D_{n,k}=\frac{n!}{(n-k)!}$$
## Disposizioni con ripetizioni
$$D^*_{n,k}=n^k$$
# Permutazioni
## Permutazioni semplici
$$P_n=n!$$
## Permutazioni con ripetizioni
$$P_n^*=\frac{n!}{a_1!\cdot a_2!\ldots a_n!}$$