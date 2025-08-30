![[macchina-termica.png]]
==$Q_1$ è sempre negativo==.
L'efficenza di una macchina, espressa senza unità di misura, si calcola tramite la seguente formula:
$$\eta=\frac{L}{Q_2}=\frac{Q_2-|Q_1|}{Q_2}$$
$\eta$ è una lettera greca detta `eta`
$\eta$ non può essere $>$ di $1$ , altrimenti si andrebbe contro il [[2° Principio]]
Se $\eta$ fosse $=1$ allora sarebbe una macchina "anti - Kelvin".

In tutto ciò $Q_2$ è la sorgente calda  mentre $Q_1$ e quella fredda.

$$\eta=\frac{Q_2-|Q_1|}{Q_2} = \frac{Q_2}{Q_2}-\frac{|Q_1|}{Q_2} = 1 - \frac{|Q_1|}{Q_2}$$
Ed essendo $Q_1$ sempre diverso da $0$ ciò dimostra perchè $\eta < 1$.
In questo caso si può dimostrare che

$$\eta_r =1-\frac{|Q_1|}{Q_2} = 1 - \frac{T_1}{T_2}$$
$\eta_r$ indica l'efficenza nelle macchine reversibili.

> La macchina reversibile è una macchina che può far tornare la sostanza dallo stato finale allo stato iniziale.

# Rendimenti tra reversibile e irreversibile
Il rendimento di una macchina reversibile è $>$ di quello di una macchina irreversibile se esse lavorano con le stesse temperature:
$$\eta_s<\eta_r$$
con $\eta_s$ come l'efficacia di una macchina irreversibile.
Questa formula è data dal teorema di Carnot
## Dimostrazione per assurdo del teorema di Carnot
![[Dimostrazione-Carnot.png]]

Se $\eta_r < \eta_s$:

Immaginiamo di avere 2 macchine: R, S; che operano alle stesse temperature tra $T_2$ e $T_1$ ed estraggono entrambe $Q_2$.
$L=Q_2-|Q_1|$

R: $T_2 \to Q_2$ che produce $L^R$ e $-Q_1^R$. Quest'ultimo va dentro $T_1$.
S: $T_2 \to Q_2$ che produce $L^S$ e $-Q_1^S$. Quest'ultimo va dentro $T_1$.

$$L^R=Q_2-|Q_1^R|$$
$$L^S=Q_2-|Q_1^S|$$
Quindi
$$\eta^R=1-\frac{Q_1^R}{Q_2}$$
$$\eta^S=1-\frac{Q_1^S}{Q_2}$$
Sostituendo in $\eta^r<\eta^s$.
$$1-\frac{Q_1^R}{Q_2} > 1-\frac{Q_1^S}{Q_2} \to |Q_1^S|<|Q_1^R|$$
quindi:
$$Q_1^R - Q_1^S >0$$
La reversibile può essere invertita, e quindi ora diventa -R.
$$L_{tot}=L_S-L_R = Q_2-|Q_1^S|-(Q_2-|Q_1^R|) = -|Q_1^S|+|Q_1^R|$$
Ma, alla fine quindi avendo $L_{tot}=-|Q_1^S|+|Q_1^R|$ per averla non servono veramente 2 contenitori, quindi avendo 1 solo contenitore e creando lavoro è una macchina anti-kelvin.

Ciò quindi viola il principio di kelvin, quindi è assurdo e $\eta_R<\eta_S$ e quindi è vero il contrario: $\eta_R>\eta_S$.