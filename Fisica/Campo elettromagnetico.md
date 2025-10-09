# Il campo elettrico indotto e la II equazione di Maxwell

Ogni volta che abbiamo un campo magnetico che varia nel tempo, questo genera un campo elettrico indotto.
![[Campo elettromagnetico.excalidraw.svg]]
$E=\frac{F}{e}$

Collegamento tra il campo magnetico e il campo elettrico
![[Campo elettrico e campo magentico.excalidraw.svg]]
![[Circuitazione del campo elettrico indotto.excalidraw.svg]]
$$\Gamma\gamma(\vec E_i) = \sum_{k=1}^n\vec E_{ik}\cdot \vec {\Delta l_k}=E_{i1}\Delta l_1 + E_{i2}\Delta l_2\dots$$
e moltiplicando da entrambi i lati
$$q\Gamma\gamma(\vec E_i) = q\sum_{k=1}^n\vec E_{ik}\cdot \vec {\Delta l_k}$$
$q$ si può spostare dentro, e moltiplicato per $\vec E _{ik}$ diventa $\vec F_{ik}$.
$\vec F_{ik}\cdot \vec{\Delta l_k} = L$.
"la sommatoria di tutti i lavori è il lavoro totale $L$".
Quindi
$$q\Gamma\gamma(\vec E_i) = L$$
ovvero
$$\Gamma\gamma(\vec E_i) = \frac{L}{q}=fem=-\frac{\Delta\Phi(\vec B)}{\Delta t}$$