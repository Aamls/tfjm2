# tfjm² 2027

**Équipe :** Équipe Lycée Rocroy Saint-Vincent de Paul  
**Date :** novembre 2026

## Chaises musicales au restaurant

**Figure 1.a —** $n=6$, table ronde, plan de table et consigne de rotation.

*Schéma source :* `table_ronde.tex` (TikZ). Le schéma représente six places numérotées de 1 à 6 disposées en cercle, avec les arêtes du cycle $1-2-3-4-5-6-1$, puis une consigne de rotation orientée.

- Le plan de table est invariant par rotation. Lorsque le plat $1<i\leq 10$ est servi, deux convives sont assis à deux places reliées si et seulement s’ils étaient assis à deux places reliées au plat précédent.

  ...

- Chaque convive ne peut parler qu’à deux personnes différentes par plat. Pour que chaque convive puisse parler aux cinq autres personnes présentes il faudra nécessairement 3 plats.

  La figure 1.b représente (à faire !) un exemple de consigne de rotation qui réalise le minimum de 3 plats (à démontrer !).

  **Figure 1.b —** Consigne de rotation permettant à chaque convive de parler à tout le monde après trois plats.

  *Schéma source :* `consigne_rotation_1b.tex` (TikZ), conservé dans le dossier d’origine. Il représente les six sommets numérotés et les flèches de rotation entre eux.

## Dés personnalisés

D’après l’exemple de l’énoncé l’espérance du dé de Léo est :

$$
\begin{aligned}
\mathbb{E}(X_L) &= 1\times\frac{1}{6}+2\times\frac{1}{6}+3\times\frac{1}{6}+5\times\frac{1}{6}+8\times\frac{1}{6}+13\times\frac{1}{6} \\
&= \frac{16}{3}.
\end{aligned}
$$

Celle de Théo :

$$
\begin{aligned}
\mathbb{E}(X_T) &= 0\times\frac{1}{4}+2\times\frac{1}{4}+10\times\frac{1}{4}+10\times\frac{1}{4}\\
&= \frac{11}{2}.
\end{aligned}
$$

Le score de Léo est défini comme la probabilité que Léo tire un chiffre strictement plus grand que celui de Théo plus la moitié de celle que ces deux chiffres soient égaux :

$$
S_L = P(X_L>X_T) + \frac{1}{2}P(X_l=X_T).
$$

L’application numérique dans le cas de l’exemple de l’énoncé est :

$$
\begin{aligned}
S_T &= P(X_T>X_L\mid X_T=10)\times P(X_T=10) + P(X_T>X_L\mid X_T=2)\times P(X_T=2)\\
&\quad + P(X_T>X_L\mid X_T=0)\times P(X_T=0) + \frac{1}{2}P(X_T=X_L\mid X_T=10)\times P(X_T=10)\\
&\quad + \frac{1}{2}P(X_T=X_L\mid X_T=2)\times P(X_T=2) + \frac{1}{2}P(X_T=X_L\mid X_T=0)\times P(X_T=0)
\end{aligned}
$$

soit encore

$$
\begin{aligned}
S_T &= P(10>X_L)\times P(X_T=10) + P(2>X_L)\times P(X_T=2)\\
&\quad + P(0>X_L)\times P(X_T=0) + \frac{1}{2}P(10=X_L)\times P(X_T=10)\\
&\quad + \frac{1}{2}P(2=X_L)\times P(X_T=2) + \frac{1}{2}P(0=X_L)\times P(X_T=0)\\
&= \frac{5}{6}\times\frac{1}{2} + \frac{1}{6}\times\frac{1}{4} + 0 + 0 + \frac{1}{2}\times\frac{1}{6}\times\frac{1}{4} + 0\\
&= \frac{23}{48}
\end{aligned}
$$

- Le pire score pour Théo est...

- Le meilleur score pour Théo est...

## La couturière de vérité

Partie de Louis...

## Triskaïdékaphobie

Partie d’Eloi...

## Perdus dans la forêt

Pour cette réponse,

Soit une droite $d$ d’équation $y = kx$ passant par $O(0,0)\in d$,

