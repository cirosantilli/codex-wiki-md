<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [product Riemannian metric](../../../../../../product-riemannian-metric.md) has block matrix

$$
g=\begin{pmatrix}g_M(x)&0\\0&g_N(y)\end{pmatrix},\qquad g^{-1}=\begin{pmatrix}g_M(x)^{-1}&0\\0&g_N(y)^{-1}\end{pmatrix}.
$$

In the given [Christoffel symbols](../../../../../../christoffel-symbol.md) formula, every mixed coefficient vanishes. Off-diagonal metric entries are zero, $\partial_{y^\alpha}g_{ij}=0$, and $\partial_{x^i}g_{\alpha\beta}=0$. These facts give $\Gamma^A_{i\alpha}=0$ for every output index $A$, as well as $\Gamma^\alpha_{ij}=0$ and $\Gamma^i_{\alpha\beta}=0$. The remaining pure blocks are precisely the Christoffel symbols of the respective factor metrics.

For the lifted fields of (i), $\partial_{x^i}Y^\alpha=0$. Consequently

$$
\nabla_XY=\sum_{i,\alpha}X^i\partial_{x^i}Y^\alpha\,\partial_{y^\alpha}+\sum_{A,i,\alpha}\Gamma^A_{i\alpha}X^iY^\alpha\partial_A=0.
$$

Thus $\boxed{\nabla_XY=0}$. The same calculation gives $\nabla_YX=0$; differentiating two fields from one factor gives the lifted factor covariant derivative. This identifies the product [Levi-Civita connection](../../../../../../levi-civita-connection.md) with the [product affine connection](../../../../../../product-affine-connection.md) and proves the curvature splitting used in the root solution.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 19](../../../paper-19-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
