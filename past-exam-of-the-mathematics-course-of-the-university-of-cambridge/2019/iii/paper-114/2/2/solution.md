<h1 id="2/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Every [singular simplex](../../../../../../singular-simplex.md) has compact image, and a [singular chain](../../../../../../singular-chain.md) is a finite sum of simplices. The image of any chain is therefore compact and lies in some $X_a$. Directedness puts any finite collection of chains into one common $X_b$, so

$$
C_*(X;\mathbb Z)=\varinjlim_aC_*(X_a;\mathbb Z).
$$

Because [filtered colimits](../../../../../../filtered-colimit-of-modules.md) of [abelian groups](../../../../../../abelian-group.md) are exact, kernels and images commute with this colimit. Taking homology gives the [homology of a directed union](../../../../../../homology-of-a-directed-union.md):

$$
\boxed{H_i(X;\mathbb Z)\cong\varinjlim_aH_i(X_a;\mathbb Z).}
$$

For an open $U\subseteq\mathbb R^N$, use the directed family of finite unions of closed rational cubes contained in $U$. Every compact subset of $U$ lies in one such finite polyhedron, and each polyhedron has finitely generated [cellular homology](../../../../../../cellular-chain-complex.md). There are only countably many of them, so their direct limit is countable. Thus **every $H_i(U;\mathbb Z)$ is countable**.

Cohomology behaves differently because $\operatorname{Hom}$ turns a direct sum into a direct product. The connected open set

$$
U=\mathbb R^2\setminus\{(n,0):n\geq1\}
$$

has one independent loop around each puncture, so $H_1(U;\mathbb Z)\cong\bigoplus_{n\geq1}\mathbb Z$. Since $H_0(U;\mathbb Z)=\mathbb Z$, the [universal coefficient theorem for cohomology](../../../../../../universal-coefficient-theorem-for-cohomology.md) gives

$$
\boxed{H^1(U;\mathbb Z)\cong\operatorname{Hom}\left(\bigoplus_{n\geq1}\mathbb Z,\mathbb Z\right)
\cong\prod_{n\geq1}\mathbb Z,}
$$

which is uncountable. This is the [first cohomology of the countably punctured plane](../../../../../../first-cohomology-of-the-countably-punctured-plane.md).

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2](../../2.md)
3. [Paper 114](../../../paper-114-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
