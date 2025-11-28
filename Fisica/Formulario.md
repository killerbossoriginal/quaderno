# Elettrostatica

| Formula                      | Nome                  |
| ---------------------------- | --------------------- |
| $$i=\frac{V}{R}$$            | Intensità di corrente |
| $$[\Omega] = [A] \cdot [V]$$ | Ohm                   |
# Elettromagnetismo
## Campo elettrico
| Formula                          | Nome                               |
| -------------------------------- | ---------------------------------- |
| $$\vec E = \frac{\vec F_l}{q}$$  | Campo elettrico                    |
| $$E= {\sigma \over \epsilon_0}$$ | Campo elettrico di un condensatore |

## Campo magnetico

| Formula                          | Nome                        |
| -------------------------------- | --------------------------- |
| $$B = \frac{\mu_0 I_d}{2\pi r}$$ | [[Legge di Ampère-Maxwell]] |

| Formula                                                                                                                                                  | Nome                                                                                                   |
| -------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------ |
| $$B=\mu_0i\frac{N}{l}$$                                                                                                                                  | Campo magnetico in un solenoide                                                                        |
| $$\vec F = i \vec l \times \vec B$$                                                                                                                      | [[Legge di Faraday]] (un filo)                                                                         |
| $$\vec F_l = q \cdot \vec V \times \vec B = i \cdot l \cdot B$$                                                                                          | Forza di Lorentz                                                                                       |
| $$i_i=-\frac{1\cdot\Delta \Phi(\vec B)}{R\cdot\Delta t}$$                                                                                                | [[Legge di Faraday - Neumann]]                                                                         |
| $$fem=\frac{L}{e^-}=-\frac{\Delta \Phi (\vec B)}{\Delta t}=i\cdot R=vlB$$                                                                                | Forza elettromotrice                                                                                   |
| $$i_s=\epsilon_0\frac{\Delta\Phi_s(\vec E)}{\Delta t}$$                                                                                                  | Corrente di spostamento ($[A]$)                                                                        |
| $$\Phi (\vec E) = \frac{Q}{\epsilon _0}$$                                                                                                                | I [[Equazioni di Maxwell]], ovvero il<br>[[Teorema di Gauss]]                                          |
| $$\Gamma _\gamma (\vec E) = 0$$                                                                                                                          | II [[Equazioni di Maxwell]] nel caso statico<br>*[[Circuitazione del campo elettrico#Caso statico]]*   |
| $$\Gamma\gamma(\vec E_i) = \frac{L}{q}=fem=-\frac{\Delta\Phi(\vec B)}{\Delta t}$$                                                                        | II [[Equazioni di Maxwell]] nel caso generico<br>*[[Circuitazione del campo elettrico#Caso generale]]* |
| $$\Phi (\vec B)=0$$                                                                                                                                      | III [[Equazioni di Maxwell]], ovvero il<br>[[Teorema di Gauss per il campo magnetico]]                 |
| $$\Gamma _\gamma (\vec B) = \mu_0i$$                                                                                                                     | IV [[Equazioni di Maxwell]] nel caso statico, ovvero il<br>[[Teorema di Ampère]]                       |
| $$\Gamma_\gamma(\vec B)={\color{red}\mu_0i}+{\color{green}\mu_0i_s}=\mu_0({\color{red}i}+{\color{green}\epsilon_0\frac{\Delta\Phi(\vec E)}{\Delta t}})$$ | IV [[Equazioni di Maxwell]] nel caso generico<br>*[[Circuitazione del campo magnetico]]*               |
| $$F=q(\vec E + \vec v \times \vec B)$$                                                                                                                   | Forza su una carica all'interno di un campo elettromagnetico                                           |
# Moto armonico

| Formula                     | Nome |
| --------------------------- | ---- |
| $$B=B_0 \sin(\omega t-kx)$$ |      |
| $$E=E_0 \sin(\omega t-kx)$$ |      |

# Luce e Onde

| Formula                                                               | Nome                                                                                              |
| --------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- |
| $$E=c\cdot B$$                                                        | Rapporto tra campo elettrico e campo magnetico (moduli)                                           |
| $$w_{\vec E} = {\epsilon_0E^2 \over 2}$$                              | Densità volumica di energia del campo elettrico                                                   |
| $$w_{\vec B} = {B^2 \over 2\mu_0}$$                                   | Densità volumica di energia del campo magnetico                                                   |
| $$w = w_{\vec E}+w_{\vec B} = \epsilon_0E^2$$                         | Densità volumica di un onda elettromagnetica                                                      |
| $$\overline{w}={\epsilon_0 E^2_0 \over 2} \left[J \over m^3 \right]$$ | Densità volumica media di energia                                                                 |
| $$E_r=c\overline{w} \left[{W\over m^2}\right]$$                       | irradiamento                                                                                      |
| $$\Delta p = {E_r \over c}$$                                          | Quantità di moto                                                                                  |
| $$F_r={\Delta p \over \Delta t}$$                                     | Forza di irradiazione                                                                             |
| $$E_r=E^i_r\cdot \cos^2(\alpha)$$                                     | Irradiamento dopo la polarizzazione, ad eccezione del primo caso in cui è sempre $E_r^i \over 2$. |

# Generiche

| Formula                                    | Nome                                                                                            |
| ------------------------------------------ | ----------------------------------------------------------------------------------------------- |
| $$\Phi(\vec X)=\vec X\cdot \vec S$$        | Flusso di un campo $\vec X$ ($\vec S = \vec n \cdot S$ con $\vec n$ normale alla superfice $S$) |
| $$\Gamma_\gamma(\vec X) = \vec X \cdot l$$ | Circuitazione di un campo $\vec X$.                                                             |


| Formula                   | Nome   |
| ------------------------- | ------ |
| $$L=\vec F \cdot \vec s$$ | Lavoro |

# Costanti e conversioni

| Nome         | Valore                                 |
| ------------ | -------------------------------------- |
| $\mu_0$      | $4 \pi \cdot 10^{-7}\cdot \frac{H}{m}$ |
| $1G$         | $10^{-4}T$                             |
| $e^-$        | $1.6\cdot10^{-19}C$                    |
| $\epsilon_0$ | $8.854\cdot 10^{-12}\frac{C^2}{Nm^2}$  |
| $k_0$        | $\frac{1}{4 \pi \epsilon_0}$           |
| $c$          | $299\ 792\ 458 {m \over s}$            |
