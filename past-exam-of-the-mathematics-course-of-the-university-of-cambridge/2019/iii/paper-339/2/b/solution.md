<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a proper three-[graph colouring](../../../../../../graph-coloring.md) $c$, associate the colors with the three [roots of unity](../../../../../../root-of-unity.md) $d(i)=\exp(2\pi i(c(i)-1)/3)$, viewed as [unit vectors](../../../../../../unit-vector.md) in $\mathbb R^2$. Define $U_{ij}=2\langle d(i),d(j)\rangle$ using the real [inner product](../../../../../../inner-product.md).

This is twice a [Gram matrix](../../../../../../gram-matrix.md), so it is a [positive semidefinite matrix](../../../../../../positive-semidefinite-matrix.md). Its diagonal is $2$. On every [edge](../../../../../../edge-of-a-graph.md), the endpoint colors differ, so their [vectors](../../../../../../vector.md) make angle $2\pi/3$ or $4\pi/3$ and $U_{ij}=2\cos(2\pi/3)=-1$. Thus $t=3$ and this $U$ are feasible in the second [semidefinite program](../../../../../../semidefinite-programming.md), proving

$$
\boxed{\bar\vartheta(G)\leq3.}
$$

This is the [regular simplex](../../../../../../regular-simplex.md) construction of a [strict vector coloring](../../../../../../strict-vector-coloring.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
