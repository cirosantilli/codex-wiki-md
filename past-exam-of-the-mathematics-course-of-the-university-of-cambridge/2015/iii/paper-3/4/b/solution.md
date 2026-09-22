<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An [algebraic group](../../../../../../algebraic-group.md) is [connected](../../../../../../connected-space.md) when its underlying [Zariski topology](../../../../../../zariski-topology.md) is a [connected space](../../../../../../connected-space.md). An [unipotent algebraic group](../../../../../../unipotent-algebraic-group.md) is a [linear algebraic group](../../../../../../linear-algebraic-group.md) whose elements, in a faithful matrix realization, satisfy that $u-I$ is nilpotent. A [reductive algebraic group](../../../../../../reductive-group.md), in the connected convention, is a [connected](../../../../../../connected-space.md) [linear algebraic group](../../../../../../linear-algebraic-group.md) whose [unipotent radical](../../../../../../unipotent-radical.md) is trivial: it has no nontrivial connected normal unipotent algebraic subgroup.

Let $E=\operatorname{End}_Q(X)$. It is a finite-dimensional associative algebra, and $\operatorname{Aut}_Q(X)=E^\times$. The latter is the nonempty open subset where the determinant on $\bigoplus_iX_i$ is nonzero. Since the affine space $E$ is irreducible, this open subset is irreducible and hence connected. It is a [linear algebraic group](../../../../../../linear-algebraic-group.md): within $\operatorname{GL}(\bigoplus_iX_i)$ it is cut out by the linear equations of preserving the vertex summands and commuting with the arrow maps. Thus **the automorphism group is connected**.

By the [Krull–Schmidt theorem](../../../../../../krull-schmidt-theorem.md), write $X\cong\bigoplus_{a=1}^sM_a^{\oplus m_a}$, with pairwise nonisomorphic indecomposables $M_a$. The [Fitting lemma](../../../../../../fitting-lemma.md) makes each $\operatorname{End}_Q(M_a)$ a local algebra. Its residue division algebra is $k$: every element of a finite-dimensional division algebra over the algebraically closed field has an eigenvalue for left multiplication, and subtracting that scalar gives a noninvertible element, hence zero.

The standard radical description of the endomorphism algebra of a [Krull-Schmidt decomposition](../../../../../../krull-schmidt-decomposition.md) therefore gives

$$
E/J(E)\cong\prod_{a=1}^s\operatorname{Mat}_{m_a}(k).
$$

Concretely, maps between nonisomorphic summands lie in the radical, while on each isotypic block one reduces all entries modulo the local radical. The off-diagonal rule follows because a composition $M_a\to M_b\to M_a$ cannot be a unit for $a\ne b$: it would split $M_a$ off the indecomposable $M_b$, forcing an isomorphism. The finite-dimensional radical description then identifies the kernel of this block reduction with $J(E)$. Put $U=1+J(E)$. The [Jacobson radical](../../../../../../jacobson-radical.md) of the finite-dimensional algebra is nilpotent, so every $1+j$ is a unit and is unipotent on $\bigoplus_iX_i$. Also $U$ is closed, being the translate of the linear subspace $J(E)$, and normal, being the kernel of

$$
E^\times\longrightarrow\prod_a\operatorname{GL}_{m_a}(k).
$$

This map has an explicit algebraic section: after fixing the direct-sum decomposition, a matrix $B_a$ acts on the $m_a$ copies by $B_a\otimes1_{M_a}$. These block actions give a subgroup $L\cong\prod_a\operatorname{GL}_{m_a}(k)$ with trivial intersection with $U$. Every unit is uniquely a product of an element of $U$ and one of $L$. Hence

$$
\boxed{\operatorname{Aut}_Q(X)\cong(1+J(E))\rtimes\prod_{a=1}^s\operatorname{GL}_{m_a}(k).}
$$

This [Levi decomposition of a quiver automorphism group](../../../../../../levi-decomposition-of-a-quiver-automorphism-group.md) holds in every characteristic; the section is constructed directly from the multiplicity spaces.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
