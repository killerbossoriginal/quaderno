# Funzioni goniometriche
![[Funzioni goniometriche.png]]

|        | Seno                       | Coseno                     | Tangente                             |
| ------ | -------------------------- | -------------------------- | ------------------------------------ |
|        | $\sin \alpha = y_p$        | $\cos \alpha = x_p$        | $\tan \alpha = \frac{y_p}{x_P}$      |
| quindi | $-1 \le \sin \alpha \le 1$ | $-1 \le \cos \alpha \le 1$ | $-\infty \le \tan \alpha \le \infty$ |
I valori notevoli sono quelli degli angoli principali

| Misura   | $0°$ | $30°$                | $45°$                | $60°$                | $90°$ | $180°$ | $270°$ |
| -------- | ---- | -------------------- | -------------------- | -------------------- | ----- | ------ | ------ |
| Seno     | $0$  | $\frac{1}{2}$        | $\frac{\sqrt{2}}{2}$ | $\frac{\sqrt{3}}{2}$ | $1$   | $0$    | $-1$   |
| Coseno   | $1$  | $\frac{\sqrt{3}}{2}$ | $\frac{\sqrt{2}}{2}$ | $\frac{1}{2}$        | $0$   | $-1$   | $0$    |
| Tangente | $0$  | $\frac{\sqrt{3}}{3}$ | $1$                  | $\sqrt{3}$           | ?     | $0$    | ?      |
## Relazioni fondamentali
**Prima relazione fondamentale**:
$$
\sin^2\alpha+\cos^2\alpha=1
$$
**Seconda relazione fondamentale**:
$$
\tan\alpha=\frac{\sin\alpha}{\cos\alpha}
$$
e ne conseguono quindi:
$$\cos\alpha=\pm\frac{1}{\sqrt{1+\tan^2\alpha}}$$
e
$$\sin\alpha=\pm\frac{|\tan{\alpha}|}{\sqrt{1+\tan^2{\alpha}}}$$
## Proprietà


| Relazione                        | Seno                                    | Coseno                                  | Tangente                                          | Immagine                                             |
| -------------------------------- | --------------------------------------- | --------------------------------------- | ------------------------------------------------- | ---------------------------------------------------- |
| Angoli supplementari             | $sin(\pi-\alpha)=sin\alpha$             | $cos(\pi-\alpha) = -\cos\alpha$         | $\tan(\pi-\alpha)=-\tan\alpha$                    | ![[Goniometria - Angoli supplementari.png]]          |
| Angoli che differiscono di $\pi$ | $\sin(\pi+\alpha)=-\sin\alpha$          | $\cos(\pi+\alpha)=-\cos\alpha$          | $\tan(\pi+\alpha)=\tan\alpha$                     | ![[Goniometria - Angoli che differiscono di pi.png]] |
| Angoli opposti                   | $\sin(-\alpha)=-\sin\alpha$             | $\cos(-\alpha)=\cos\alpha$              | $\tan(-\alpha)=-\tan(\alpha)$                     | ![[Goniometria - Angoli opposti.png]]                |
| Angoli complementari             | $\sin(\frac{\pi}{2}-\alpha)=\cos\alpha$ | $\cos(\frac{\pi}{2}-\alpha)=\sin\alpha$ | $\tan(\frac{\pi}{2}-\alpha)=\frac{1}{\tan\alpha}$ | ![[Goniometria - Angoli complementari.png]]          |
# Formule goniometriche

|                                                        | Seno                                                             | Coseno                                                                                               | Tangente                                                                                                                        |
| ------------------------------------------------------ | ---------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- |
| Addizione e sottrazione                                | $\sin(\alpha\pm\beta)=\sin\alpha\cos\beta\pm\cos\alpha\sin\beta$ | $\cos(\alpha\pm\beta)=\cos\alpha\cos\beta\mp\sin\alpha\sin\beta$                                     | $\tan(\alpha\pm\beta)=\frac{\tan\alpha\pm\tan\beta}{1\mp\tan\alpha\tan\beta}$                                                   |
| Duplicazione                                           | $\sin2\alpha=2\sin\alpha\cos\alpha$                              | $\cos2\alpha=\cos^2\alpha-\sin^2\alpha=\begin{cases} 1-2\sin^2\alpha \\ 2\cos^2\alpha-1 \end{cases}$ | $\tan2\alpha=\frac{2\tan\alpha}{1-\tan^2\alpha}$                                                                                |
| Bisezione                                              | $\sin\frac{\alpha}{2}=\pm\sqrt\frac{1-\cos\alpha}{2}$            | $\cos\frac{\alpha}{2}=\pm\sqrt\frac{1+\cos\alpha}{2}$                                                | $\tan\frac{\alpha}{2}=\pm\sqrt\frac{1-\cos\alpha}{1+\cos\alpha}=\frac{1-cos\alpha}{\sin\alpha}=\frac{\sin\alpha}{1+\cos\alpha}$ |
| Formule parametriche<br>(con $t=\tan\frac{\alpha}{2}$) | $\sin\alpha=\frac{2t}{1+t^2}$                                    | $\cos\alpha=\frac{1-t^2}{1+t^2}$                                                                     | $\tan\alpha=\frac{2t}{1-t^2}$                                                                                                   |
# Valori e soluzioni

