**CONDITION NÉCESSAIRE**

Pour cette réponse, soit une droite $d$ d'équation $y = kx$ passant par $O(0,0) \in d$, un point $F(x,y) \in \mathbb{N}^2 \setminus \{(0,0)\}$ tel que $x$ et $y$ sont premiers entre eux (c'est-à-dire que $F$ est le premier point de $d$ de coordonnées entières naturelles non nulles). Et soit $I(a,b) \in d$ tel que $(a,b) \in \mathbb{R}^2 \setminus A$ et $I \neq O$.

Si Inès est cachée, alors $d$ passe par $F(x,y)$ et $I(a,b) \in d$ tel que le segment $[OI]$ passe par $F$.
Donc $k \in \mathbb{Q}^+$ puisque $F(x,y) \in d$, et $\overrightarrow{OF}$ et $\overrightarrow{OI}$ sont colinéaires ($I \in d$, $F \in d$ et $O \in d$).
Donc $k \in \mathbb{Q}^+$ et $\overrightarrow{OI} = n\overrightarrow{OF}$ avec $n > 1$ car $[OI]$ passe par $F$ (et $F \neq I$ car $I \notin A$).
Donc $k \in \mathbb{Q}^+$ et $\begin{cases} a = nx \\ b = ny \end{cases}$ avec $n > 1$.
Donc $k \in \mathbb{Q}^+$ et $n = \frac{a}{x} = \frac{b}{y} > 1$.

Par contraposée, on peut conclure que si Inès est visible, alors $k \in \mathbb{R} \setminus \mathbb{Q}^+$ ou $\left(k \in \mathbb{Q}^+ \text{ et } n = \frac{a}{x} = \frac{b}{y} < 1 \text{ avec } n \neq 0\right)$.

---

**CONDITION SUFFISANTE**

* **Si $k \in \mathbb{R} \setminus \mathbb{Q}^+$**, alors la droite $d$ ne passe par aucun point de coordonnées entières naturelles autres que $O(0,0)$.
  Donc il n'existe pas de point $F(x,y) \in d$ tel que $F(x,y) \in \mathbb{N}^2 \setminus \{(0,0)\}$.
  Or $I(a,b) \in d$, donc il n'existe pas d'arbre sur le segment $[OI]$.
  Donc Inès est visible.

* **Si $k \in \mathbb{Q}^+$ et $n = \frac{a}{x} = \frac{b}{y} < 1$ ($n \neq 0$)**, alors $\overrightarrow{OI} = n\overrightarrow{OF}$ où $n = \frac{a}{x} = \frac{b}{y} < 1$ ($n \neq 0$).

  * **Cas $n < 0$ :**
    Donc $n = \frac{a}{x} = \frac{b}{y} < 0$. Or $(x,y) \in \mathbb{N}^2 \setminus \{(0,0)\}$ (donc $x > 0$ et $y > 0$), d'où $a < 0$ et $b < 0$.
    Ainsi, tout point du segment $[OI]$ (autre que $O$) a des coordonnées strictement négatives. Or il n'y a pas d'arbre dans cette zone car $A = \mathbb{N}^2 \setminus \{(0,0)\}$.
    Donc Inès est visible.

  * **Cas $0 < n < 1$ :**
    Alors $0 < a < x$ et $0 < b < y$.
    Tout point $M(x_M, y_M)$ situé sur le segment $[OI]$ (avec $M \neq O$) vérifie donc $0 < x_M \leq a < x$ et $0 < y_M \leq b < y$.
    Or, par définition, $F(x,y)$ est le premier point de la droite $d$ appartenant à $\mathbb{N}^2 \setminus \{(0,0)\}$ (il possède les plus petites coordonnées entières strictement positives).
    Il ne peut donc exister aucun point à coordonnées entières strictement positives sur $[OI]$, et par conséquent aucun arbre entre $O$ et $I$.
    Donc Inès est visible.
