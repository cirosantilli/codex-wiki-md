<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

First, the inverse [metric tensor](../../../../../../metric-tensor.md) printed in the PDF has a missing factor: its lower-left entry must be $g^{i0}=\alpha^{-2}\beta^i$, symmetric with $g^{0i}$. This correction follows either from symmetry or direct block multiplication and does not change the evolution equation used here.

Let $D_t=\partial_t-\beta^k\partial_k$. Contract the spatial [metric tensor](../../../../../../metric-tensor.md) evolution equation with $\gamma^{ij}$. Both shift-gradient terms contribute $\partial_k\beta^k$, giving

$$
\gamma^{ij}D_t\gamma_{ij}-2\partial_k\beta^k=-2\alpha\gamma^{ij}K_{ij}=-2\alpha K.
$$

The [Jacobi determinant derivative formula](../../../../../../jacobi-determinant-derivative-formula.md) applies to every derivative of $\gamma=\det(\gamma_{ij})$ and gives $D_t\gamma=\gamma\gamma^{ij}D_t\gamma_{ij}$. Therefore **the spatial determinant evolves as**

$$
\boxed{\partial_t\gamma-\beta^k\partial_k\gamma-2\gamma\partial_k\beta^k=-2\alpha\gamma K.}
$$

Equivalently, the [spatial volume evolution identity](../../../../../../spatial-volume-evolution-identity.md) is $D_t\sqrt\gamma=\sqrt\gamma(\partial_k\beta^k-\alpha K)$, with $K$ the trace of the [extrinsic curvature of a spatial hypersurface](../../../../../../extrinsic-curvature-of-a-spatial-hypersurface.md).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 52](../../../paper-52-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