| equazione   | $m<-1$          | $-1\le m\le1$                              | $m>1$           | valore              |
| ----------- | --------------- | ------------------------------------------ | --------------- | ------------------- |
| $\sin(x)=m$ | $\not\exists$   | $x=\alpha + 2k\pi \lor x=\pi-\alpha+2k\pi$ | $\not\exists$   | $\alpha=\arcsin(m)$ |
| $\cos(x)=m$ | $\not\exists$   | $x=\pm\alpha+2k\pi$                        | $\not\exists$   | $\alpha=\arccos(m)$ |
| $\tan(x)=m$ | $x=\alpha+k\pi$ | $x=\alpha+k\pi$                            | $x=\alpha+k\pi$ | $\alpha=\arctan(m)$ |
per le equazioni goniometriche di II grado, sostituisci i seni al quadrato con una lettera temporanea, risolvi l'equazione e poi risolvi con i valori la lettera.
# Equazioni goniometriche
$f(x)=$ qualsiasi funzione con risultato appartenente a $\mathbb{R}$
$h(x)=$ qualsiasi funzione con risultato appartenente a $\mathbb{R}$
$g(x)=(\cos(x)\lor \sin(x) \lor \tan(x))$
## Equazioni elementari

$$\sin(x)=m$$
$$
S=
\begin{cases}
	x \notin \mathbb{R} & \mbox{con} \quad y < -1 \lor y > 1 \\
	x = \arcsin(x) + 2k\pi \lor \pi - \arcsin(x)+2k\pi & \mbox{con} \quad-1 < y < 1 \\
	x=\pm \frac{\pi}{2}+2k\pi & \mbox{con} \quad y=\pm1 \\
	x = k\pi & \mbox{con} \quad y=0
\end{cases}
$$
$$\cos(x)=m$$
$$
S=
\begin{cases}
	x \notin \mathbb{R} & \mbox{con} \quad y < -1 \lor y > 1 \\
	x = \pm \arccos(x) + 2k\pi & \mbox{con} \quad-1 < y < 1 \\
	x=\pm \pi + 2k \pi & \mbox{con} \quad y=\pm1 \\
	x = \frac{\pi}{2} + 2k\pi & \mbox{con} \quad y=0
\end{cases}
$$
$$\tan(x)=m \to x = \arctan(x) + k\pi \quad \forall m \in \mathbb{R}$$

## Equazioni elementari con funzioni
$$g(f(x))=m$$
La risoluzione può avvenire rimpiazzando $x$ con $f(x)$ nel processo risolutivo.
## Equazioni elementari tra funzioni goniometriche
$$g(f(x))=g(h(x))$$
La risoluzione può avvenire rimpiazzando $arcg(x)$ con di $h(x)$ nel processo risolutivo.
## Risoluzione
1. E' elementare? [[#Equazioni elementari]]
2. E' di secondo grado? Rimpiazza con $t$ la funzione al quadrato, risolvi con la [[Equazioni di II grado#Formula risolutiva]].
3. Prova a ricondurla ad elementare tramite:
	1. le formule delle [[#Relazioni fondamentali]].
	2. le [[#Formule goniometriche]].
	3. dividendo per $\cos$. (ad esempio $a\sin(x)+b\cos(x)=0 \to a\tan(x)+b=0$)
4. Se sono lineari complete ($a\sin(x)+b\cos(x)+c=0$) risolvi tramite uno dei seguenti metodi:
	1. Metodo grafico (rimpiazza $\sin(x)=X$ e $\cos(x)=Y$, e poi metti a sistema $\begin{cases} eq \\ X^2+Y^2=0 \end{cases}$)
	2. Metodo algebrico (utilizza le [[#Formule goniometriche|formule parametriche con t]] e poi risolvi per t.)
	3. Angolo aggiunto ($A=\sqrt{a^2+b^2} \to \exists\gamma | \cos(\gamma)=\frac{a}{A}\lor\sin(\gamma)=\frac{b}{A} \to A\sin(x+\gamma)+c=0$)
5. Se sono omogenee ($a \sin^2(x)+b\sin(x)\cos(x)+c\cos^2(x)+d=0$)
	1. Fai sparire $d$ con questo trucchetto: $d=d\cdot1=d(\sin^2(x)+\cos^2(x)$
	2. raccogli e utilizza l'annullamento dei prodotti, (se $a=0\lor c=0$),
	3. dividi per $cos^2(x)$ e poi utilizza la [[#Risoluzione]] di 2° grado della tangente.