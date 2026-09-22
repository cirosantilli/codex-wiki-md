<h1 id="b/5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [CW complex](../../../../../cw-complex.md) is built from a discrete set of zero-cells by attaching $k$-discs along maps of their boundary spheres into the previous skeleton. Its topology is the weak topology determined by the characteristic maps, and each cell closure meets only finitely many cells. The [k-skeleton](../../../../../skeleton-of-a-cw-complex.md) $X^k$ is the union of cells of dimension at most $k$, with $X^{-1}=\varnothing$.

Set $C_k^{CW}(X)=H_k(X^k,X^{k-1};\mathbb Z)$. This is the free abelian group on the $k$-cells. The [cellular boundary map](../../../../../cellular-boundary.md) is $\partial_k=q_{k-1}\delta_k$ with the maps in the question. In the long exact sequence of the pair $(X^{k-1},X^{k-2})$, the consecutive maps are

$$
H_{k-1}(X^{k-1})\xrightarrow{q_{k-1}}H_{k-1}(X^{k-1},X^{k-2})\xrightarrow{\delta_{k-1}}H_{k-2}(X^{k-2}).
$$

Exactness gives $\delta_{k-1}q_{k-1}=0$. Hence

$$
\boxed{\partial_{k-1}\partial_k=q_{k-2}\delta_{k-1}q_{k-1}\delta_k=0}.
$$

At the lowest indices put negative chain groups equal to zero.

The [cellular homology](../../../../../cellular-chain-complex.md) is $H_n^{CW}(X)=\ker\partial_n/\operatorname{im}\partial_{n+1}$. For a field $\mathbb F$, use $C_k^{CW}(X;\mathbb F)=H_k(X^k,X^{k-1};\mathbb F)$, the vector space with basis the $k$-cells, with the same connecting-and-quotient construction. Its homology is $H_n^{CW}(X;\mathbb F)$. Equivalently tensor the integral free [cellular chain complex](../../../../../cellular-chain-complex.md) with $\mathbb F$. The [cellular homology theorem](../../../../../cellular-homology-theorem.md) identifies these with [singular homology](../../../../../singular-homology.md) using the same coefficients.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the topology and Groups and Algebraic Topology course of the University of Oxford](../../../../split.md)
6. [Topology and Groups and Algebraic Topology course of the University of Oxford](../../../../../topology-and-groups-and-algebraic-topology-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
