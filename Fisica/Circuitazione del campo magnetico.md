![[Dimostrazione IV equazione di Maxwell.excalidraw.svg]]
Proviamo in 3 punti diversi a misurare la circuitazione del campo magnetico.
$${\color{Red}\Gamma_{\gamma_1}(\vec B)=\mu_0i}$$
$${\color{Green}\Gamma_{\gamma_2}(\vec B)=0}$$
$${\color{LightBlue}\Gamma_{\gamma_3}(\vec B)=?}$$
Nel punto $\color{red} \gamma_1$ è facile, e si utilizza la formula statica.
Nel punto $\color{green} \gamma_2$ non esiste il filo, quindi non c'è corrente e quindi non è presente circuitazione.
Nel punto $\color{lightblue} \gamma_3$ non sappiamo come calcolarla.


Però in ${\color{green}\gamma_2}$ si crea una corrente $i_s$ "corrente di spostamento", in modulo uguale a $i$ in cui tutte le molecole presenti tra le piastre del condensatore si polarizzano.
Quindi..
$${\color{Green}\Gamma_{\gamma_2}(\vec B)=\mu_0i_s}$$
e quindi nel punto $\color{lightblue} \gamma_3$ passerà una corrente tra il filo e l'interno del condensatore, che sarà uguale a $i$, perciò
$${\color{LightBlue}\Gamma_{\gamma_3}(\vec B)=\mu_0i_s=\mu_0i}$$
(in questo caso è corretto usare entrambe le correnti).

Proviamo a calcolare $i_s$, tramite le formule dei condensatori.
$$E=\frac{\sigma}{\epsilon_0}=\frac{\Delta Q}{S\cdot \epsilon_0}$$
ovvero
$$
\Delta Q=\Delta E\cdot S \cdot \epsilon_0=\Delta\Phi(\vec E) \cdot \epsilon_0
$$
e quindi
$$i_s=\frac{\Delta Q}{\Delta t}=\frac{\Delta\Phi(\vec E)\cdot \epsilon_0}{\Delta t}$$
