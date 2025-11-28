```
\newcommand{\s}[2]{#1 \times 10^{#2}}
```

```
\begin{align}
& \\
\end{align}
```
$\overset{testo sopra}{testo}$ `\overset{testo sopra}{testo}
$\underset{testo sotto}{testo}$ `\underset{testo sotto}{testo}
# Aiuto:Formule matematiche

> **Nota:** Questa pagina è la traduzione della pagina inglese [meta:Help:Formula](https://meta.wikimedia.org/wiki/Help:Formula). Verrà aggiornata di tanto in tanto, ma la pagina inglese resta la guida di riferimento.

Dal gennaio 2003, su Wikipedia è possibile utilizzare comandi [TeX](https://it.wikipedia.org/wiki/TeX) per la formattazione di formule matematiche. In Obsidian, le formule inline sono racchiuse tra singoli simboli `$`, mentre le formule a blocco (che occupano l'intera larghezza della pagina) sono racchiuse tra tripli simboli `$$$`. Le interruzioni di linea all'interno delle formule non vengono tradotte, ma è possibile richiedere interruzioni di linea o altri posizionamenti con comandi specifici (ad esempio, un'interruzione di linea dopo ogni termine o riga di una matrice).

**Segnalazioni:** Discussioni, errori riscontrati o richieste di nuove funzionalità devono essere indirizzate alla [mailing list Wikitech-l](http://mail.wikipedia.org/mailman/listinfo/wikitech-l) o a [Wikipedia:TeX requests](https://en.wikipedia.org/wiki/Wikipedia:TeX_requests) (in inglese).

**Stile:** Per problemi relativi alla composizione di contenuti matematici, consultare il [Manuale di stile del Progetto Matematica](https://it.wikipedia.org/wiki/Progetto:Matematica/Manuale_di_stile). Si raccomanda di evitare l'uso di formule inline in un testo normale, poiché le formule non si allineano coerentemente con il testo e il loro font ha una dimensione maggiore.

**Colore:** Questa pagina ha uno sfondo rosa poiché appartiene allo spazio "Aiuto:". Le pagine normali di Wikipedia hanno uno sfondo bianco, come le formule, quindi non dovrebbero esserci problemi di visualizzazione.

## MediaWiki e TeX

[MediaWiki](https://it.wikipedia.org/wiki/MediaWiki) utilizza un sottoinsieme dei comandi [TeX](https://it.wikipedia.org/wiki/TeX) (con alcune estensioni di [LaTeX](https://it.wikipedia.org/wiki/LaTeX) e [AMSLaTeX](https://it.wikipedia.org/wiki/AMS-LaTeX)) per formattare formule matematiche, convertendole in immagini [PNG](https://it.wikipedia.org/wiki/Portable_Network_Graphics). Più precisamente, MediaWiki filtra il markup attraverso Texvc, che converte i comandi in TeX e li passa al motore di rendering. Solo una parte del linguaggio TeX è supportata (vedi dettagli di seguito).

## Sintassi

In Obsidian, i comandi TeX per formule inline devono essere racchiusi tra `$`, mentre le formule a blocco devono essere racchiuse tra `$$$`. La barra degli strumenti di modifica di Wikipedia include un pulsante dedicato per i tag `<math>`, ma in Obsidian si utilizzano i simboli `$` o `$$$` (consultare la [guida alla barra degli strumenti](https://meta.wikimedia.org/wiki/Help:Edit_toolbar) per dettagli su Wikipedia).

**Spazi e ritorno a capo:** TeX tratta gli spazi bianchi e i ritorni a capo in modo simile all'[HTML](https://it.wikipedia.org/wiki/HTML), ignorandoli. Tuttavia, è possibile gestire manualmente la spaziatura, come descritto più avanti.

**Limitazioni:** I template, le variabili e i parametri non possono contenere formule TeX in Obsidian. Per dettagli, vedere [Demo per l'utilizzo di parametri che includono TeX](https://meta.wikimedia.org/wiki/Template_talk:Demo_of_attempt_to_use_parameters_within_TeX).

## Funzioni, simboli, caratteri speciali

|**Caratteristica**|**Sintassi**|**Come appare**|
|---|---|---|
|**Accenti**|`\acute{a} \quad \grave{a} \quad \breve{a} \quad \check{a} \quad \tilde{a} \quad \hat{a} \quad \dot{a}`|$\acute{a} \quad \grave{a} \quad \breve{a} \quad \check{a} \quad \tilde{a} \quad \hat{a} \quad \dot{a}$|
|**Funzioni elementari (metodo corretto)**|`\sin x + \ln y + \operatorname{sgn} \, z<br />\sin a \ \cos b \ \tan c \ \cot d \ \sec e \ \csc f<br />\sinh g \ \cosh h \ \tanh i \ \coth j<br />\arcsin k \ \arccos l \ \arctan m<br />\lim n \ \limsup o \ \liminf p<br />\min q \ \max r \ \inf s \ \sup t<br />\exp u \ \lg v \ \log w<br />\ker x \ \deg x \gcd x \Pr x \ \det x \hom x \ \arg x \dim x`|$\sin x + \ln y + \operatorname{sgn} , z$  <br>$\sin a \ \cos b \ \tan c \ \cot d \ \sec e \ \csc f$  <br>$\sinh g \ \cosh h \ \tanh i \ \coth j$  <br>$\arcsin k \ \arccos l \ \arctan m$  <br>$\lim n \ \limsup o \ \liminf p$  <br>$\min q \ \max r \ \inf s \ \sup t$  <br>$\exp u \ \lg v \ \log w$  <br>$\ker x \ \deg x \gcd x \Pr x \ \det x \hom x \ \arg x \dim x$|
|**Funzioni elementari (metodo non corretto)**|`sin x + ln y + sgn z`|$sin x + ln y + sgn z$|
|**Aritmetica dell'orologio**|`s_k \equiv 0 \pmod{m}<br />a \bmod b`|$s_k \equiv 0 \pmod{m}$  <br>$a \bmod b$|
|**Derivate**|`\nabla \partial x dx \dot x \ddot y`|$\nabla ; \partial x ; dx ; \dot x ; \ddot y$|
|**Insiemi**|`\forall \exists \empty \emptyset \varnothing \in \ni \not\in \notin<br />\subset \subseteq \not\subseteq \supset \supseteq \cap \bigcap \cup \bigcup \biguplus \times \setminus \smallsetminus`|$\forall ; \exists ; \empty ; \emptyset ; \varnothing \in \ni \not\in \notin$  <br>$\subset \subseteq \not\subseteq \supset \supseteq \cap \bigcap \cup \bigcup \biguplus \times \setminus \smallsetminus$|
|**Insiemi (continua)**|`\sqsubset \sqsubseteq \sqsupset \sqsupseteq \sqcap \sqcup \bigsqcup`|$\sqsubset \sqsubseteq \sqsupset \sqsupseteq \sqcap \sqcup \bigsqcup$|
|**Logica**|`p \land \wedge \bigwedge \bar{q} \to p \lor \vee \bigvee \lnot \neg q`|$p \land \wedge ; \bigwedge ; \bar{q} \to p \lor \vee ; \bigvee ; \lnot ; \neg q$|
|**Radicali**|`\sqrt{2}\approx 1{,}4`|$\sqrt{2}\approx 1{,}4$|
|**Radicali (continua)**|`\sqrt[n]{x}`|$\sqrt[n]{x}$|
|**Simboli relazionali**|`\sim \approx \simeq \cong \doteq \le < \ll \gg \ge > \equiv \not\equiv \ne \propto \div \pm \mp`|$\sim ; \approx ; \simeq ; \cong ; \doteq ; \le ; < ; \ll ; \gg ; \ge ; > ; \equiv ; \not\equiv ; \ne ; \propto ; \div ; \pm ; \mp$|
|**Simboli geometrici**|`\Diamond \Box \triangle \angle \perp \mid \nmid \| 45^\circ`|$\Diamond ; \Box ; \triangle ; \angle ; \perp ; \mid ; \nmid ; \| ; 45^\circ$|
|**Frecce**|`\leftarrow \gets \rightarrow \to \leftrightarrow<br />\longleftarrow \longrightarrow<br />\mapsto \longmapsto \hookrightarrow \hookleftarrow<br />\nearrow \searrow \swarrow \nwarrow<br />\uparrow \downarrow \updownarrow \leftrightarrows`|$\leftarrow ; \gets ; \rightarrow ; \to ; \leftrightarrow$  <br>$\longleftarrow ; \longrightarrow$  <br>$\mapsto ; \longmapsto ; \hookrightarrow ; \hookleftarrow$  <br>$\nearrow ; \searrow ; \swarrow ; \nwarrow$  <br>$\uparrow \downarrow \updownarrow\ ; \leftrightarrows$|
|**Frecce (continua)**|`\rightharpoon \rightharpoondown \leftharpoon \leftharpoondown \upharpoonleft \upharpoonright \downharpoonleft \downharpoonright`|$\rightharpoon ; \rightharpoondown ; \leftharpoon ; \leftharpoondown ; \upharpoonleft ; \upharpoonright ; \downharpoonleft ; \downharpoonright$|
|**Frecce (continua)**|`\Leftarrow \Rightarrow \Leftrightarrow<br />\Longleftarrow \Longrightarrow \Longleftrightarrow (o \iff)<br />\Uparrow \Downarrow \Updownarrow`|$\Leftarrow ; \Rightarrow ; \Leftrightarrow$  <br>$\Longleftarrow ; \Longrightarrow ; \Longleftrightarrow (o \iff)$  <br>$\Uparrow ; \Downarrow ; \Updownarrow$|
|**Simboli speciali**|`\eth \S \P \% \dagger \ddagger \star * \ldots<br />\smile \frown \wr \oplus \bigoplus \otimes \bigotimes<br />\cdot \circ \bullet \bigodot \triangleleft \triangleright \infty \bot \top \vdash \vDash \Vdash \models \lVert \rVert<br />\imath \hbar \ell \mho \Finv \Re \Im \wp \complement \quad \diamondsuit \heartsuit \clubsuit \spadesuit \Game \quad \flat \natural \sharp`|$\eth ; \S ; \P ; % ; \dagger ; \ddagger ; \star ; * ; \ldots$  <br>$\smile \frown \wr \oplus \bigoplus \otimes \bigotimes$  <br>$\cdot \circ \bullet \bigodot \triangleleft \triangleright \infty \bot \top \vdash \vDash \Vdash \models \lVert \rVert$  <br>$\imath ; \hbar ; \ell ; \mho ; \Finv ; \Re ; \Im ; \wp ; \complement \quad \diamondsuit ; \heartsuit ; \clubsuit ; \spadesuit ; \Game \quad \flat ; \natural ; \sharp$|
|**Lettere maiuscole con \mathcal**|`\mathcal {0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZ}`|$\mathcal {0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZ}$|

## Apici, pedici, integrali

| **Caratteristica**                      | **Sintassi**                                                                                                                                 | **Come appare**                                                                                                                             |
| --------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- |
| **Apice**                               | `a^2`                                                                                                                                        | $a^2$                                                                                                                                       |
| **Pedice**                              | `a_2`                                                                                                                                        | $a_2$                                                                                                                                       |
| **Raggruppamento**                      | `a^{2+2}`                                                                                                                                    | $a^{2+2}$                                                                                                                                   |
| **Raggruppamento**                      | `a_{i,j}`                                                                                                                                    | $a_{i,j}$                                                                                                                                   |
| **Combinazione di apici e pedici**      | `x_2^3`                                                                                                                                      | $x_2^3$                                                                                                                                     |
| **Derivate**                            | `x', y'', f', f''`                                                                                                                           | $x', y'', f', f''$                                                                                                                          |
| **Sottolineato, sopralineato, vettori** | `\hat a \ \bar b \ \vec c \ \overrightarrow{a b} \ \overleftarrow{c d} \ \widehat{d e f} \ \overline{g h i} \ \underline{j k l} \ \tilde{x}` | $\hat a \ \bar b \ \vec c \ \overrightarrow{a b} \ \overleftarrow{c d} \ \widehat{d e f} \ \overline{g h i} \ \underline{j k l}\ \tilde{x}$ |
| **Parentesi sopra**                     | `\overbrace{ 1+2+\cdots+100 }^{5050}`                                                                                                        | $\overbrace{ 1+2+\cdots+100 }^{5050}$                                                                                                       |
| **Parentesi sotto**                     | `\underbrace{ a+b+\cdots+z }_{26}`                                                                                                           | $\underbrace{ a+b+\cdots+z }_{26}$                                                                                                          |
| **Sommatoria**                          | `\sum_{k=1}^N k^2`                                                                                                                           | $\sum_{k=1}^N k^2$                                                                                                                          |
| **Sommatoria (forzando \textstyle)**    | `\begin{matrix} \sum_{k=1}^N k^2 \end{matrix}`                                                                                               | $\begin{matrix} \sum_{k=1}^N k^2 \end{matrix}$                                                                                              |
| **Produttoria**                         | `\prod_{i=1}^N x_i`                                                                                                                          | $\prod_{i=1}^N x_i$                                                                                                                         |
| **Produttoria (forzando \textstyle)**   | `\begin{matrix} \prod_{i=1}^N x_i \end{matrix}`                                                                                              | $\begin{matrix} \prod_{i=1}^N x_i \end{matrix}$                                                                                             |
| **Coproduttoria**                       | `\coprod_{i=1}^N x_i`                                                                                                                        | $\coprod_{i=1}^N x_i$                                                                                                                       |
| **Coproduttoria (forzando \textstyle)** | `\begin{matrix} \coprod_{i=1}^N x_i \end{matrix}`                                                                                            | $\begin{matrix} \coprod_{i=1}^N x_i \end{matrix}$                                                                                           |
| **Limite**                              | `\lim_{n \to \infty}x_n`                                                                                                                     | $\lim_{n \to \infty}x_n$                                                                                                                    |
| **Limite (forzando \textstyle)**        | `\begin{matrix} \lim_{n \to \infty}x_n \end{matrix}`                                                                                         | $\begin{matrix} \lim_{n \to \infty}x_n \end{matrix}$                                                                                        |
| **Integrale**                           | `\int_{-N}^{N} e^x\, dx`                                                                                                                     | $\int_{-N}^{N} e^x, dx$                                                                                                                     |
| **Integrale (forzando \textstyle)**     | `\begin{matrix} \int_{-N}^{N} e^x\, dx \end{matrix}`                                                                                         | $\begin{matrix} \int_{-N}^{N} e^x, dx \end{matrix}$                                                                                         |
| **Integrale doppio**                    | `\iint_{D}^{W} \, dx\,dy`                                                                                                                    | $\iint_{D}^{W} , dx,dy$                                                                                                                     |
| **Integrale triplo**                    | `\iiint_{E}^{V} \, dx\,dy\,dz`                                                                                                               | $\iiint_{E}^{V} , dx,dy,dz$                                                                                                                 |
| **Integrale quadruplo**                 | `\iiiint_{F}^{U} \, dx\,dy\,dz\,dt`                                                                                                          | $\iiiint_{F}^{U} , dx,dy,dz,dt$                                                                                                             |
| **Integrale su frontiera**              | `\oint_{C} x^3\, dx + 4y^2\, dy`                                                                                                             | $\oint_{C} x^3, dx + 4y^2, dy$                                                                                                              |
| **Intersezioni**                        | `\bigcap_1^{n} p`                                                                                                                            | $\bigcap_1^{n} p$                                                                                                                           |
| **Unioni**                              | `\bigcup_1^{k} p`                                                                                                                            | $\bigcup_1^{k} p$                                                                                                                           |

## Frazioni, matrici, multi-linea

|**Caratteristica**|**Sintassi**|**Come appare**|
|---|---|---|
|**Frazioni**|`\frac{2}{4}` o `{2 \over 4}`|$\frac{2}{4}$|
|**Frazioni**|`\tfrac{2}{4}`|$\tfrac{2}{4}$|
|**Coefficienti binomiali**|`\binom{n}{k}` o `{n \choose k}`|${n \choose k}$|
|**Matrici**|`\begin{matrix} x & y \\ z & v \end{matrix}`|$\begin{matrix} x & y \ z & v \end{matrix}$|
|**Matrici**|`\begin{vmatrix} x & y \\ z & v \end{vmatrix}`|$\begin{vmatrix} x & y \ z & v \end{vmatrix}$|
|**Matrici**|`\begin{Vmatrix} x & y \\ z & v \end{Vmatrix}`|$\begin{Vmatrix} x & y \ z & v \end{Vmatrix}$|
|**Matrici**|`\begin{bmatrix} 0 & \cdots & 0 \\ \vdots & \ddots & \vdots \\ 0 & \cdots & 0\end{bmatrix}`|$\begin{bmatrix} 0 & \cdots & 0 \ \vdots & \ddots & \vdots \ 0 & \cdots & 0\end{bmatrix}$|
|**Matrici**|`\begin{Bmatrix} x & y \\ z & v \end{Bmatrix}`|$\begin{Bmatrix} x & y \ z & v \end{Bmatrix}$|
|**Distinzione di casi**|`f(n)=\begin{cases} n/2, & \mbox{se }n\mbox{ pari} \\ 3n+1, & \mbox{se }n\mbox{ dispari} \end{cases}`|$f(n)=\begin{cases} n/2, & \mbox{se }n\mbox{ pari} \ 3n+1, & \mbox{se }n\mbox{ dispari} \end{cases}$|
|**Equazioni su più righe**|`\begin{align} f(n+1) &= (n+1)^2 \\ &= n^2 + 2n + 1\end{align}`|$\begin{align} f(n+1) &= (n+1)^2 \ &= n^2 + 2n + 1\end{align}$|

## Font

| **Caratteristica**                  | **Sintassi**                                                                                                                                          | **Come appare**                                                                                                                                                              |
| ----------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Lettere greche maiuscole**        | `\Alpha \Beta \Gamma \Delta \Epsilon \Zeta \Eta \Theta \Iota \Kappa \Lambda \Mu \Nu \Xi \Omicron \Pi \Rho \Sigma \Tau \Upsilon \Phi \Chi \Psi \Omega` | $\Alpha\ \Beta\ \Gamma\ \Delta\ \Epsilon\ \Zeta\ \Eta\ \Theta\ \Iota\ \Kappa\ \Lambda\ \Mu\ \Nu\ \Xi\ \Omicron\ \Pi\ \Rho\ \Sigma\ \Tau\ \Upsilon\ \Phi\ \Chi\ \Psi\ \Omega$ |
| **Lettere greche minuscole**        | `\alpha \beta \gamma \delta \epsilon \zeta \eta \theta \iota \kappa \lambda \mu \nu \xi \omicron \pi \rho \sigma \tau \upsilon \phi \chi \psi \omega` | $\alpha\ \beta\ \gamma\ \delta\ \epsilon\ \zeta\ \eta\ \theta\ \iota\ \kappa\ \lambda\ \mu\ \nu\ \xi\ \omicron\ \pi\ \rho\ \sigma\ \tau\ \upsilon\ \phi\ \chi\ \psi\ \omega$ |
| **Altre lettere greche**            | `\varepsilon \digamma \vartheta \varkappa \varpi \varrho \varsigma \varphi`                                                                           | $\varepsilon\ \digamma\ \vartheta\ \varkappa\ \varpi\ \varrho\ \varsigma\ \varphi$                                                                                           |
| **Grassetto lavagna**               | `\mathbb{N} \mathbb{Z} \mathbb{Q} \mathbb{R} \mathbb{C} \mathbb{H} \mathbb{E}`                                                                        | $\mathbb{N}\ \mathbb{Z}\ \mathbb{Q}\ \mathbb{R}\ \mathbb{C} \ \mathbb{H} \ \mathbb{E}$                                                                                       |
| **Grassetto (per vettori)**         | `\mathbf{x}\cdot\mathbf{y} = 0`                                                                                                                       | $\mathbf{x}\cdot\mathbf{y} = 0$                                                                                                                                              |
| **Grassetto per lettere greche**    | `\boldsymbol{\alpha} + \boldsymbol{\beta} + \boldsymbol{\gamma}`                                                                                      | $\boldsymbol{\alpha} + \boldsymbol{\beta} + \boldsymbol{\gamma}$                                                                                                             |
| **Corsivo**                         | `\mathit{ABCDE abcde 1234}`                                                                                                                           | $\mathit{ABCDE abcde 1234}$                                                                                                                                                  |
| **Font Roman**                      | `\mathrm{ABCDE abcde 1234}`                                                                                                                           | $\mathrm{ABCDE abcde 1234}$                                                                                                                                                  |
| **Font Fraktur**                    | `\mathfrak{ABCDE abcde 1234}`                                                                                                                         | $\mathfrak{ABCDE abcde 1234}$                                                                                                                                                |
| **Calligrafico**                    | `\mathcal{ABCDE abcde 1234}`                                                                                                                          | $\mathcal{ABCDE abcde 1234}$                                                                                                                                                 |
| **Lettere ebraiche**                | `\aleph \beth \gimel \daleth`                                                                                                                         | $\aleph\ \beth\ \gimel\ \daleth$                                                                                                                                             |
| **Caratteri non corsivi**           | `\mbox{abc}` o `\text{abc}`                                                                                                                           | $\mbox{abc}$                                                                                                                                                                 |
| **Misto corsivo (cattivo esempio)** | `\mbox{se} n \mbox{pari}`                                                                                                                             | $\mbox{se} n \mbox{pari}$                                                                                                                                                    |
| **Misto corsivo (buon esempio)**    | `\mbox{se } n \mbox{ pari}`                                                                                                                           | $\mbox{se }n\mbox{ pari}$                                                                                                                                                    |

## Le parentesi nelle espressioni estese

|**Caratteristica**|**Sintassi**|**Come appare**|
|---|---|---|
|**Da evitare**|`( \frac{1}{2} )`|$( \frac{1}{2} )$|
|**Preferibile**|`\left( \frac{1}{2} \right)`|$\left ( \frac{1}{2} \right )$|

**Delimitatori con \left e \right:**

| **Caratteristica**           | **Sintassi**                                           | **Come appare**                      |
| ---------------------------- | ------------------------------------------------------ | ------------------------------------ |
| **Parentesi tonde**          | `\left ( A \right )`                                   | $\left ( A \right )$                 |
| **Parentesi quadre**         | `\left [ A \right ]`                                   | $\left [ A \right ]$                 |
| **Parentesi graffe**         | `\left \{ A \right \}`                                 | $\left { A \right }$                 |
| **Parentesi angolari**       | `\left \langle A \right \rangle`                       | $\left \langle A \right \rangle$     |
| **Barre semplici e doppie**  | `\left                                                 | A \right                             |
| **Delimitatori combinati**   | `\left [ 0,1 \right )`  <br>`\left \langle \psi \right | `                                    |
| **Omettere un delimitatore** | `\left . \frac{A}{B} \right \} \to X`                  | $\left . \frac{A}{B} \right } \to X$ |

## Spaziatura

TeX gestisce automaticamente la spaziatura, ma può essere controllata manualmente:

| **Caratteristica**         | **Sintassi** | **Come appare**  |
| -------------------------- | ------------ | ---------------- |
| **Doppia spaziatura quad** | `a \qquad b` | $a \qquad b$     |
| **Spaziatura quad**        | `a \quad b`  | $a \quad b$      |
| **Spaziatura del testo**   | `a\ b`       | $a\ b$           |
| **Spaziatura grande**      | `a\;b`       | $a;b$            |
| **Spaziatura media**       | `a\>b`       | [non supportata] |
| **Spaziatura piccola**     | `a\,b`       | $a,b$            |
| **Nessuna spaziatura**     | `ab`         | $ab$             |
| **Spaziatura negativa**    | `a\!b`       | $a!b$            |

## Allineamento col testo normale

Per impostazione predefinita, lo stile CSS applica:

```css
img.tex { vertical-align: middle; }
```

Ad esempio: $$$\int_{-N}^{N} e^x, dx$$$.

Per un allineamento diverso, utilizzare:

```html
<div style="vertical-align:-100%;display:inline;">$$$\int_{-N}^{N} e^x\, dx$$$</div>
```

Modificate il valore di `vertical-align` per ottenere il risultato desiderato. Nota: il rendering può variare tra browser diversi.

## Esempi

### Polinomio di secondo grado

```latex
$ax^2 + bx + c = 0$
```

$$$ax^2 + bx + c = 0$$$

### Soluzioni di un'equazione di secondo grado

```latex
$x_{1,2}=\frac{-b\pm\sqrt{b^2-4ac}}{2a}$
```

$$$x_{1,2}=\frac{-b\pm\sqrt{b^2-4ac}}{2a}$$$

### Radici

```latex
$\sqrt{256}=16$
```

$$$\sqrt{256}=16$$$

```latex
$\sqrt[5]{32}=2$
```

$$$\sqrt[5]{32}=2$$$

### Sistema di equazioni

```latex
$\begin{cases} 3x-y+8=0\\ 7-6x+12y=0\\ \end{cases}$
```

$$$\begin{cases} 3x-y+8=0\ 7-6x+12y=0\ \end{cases}$$$

### Logaritmi

```latex
$\log_{a}{b}=\frac{\log_{c}{b}}{\log_{c}{a}}$
```

$$$\log_{a}{b}=\frac{\log_{c}{b}}{\log_{c}{a}}$$$

### Parentesi e frazioni

```latex
$2=\left[\frac{\left(3-x\right)\times 2}{3-x}\right]$
```

$$$2=\left[\frac{\left(3-x\right)\times 2}{3-x}\right]$$$

### Integrali

```latex
$\int_a^x \int_a^s f(y)\,dy\,ds = \int_a^x f(y)(x-y)\,dy$
```

$$$\int_a^x \int_a^s f(y),dy,ds = \int_a^x f(y)(x-y),dy$$$

### Sommatorie

```latex
$\sum_{m=1}^\infty\sum_{n=1}^\infty\frac{m^2\,n}{3^m\left(m\,3^n+n\,3^m\right)}$
```

$$$\sum_{m=1}^\infty\sum_{n=1}^\infty\frac{m^2,n}{3^m\left(m,3^n+n,3^m\right)}$$$

### Equazioni differenziali

```latex
$u'' + p(x)u' + q(x)u=f(x),\quad x>a$
```

$$$u'' + p(x)u' + q(x)u=f(x),\quad x>a$$$

### Numeri complessi

```latex
$|\bar{z}| = |z|, |(\bar{z})^n| = |z|^n, \arg(z^n) = n \arg(z)$
```

$$$|\bar{z}| = |z|, |(\bar{z})^n| = |z|^n, \arg(z^n) = n \arg(z)$$$

### Limiti

```latex
$\lim_{z\rightarrow z_0} f(z)=f(z_0)$
```

$$$\lim_{z\rightarrow z_0} f(z)=f(z_0)$$$

Per limiti in due variabili:

```latex
$\lim_{(x,y) \to (x_0 , y_0)} f(x,y)=f(x_0,y_0)$
```

$$$\lim_{(x,y) \to (x_0 , y_0)} f(x,y)=f(x_0,y_0)$$$

Oppure con:

```latex
$\mathbf{x} = (x,y)$ e $\mathbf{x}_0 = (x_0,y_0)$
$\lim_{\mathbf{x} \to \mathbf{x}_0} f(\mathbf{x})=f(\mathbf{x}_0)$
```

$$$\mathbf{x} = (x,y)$$$ e $$$\mathbf{x}_0 = (x_0,y_0)$$$  
$$$\lim_{\mathbf{x} \to \mathbf{x}_0} f(\mathbf{x})=f(\mathbf{x}_0)$$$

### Equazioni integrali

```latex
$\phi_n(\kappa) = \frac{1}{4\pi^2\kappa^2} \int_0^\infty \frac{\sin(\kappa R)}{\kappa R} \frac{\partial}{\partial R}\left[R^2\frac{\partial D_n(R)}{\partial R}\right]\,dR$
```

$$$\phi_n(\kappa) = \frac{1}{4\pi^2\kappa^2} \int_0^\infty \frac{\sin(\kappa R)}{\kappa R} \frac{\partial}{\partial R}\left[R^2\frac{\partial D_n(R)}{\partial R}\right],dR$$$

### Esempio generico

```latex
$\phi_n(\kappa) = 0,\!033 \, C_n^2 \, \kappa^{-11/3},\quad \frac{1}{L_0}\ll\kappa\ll\frac{1}{l_0}$
```

$$$\phi_n(\kappa) = 0,!033 , C_n^2 , \kappa^{-11/3},\quad \frac{1}{L_0}\ll\kappa\ll\frac{1}{l_0}$$$

### Funzioni definite a tratti

```latex
$f(x) = \begin{cases}1 & -1 \le x < 0\\ \frac{1}{2} & x = 0\\x&0<x\le 1\end{cases}$
```

$$$f(x) = \begin{cases}1 & -1 \le x < 0\ \frac{1}{2} & x = 0\x&0<x\le 1\end{cases}$$$

### Pedice prescritta

```latex
${}_pF_q(a_1,\dots,a_p;c_1,\cdots,c_q;z) = \sum_{n=0}^\infty \frac{(a_1)_n\cdots(a_p)_n}{(c_1)_n\cdots(c_q)_n}\frac{z^n}{n!}$
```

$$${}_pF_q(a_1,\dots,a_p;c_1,\cdots,c_q;z) = \sum_{n=0}^\infty \frac{(a_1)_n\cdots(a_p)_n}{(c_1)_n\cdots(c_q)_n}\frac{z^n}{n!}$$$