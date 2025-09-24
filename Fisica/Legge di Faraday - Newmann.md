$$i_i=\frac{1\cdot\Delta \Phi(\vec B)}{R\cdot\Delta T}$$

($i\downarrow i = \Delta\Phi(\vec B) \cdot (R\Delta T)\uparrow(-1)$)

Con $i_i$ corrente indotta nel filo.
# Dimostrazione
![[Dimostrazione legge di Faraday - Newmann.png]]
Partendo dal flusso del campo $\vec B$ dentro la superfice racchiusa tra la barra in movimento e il filo, possiamo dire che:
$$\Phi_i(\vec B)=\vec B\cdot \vec n \cdot S_i$$
con $\vec n$ vettore normale alla superfice iniziale $S_i$ e $\vec B$ campo magnetico parallelo a $\vec n$.
Allora si può trovare che $\Phi_i(\vec B) = B \cdot n \cdot \cos(0) \cdot S_i$
ovvero $$\Phi_i(\vec B) = B\cdot S_i $$
Con lo stesso ragionamento allora si può trovare che $$\Phi_f(\vec B)=B\cdot S_f$$

Allora unendoli entrambi $\Delta \Phi (\vec B) = \Phi_f (\vec B) - \Phi_i (\vec B) =B\cdot S_f - B \cdot S_i = B (S_f - S_i).$
Ma visto che stiamo cercando l'area coperta dalla barra in movimento, $S_f - S_i = l\cdot v\Delta t$, e sarà un risultato negativo, visto che si sta rimpicciolendo l'area.
Raggruppando i pezzi, quindi: $\Delta \Phi (\vec B) = -B \cdot l \cdot v \Delta t$, e quindi:
$$\frac{\Delta \Phi (\vec B)}{\Delta t}=-Blv$$

Però $-Blv$, può anche essere preso dal seguente ragionamento:
Il lavoro $L = \vec F_l \cdot \vec l = |e^-| v B \cdot l \cdot \cos \alpha$, con $\cos\alpha=0$
$fem = \frac{L}{e^-}=\frac{e^- \cdot vB \cdot l}{e^-} = Blv$

allora sarà che:
$$fem = -\frac{\Delta \Phi (\vec B)}{\Delta t}$$
però $fem = i*R$, allora 
$$i=-\frac{\Delta \Phi (\vec B)}{R\cdot\Delta t}$$