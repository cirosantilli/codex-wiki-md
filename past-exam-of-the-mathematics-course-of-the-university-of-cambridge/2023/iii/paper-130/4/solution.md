<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $X=\{v_1,\ldots,v_m\}$ be the vertices of a [regular polygon](../../../../../regular-polygon.md), indexed cyclically so that $v_i\mapsto v_{i+1}$ is an [isometry](../../../../../isometry.md). We first prove the product lemma needed for the cyclic-symmetry argument.

Suppose $A\subseteq X$ has the property that, for every number of colors, a finite witness forces a copy of $X$ on which the vertices corresponding to $A$ are monochromatic. We claim that for every $N,k$ there is a finite witness forcing an $A$-invariant copy of $X^N$. Proceed by [mathematical induction](../../../../../mathematical-induction.md) on $N$. The case $N=1$ is the assumption. For the step, choose a finite set $S$ that forces an $A$-invariant $X^{N-1}$ for a coloring with $k^{|X|-|A|+1}$ colors, and choose $T$ that forces an $A$-monochromatic $X$ for a coloring with $k^{|S|}$ colors.

Given a $k$-coloring $c$ of $S\times T$, color $t\in T$ by its complete vector $(c(s,t))_{s\in S}$. In the resulting copy of $X$ in $T$, that vector is the same for every member of $A$. Each $s\in S$ can therefore be colored by the vector consisting of $c(s,a)$ for one $a\in A$ and the colors $c(s,x)$ for $x\in X\setminus A$. Applying the choice of $S$ gives an $A$-invariant copy of $X^{N-1}$, and its product with the chosen copy of $X$ in $T$ is the desired $A$-invariant copy of $X^N$. This proves the lemma rather than assuming it.

We now prove by induction on $r$ that a finite witness forces a copy of $X$ whose first $r$ vertices have one color. The case $r=1$ is trivial. For $r=2$, use that a [line segment is a Euclidean Ramsey set](../../../../../line-segment-is-a-euclidean-ramsey-set.md); each occurrence of a segment congruent to $v_1v_2$ can be extended to a copy of the regular polygon, and only finitely many extensions are needed for a finite witness.

Assume the assertion for $r$, and put $A=\{v_1,\ldots,v_r\}$. The product lemma lets us work inside an $A$-invariantly colored copy of $X^N$, with $N$ as large as required. For an increasing $(m-1)$-element subset $H=\{a_1<\cdots<a_{m-1}\}$ of $[N]$ and $1\leq i\leq r$, define a word $w_i(H)$ by putting $v_{i+j}$ in coordinate $a_j$, with subscripts read modulo $m$, and putting $v_1$ in every other coordinate. Color $H$ by the $r$-tuple

$$
\bigl(c(w_1(H)),\ldots,c(w_r(H))\bigr).
$$

By the [Finite Ramsey theorem](../../../../../finite-ramsey-theorem.md), for sufficiently large $N$ there are coordinates $b_1<\cdots<b_m$ on which all $(m-1)$-subsets have the same tuple color.

For $1\leq i\leq r+1$, let $z_i$ be the word whose entries in coordinates $b_1,\ldots,b_m$ are

$$
v_i,v_{i+1},\ldots,v_{i+m-1},
$$

cyclically, and whose other entries are $v_1$. For $i\leq r$, the word $z_i$ differs from $w_i(\{b_2,\ldots,b_m\})$ only in coordinate $b_1$, where the two entries $v_i,v_1$ lie in $A$. Similarly $z_{i+1}$ differs from $w_i(\{b_1,\ldots,b_{m-1}\})$ only in coordinate $b_m$, again by two members of $A$. The $A$-invariance and the homogeneous choice of the $b_j$ therefore give

$$
c(z_i)=c\bigl(w_i(\{b_2,\ldots,b_m\})\bigr)
=c\bigl(w_i(\{b_1,\ldots,b_{m-1}\})\bigr)
=c(z_{i+1}).
$$

Hence $z_1,\ldots,z_{r+1}$ have one color.

The cyclic words $z_1,\ldots,z_m$ form an isometric copy of $\sqrt m X$: in each of the $m$ varying coordinates the cyclic shift is an isometry, so every squared distance is multiplied by $m$. Rescaling the finite witness by $1/\sqrt m$ gives a copy of $X$. The induction reaches $r=m$, proving that every regular polygon is a [Euclidean Ramsey set](../../../../../euclidean-ramsey-set.md).

For three consecutive vertices $p_0,p_1,p_2$ of a regular $M$-gon scaled to have side length one,

$$
d(p_0,p_1)=d(p_1,p_2)=1,
\qquad
d(p_0,p_2)=2\cos\frac{\pi}{M}\longrightarrow2.
$$

Since the polygon is Euclidean Ramsey, choosing $M$ large enough proves that $\{0,1,2\}$ is an [approximately Euclidean Ramsey set](../../../../../approximately-euclidean-ramsey-set.md).

In fact every finite $X\subseteq\mathbb R^d$ is approximately Ramsey. First perturb each coordinate of each point onto a sufficiently fine lattice $\delta\mathbb Z$, changing all pairwise [distances](../../../../../euclidean-distance.md) by less than $\varepsilon/2$. For each coordinate, map the finitely many required integers to consecutive vertices of a very large regular polygon, scaled so that one angular step has arc length $\delta$. If the step angle is $\theta$, the chord replacing a difference of $q$ lattice steps has length

$$
2\frac{\delta}{\theta}\sin\frac{|q|\theta}{2}
\longrightarrow |q|\delta
$$

as $\theta\to0$, uniformly over the finitely many differences involved. Taking the orthogonal [Cartesian product](../../../../../cartesian-product.md) of $d$ such polygons therefore embeds the perturbed points with a further distance error below $\varepsilon/2$. Each polygon is Euclidean Ramsey, and their product is Euclidean Ramsey by the [product theorem for Euclidean Ramsey sets](../../../../../product-theorem-for-euclidean-ramsey-sets.md). A monochromatic copy of that product contains the corresponding approximate copy of $X$, completing the proof.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 130](../../paper-130-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
