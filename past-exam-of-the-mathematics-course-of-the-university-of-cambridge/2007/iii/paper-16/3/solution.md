<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For an open subset $U\subseteq B$, let $E_U=\pi^{-1}(U)$ and define the degree-preserving module map

$$
\Phi_U:\bigoplus_{j=1}^vH^{*-k_j}(U;\mathbb Q)\longrightarrow H^*(E_U;\mathbb Q),\qquad
(b_j)_j\longmapsto\sum_j\pi^*b_j\smile c_j|_{E_U}.
$$

Using the prescribed fiber basis identifies its domain with the tensor product in the question. We prove that $\Phi_B$ is an [isomorphism](../../../../../isomorphism.md), giving the [Leray-Hirsch theorem](../../../../../leray-hirsch-theorem.md) in this setting.

First suppose $U$ is a trivializing patch. The [cohomological Künneth theorem over a field](../../../../../cohomological-kunneth-theorem-over-a-field.md) identifies $H^*(U\times F;\mathbb Q)$ with the finite free graded $H^*(U;\mathbb Q)$-module on a homogeneous basis of $H^*(F;\mathbb Q)$. The required finiteness is supplied by the finite list $c_1,\ldots,c_v$ spanning the fiber's total cohomology. Express the restrictions of the $c_j$ in this product basis. A coefficient multiplying a fiber basis element of degree $k_i$ belongs to $H^{k_j-k_i}(U;\mathbb Q)$; thus no coefficient can increase fiber degree. The degree-zero blocks are invertible on every path component, because restriction at every point gives a basis. Their inverses are again degree-zero cohomology classes.

After inverting those blocks, the remaining change-of-basis map is $I+N$, where $N$ strictly lowers fiber degree. There are only finitely many fiber degrees, so $N$ is [nilpotent](../../../../../nilpotent.md) and $(I+N)^{-1}=I-N+N^2-\cdots$ is a finite sum. This proves the [local basis criterion for Leray-Hirsch classes](../../../../../local-basis-criterion-for-leray-hirsch-classes.md) and therefore the isomorphism on every trivializing patch, without requiring the patch to be contractible.

Now use a finite trivializing open cover $U_1,\ldots,U_r$, supplied by [compactness](../../../../../compact-space.md) of $B$. Induct on $r$. Put $U=U_1\cup\cdots\cup U_{r-1}$ and $V=U_r$. The intersection $U\cap V$ is covered by the at most $r-1$ trivializing open sets $U_i\cap V$, so the induction hypothesis applies to $U$, $V$ and $U\cap V$.

Take the direct sum of shifted [Mayer–Vietoris sequences](../../../../../mayer-vietoris-sequence.md) for the base and compare it with the sequence for $E_U\cup E_V$. Restriction commutes with multiplication by each global [cohomology class](../../../../../cohomology-class.md) $c_j$. The connecting homomorphism also commutes: multiply the cochain representatives on the right by the restriction of a global cocycle representing $c_j$, and use $d(b\smile c_j)=db\smile c_j$. Consequently the maps $\Phi$ form a morphism of exact sequences. The [Five lemma](../../../../../five-lemma.md) makes $\Phi_{U\cup V}$ an isomorphism, completing the [finite-cover proof of the Leray-Hirsch theorem](../../../../../finite-cover-proof-of-the-leray-hirsch-theorem.md).

This is an additive graded module isomorphism. It does not assert that the fiber classes have the same multiplicative relations in the total space.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 16](../../paper-16-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
