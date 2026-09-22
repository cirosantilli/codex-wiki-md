<h1 id="b/7/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

We calculate the exact multiplicity without using [Young's rule](../../../../../young-s-rule.md), via a [two-subset incidence realization of a two-row Specht module](../../../../../two-subset-incidence-realization-of-a-two-row-specht-module.md). Let $V_2$ be the [permutation](../../../../../permutation.md) [representation](../../../../../group-representation.md) on unordered pairs from a six-element set, and $V_1$ the natural [permutation](../../../../../permutation.md) [representation](../../../../../group-representation.md) on its singletons. The equivariant incidence map

$$
D:V_2\to V_1,\qquad e_{ij}\longmapsto e_i+e_j
$$

is surjective: the transpose map sends $\sum c_ie_i$ to the pair coefficients $c_i+c_j$, and all such sums can be zero only when every $c_i=0$ in [characteristic zero](../../../../../characteristic-zero.md). Thus $\dim\ker D=15-6=9$.

Identify the [tabloids](../../../../../tabloid.md) of shape $(4,2)$ with their two-element bottom rows. A [polytabloid](../../../../../polytabloid.md) is a signed four-edge [vector](../../../../../vector.md) $e_{cd}-e_{ad}-e_{cb}+e_{ab}$, whose incidence at every vertex is zero. Hence $S^{(4,2)}\subseteq\ker D$. The [standard polytabloid](../../../../../standard-polytabloid.md) [basis](../../../../../basis.md) theorem and the [hook-length formula](../../../../../hook-length-formula.md) give $\dim S^{(4,2)}=\binom62-\binom61=9$, so equality holds. By [Maschke's theorem](../../../../../maschke-s-theorem.md),

$$
V_2\cong S^{(4,2)}\oplus V_1.
$$

Take $H=\Sigma_3\times\Sigma_2\times\Sigma_1$, preserving blocks of sizes three, two and one. It has three orbits on singletons and five on pairs: pairs inside the first block, inside the second, and between each of the three distinct pairs of blocks. Thus $\dim V_1^H=3$ and $\dim V_2^H=5$. Averaging over $H$ makes taking fixed [vectors](../../../../../vector.md) exact in [characteristic zero](../../../../../characteristic-zero.md), so $\dim(S^{(4,2)})^H=2$.

Finally $M^{(3,2,1)}=\operatorname{Ind}_H^{\Sigma_6}1$. [Frobenius reciprocity](../../../../../frobenius-reciprocity.md), and equality of invariant and coinvariant dimensions in [characteristic zero](../../../../../characteristic-zero.md), identify the required multiplicity with this two-dimensional fixed space. Therefore

$$
\boxed{[M^{(3,2,1)}:S^{(4,2)}]=2,}
$$

which in particular satisfies the requested lower and upper bounds.

## ↑ Ancestors (13)

1. [E](../e.md)
2. [7](../../7.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../split.md)
6. [Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../../lie-algebras-and-representation-theory-of-symmetric-groups-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
