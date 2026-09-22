<h1 id="8g/solution">Solution</h1>

↑ **Parent:** [8G](../8g.md)

The positive-definite symmetric form $b$ is a real [inner product](../../../../../inner-product.md). Choose a $b$-orthonormal [basis](../../../../../basis.md) by the [Gram-Schmidt process](../../../../../gram-schmidt-process.md). The stated identity means that the [matrix](../../../../../matrix.md) $K$ of $\psi$ satisfies $K^T=-K$. If $d=\dim U$, then

$$
\det K=\det K^T=\det(-K)=(-1)^d\det K.
$$

An invertible $K$ has nonzero [determinant](../../../../../determinant.md), so **$d$ is even**.

To cover a possibly singular map, first show $\ker\psi=(\operatorname{im}\psi)^\perp$. If $x\in\ker\psi$, then $b(x,\psi y)=-b(\psi x,y)=0$ for every $y$, giving one inclusion. Conversely orthogonality to the image gives $b(\psi x,y)=0$ for all $y$, so nondegeneracy of $b$ gives $\psi x=0$. Positivity then implies $\operatorname{im}\psi\cap\ker\psi=\{0\}$.

The image is invariant under $\psi$, and its restricted map $\psi|_{\operatorname{im}\psi}$ is injective by that trivial intersection. In finite dimension it is consequently invertible. The restricted [inner product](../../../../../inner-product.md) is positive definite and the same skew-adjoint identity holds, so the first argument applied to this restriction makes $\dim\operatorname{im}\psi$ even. Thus

$$
\boxed{\operatorname{rank}\psi\text{ is always even},}
$$

including [rank](../../../../../rank-one-quadratic-form.md) zero. This is the [even rank of a skew-adjoint linear map](../../../../../even-rank-of-a-skew-adjoint-linear-map.md).

## ↑ Ancestors (10)

1. [8G](../8g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
