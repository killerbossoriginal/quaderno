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
| Somma e sottrazione                                    | $\sin(\alpha\pm\beta)=\sin\alpha\cos\beta\pm\cos\alpha\sin\beta$ | $\cos(\alpha\pm\beta)=\cos\alpha\cos\beta\mp\sin\alpha\sin\beta$                                     | $\tan(\alpha\pm\beta)=\frac{\tan\alpha\pm\tan\beta}{1\mp\tan\alpha\tan\beta}$                                                   |
| Duplicazione                                           | $\sin2\alpha=2\sin\alpha\cos\alpha$                              | $\cos2\alpha=\cos^2\alpha-\sin^2\alpha=\begin{cases} 1-2\sin^2\alpha \\ 2\cos^2\alpha-1 \end{cases}$ | $\tan2\alpha=\frac{2\tan\alpha}{1-\tan^2\alpha}$                                                                                |
| Bisezione                                              | $\sin\frac{\alpha}{2}=\pm\sqrt\frac{1-\cos\alpha}{2}$            | $\cos\frac{\alpha}{2}=\pm\sqrt\frac{1+\cos\alpha}{2}$                                                | $\tan\frac{\alpha}{2}=\pm\sqrt\frac{1-\cos\alpha}{1+\cos\alpha}=\frac{1-cos\alpha}{\sin\alpha}=\frac{\sin\alpha}{1+\cos\alpha}$ |
| Formule parametriche<br>(con $t=\tan\frac{\alpha}{2}$) | $\sin\alpha=\frac{2t}{1+t^2}$                                    | $\cos\alpha=\frac{1-t^2}{1+t^2}$                                                                     | $\tan\alpha=\frac{2t}{1-t^2}$                                                                                                   |

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