<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

First account for the unlabelled coefficient-sequence construction. The two [short exact sequences](../../../../../../short-exact-sequence.md) of [abelian groups](../../../../../../abelian-group.md) are

$$
0\longrightarrow\mathbb Z\xrightarrow{\,n\,}\mathbb Z\xrightarrow{\widehat\alpha}\mathbb Z/n\longrightarrow0,
\qquad
0\longrightarrow\mathbb Z/n\xrightarrow{\,j\,}\mathbb Z/n^2\xrightarrow{\alpha}\mathbb Z/n\longrightarrow0,
\quad j([a])=[na].
$$

The [singular chain groups](../../../../../../singular-chain-group.md) of $X$ are free abelian. Applying $\operatorname{Hom}(C_q(X),-)$ therefore preserves these exact sequences, degree by degree, giving [short exact sequences of cochain complexes](../../../../../../short-exact-sequence-of-cochain-complexes.md). The associated [long exact sequence from a coefficient sequence](../../../../../../long-exact-sequence-from-a-coefficient-sequence.md) gives the displayed maps in [cohomology](../../../../../../cohomology-split.md); the connecting maps are the [integral Bockstein homomorphism](../../../../../../integral-bockstein-homomorphism.md) $\widehat\beta$ and the modulo-$n$ [Bockstein homomorphism](../../../../../../bockstein-homomorphism.md) $\beta$. The first omitted map is multiplication by $n$, and the second is induced by $j$.

For the requested example, attach an $(i+1)$-cell to $S^i$ using a map of degree $n$. The resulting [Moore space](../../../../../../moore-space-algebraic-topology.md) $X=M(\mathbb Z/n,i)$ has positive-degree [cellular chain complex](../../../../../../cellular-chain-complex.md)

$$
0\longrightarrow\mathbb Z\xrightarrow{\,n\,}\mathbb Z\longrightarrow0
$$

in degrees $i+1,i$. This construction also works for $i=1$, using the degree-$n$ map of the circle. In [cellular cohomology](../../../../../../cellular-cohomology.md) with coefficients $\mathbb Z/n$, the differential is zero, so both $H^i$ and $H^{i+1}$ are $\mathbb Z/n$.

Lift the cochain taking value $1$ on the $i$-cell to a cochain with coefficients $\mathbb Z/n^2$. Its coboundary takes value $n$ on the $(i+1)$-cell, which is $j(1)$. The definition of the [connecting homomorphism](../../../../../../connecting-homomorphism.md) therefore sends the degree-$i$ generator to the degree-$(i+1)$ generator. Hence

$$
\boxed{\beta:H^i(M(\mathbb Z/n,i);\mathbb Z/n)\xrightarrow{\ \cong\ }H^{i+1}(M(\mathbb Z/n,i);\mathbb Z/n).}
$$

It is nonzero for every $i\geq1$ and $n\geq2$, including composite $n$. This is the [Bockstein on a cyclic Moore space](../../../../../../bockstein-on-a-cyclic-moore-space.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 114](../../../paper-114-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
