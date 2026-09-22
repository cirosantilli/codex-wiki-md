<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\pi:G\to G/[G,G]$ be the [abelianization](../../../../../../abelianization.md) map. Its image $\pi(A)$ is again a $K$-[approximate group](../../../../../../approximate-group.md). Apply the large-progression form of the [Freiman-Green-Ruzsa theorem](../../../../../../freiman-ruzsa-theorem.md) to $\pi(A)$. It gives a finite subgroup $H$, elements $x_1,\ldots,x_r$, and lengths $L_1,\ldots,L_r$, with

$$
r\leq K^{O(1)},\qquad
HP(x_1,\ldots,x_r;L_1,\ldots,L_r)\subseteq\pi(A^4),
$$

and

$$
|HP|\geq\exp(-K^{O(1)})|\pi(A)|.
$$

The [large lifted product from a coset progression](../../../../../../large-lifted-product-from-a-coset-progression.md) applied to this progression gives

$$
\left|
\bigl(A^{16}\cap\pi^{-1}(H)\bigr)
\prod_{i=1}^r\bigl(A^{22}\cap\pi^{-1}(\langle x_i\rangle)\bigr)
\right|
\geq \exp(-K^{O(1)})|A|.
$$

Briefly, choose a section of $\pi$ on $\pi(A^6)$. Multiplication by that section is multiplicative up to $A^{12}\cap[G,G]$; lifting successively the subgroup part and each progression direction therefore places every element of $A^6\cap\pi^{-1}(HP)$ in the displayed product. The [fiber-counting lemma for a quotient map](../../../../../../fiber-counting-lemma-for-a-quotient-map.md) gives $|A^6\cap\pi^{-1}(HP)|\geq\exp(-K^{O(1)})|A|$, which proves the estimate.

Set

$$
A_0=A^{16}\cap\pi^{-1}(H),\qquad
A_i=A^{22}\cap\pi^{-1}(\langle x_i\rangle)\quad(1\leq i\leq r).
$$

The [intersection of an approximate group power with a subgroup](../../../../../../intersection-of-an-approximate-group-power-with-a-subgroup.md) shows that each $A_i$ is a $K^{O(1)}$-approximate group contained in $A^{O(1)}$. The preimage of a [cyclic subgroup](../../../../../../cyclic-subgroup.md) of $G/[G,G]$ has step less than $s$. The same is true of the preimage of the finite subgroup $H$ because $G$ is a [torsion-free group](../../../../../../torsion-free-group.md). Consequently each $\langle A_i\rangle$ has step less than $s$, and the displayed estimate is the required conclusion.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 149](../../../paper-149-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