Un point $F(x',y')\in A$ tel que $x'$ et $y'$ sont premiers entre eux, i.e. $F$ est le premier point de $d$ de coordonnées entières naturelles non nulles. Donc $F$ est le premier arbre sur $d$.

Et $I(a,b)\in d$ tel que $(a,b)\in\mathbb{R}^2 \setminus A$.

### 1. Condition nécessaire

Si $F(x',y')\in d$ et $I(a,b)\in d$ tel que $F\in [OI]$ alors Ines est cachée, d’après l’énoncé.

$$
F(x',y')\in d \text{ et } I(a,b)\in d \text{ tel que } F\in [OI]
$$

$$
\Leftrightarrow\ k\in \mathbb{Q}^+ \text{ car } F(x',y')\in A \text{ et } \vec{OF} \text{ et } \vec{OI} \text{ sont colinéaires car } F\in [OI]\subset d
$$

$$
\Leftrightarrow\ k\in \mathbb{Q}^+ \text{ et } \vec{OI}=n\vec{OF} \text{ avec } n>1
$$

$$
\Leftrightarrow\ k\in \mathbb{Q}^+ \text{ et } \vec{OI}=\begin{pmatrix} a \\ b \end{pmatrix} = n\vec{OF}=\begin{pmatrix} x' \\ y' \end{pmatrix} \text{ où } n>1
$$

$$
\Leftrightarrow\ k\in \mathbb{Q}^+ \text{ et } n=\frac{a}{x'}=\frac{b}{y'}>1
$$

On a donc :

Si $k\in \mathbb{Q}^+$ et $n=\frac{a}{x'}=\frac{b}{y'}>1$ ($n\neq 0$) alors Ines est cachée.

Ainsi par contraposée on peut donc conclure :

Si Ines est visible alors $k\in \mathbb{R}\setminus \mathbb{Q}^+$ ou $k\in \mathbb{Q}^+$ et $n=\frac{a}{x'}=\frac{b}{y'}<1$ ($n\neq 0$).

### 2. Condition suffisante

- Si $k\in \mathbb{R} \setminus \mathbb{Q}^+$ alors il n’existe pas de point $E\in A$ tel que $E\in d$.

  Donc il n’existe pas de point $F(x',y')\in d$ tel que $F(x',y')\in A$.

  Or $I(a,b)\in d$.

  Donc il n’existe pas d’arbre sur le segment $[OI]$.

  Donc Ines est visible.

- $k\in \mathbb{Q}^+$ et $n=\frac{a}{x'}=\frac{b}{y'}<1$ ($n\neq 0$) $\Leftrightarrow$ $k\in \mathbb{Q}^+$ et $\vec{OI}=\begin{pmatrix} a \\ b \end{pmatrix} = n\vec{OF}=\begin{pmatrix} x' \\ y' \end{pmatrix}$ ($n\neq 0$).

  - Si $n<0$ :

    Donc $n=\frac{a}{x'}=\frac{b}{y'}<0$ or $(x',y')\in A$ donc $a<0$ et $b<0$.

    Donc $(a,b)\in \mathbb{R}^{-2}$ or il n’y a pas d’arbre car $A=\mathbb{N}^2 \setminus \{(0,0)\}$.

    Donc Ines est visible.

  - Si $0<n<1$ :

    Donc $0<n=\frac{a}{x'}=\frac{b}{y'}<1$ donc $a<x'$ et $b<y'$.

    Or $I(a,b)\in d$ et $F(x',y')\in d$.

    Donc $F\notin[OI]$.

    Donc il n’y a pas d’arbre sur $[OI]$, F étant le premier arbre sur $d$.

    Donc Ines est visible.

**Conclusion :**

Si $k\in \mathbb{R} \setminus \mathbb{Q}^+$ ou $k\in \mathbb{Q}^+$ et $n=\frac{a}{x'}=\frac{b}{y'}<1$ ($n\neq 0$) alors Ines est visible.

### 3. Condition nécessaire et suffisante

On a montré l’implication et la réciproque donc on a :

Ines est visible si et seulement si $k\in \mathbb{Q}^+$ et $n=\frac{a}{x'}=\frac{b}{y'}<1$ ($n\neq 0$) ou $k\in \mathbb{R} \setminus \mathbb{Q}^+$.
