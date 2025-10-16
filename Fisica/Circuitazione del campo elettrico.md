# Caso statico
$$\Gamma _\gamma (\vec E) = 0$$
Nel caso statico, il campo elettrico che passa attraverso una linea $\gamma$ chiusa, non compie lavoro, perché il punto di partenza sarà lo stesso del punto di arrivo (essendo una linea chiusa), e il campo elettrico $\vec E$ è conservativo.
# Caso generale
$$\Gamma\gamma(\vec E_i) = \frac{L}{q}=fem=-\frac{\Delta\Phi(\vec B)}{\Delta t}$$
## Dimostrazione
Ogni volta che abbiamo un campo magnetico che varia nel tempo, questo genera un campo elettrico indotto, come dimostrato dalla [[Legge di Lenz]].

![[Campo elettromagnetico.excalidraw.svg]]
All'apertura/chiusura del circuito azzurro, verrà generata una [[Corrente indotta]] (che nel disegno produrrà una $\color{lightblue} \vec F_i$), che produrrà una variazione del campo magnetico e quindi la creazione di campo elettrico indotto $\color{green}\vec E_i$.
Il campo elettrico è definito come $\vec E=\frac{\vec F}{e^-}$.

![[Circuitazione del campo elettrico indotto.excalidraw.svg]]
Quindi, per la definizione di circuitazione varrà questa formula...
$$\Gamma\gamma(\vec E_i) = \sum_{k=1}^n\vec E_{ik}\cdot \vec {\Delta l_k}=E_{i1}\Delta l_1 + E_{i2}\Delta l_2\dots$$

Se moltiplichiamo da entrambi i lati per la carica $q$,
$$q\Gamma\gamma(\vec E_i) = q\sum_{k=1}^n\vec E_{ik}\cdot \vec {\Delta l_k}$$
Visto che $\vec E \cdot q = \vec F$, allora ci ritroveremo con $\vec F_{ik}\cdot \vec{\Delta l_k} = L_k$.
"la sommatoria di tutti i lavori è il lavoro totale $L$".
Quindi
$$q\Gamma\gamma(\vec E_i) = L$$
ovvero
$$\Gamma\gamma(\vec E_i) = \frac{L}{q}=fem=-\frac{\Delta\Phi(\vec B)}{\Delta t}$$