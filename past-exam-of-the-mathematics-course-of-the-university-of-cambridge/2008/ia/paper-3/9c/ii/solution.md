<h1 id="9c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The derivative [matrix](../../../../../../matrix.md)

$$
\partial_jF_k=\omega_k\omega_j-|\boldsymbol\omega|^2\delta_{kj}
$$

is symmetric in $j,k$. Contracting it with the antisymmetric [Levi-Civita symbol](../../../../../../levi-civita-symbol.md) gives the [curl](../../../../../../curl.md)

$$
(\nabla\times\mathbf F)_i=\epsilon_{ijk}(\omega_k\omega_j-|\boldsymbol\omega|^2\delta_{kj})=0.
$$

Direct differentiation of the [scalar potential](../../../../../../scalar-potential.md) gives

$$
\partial_i\phi=\omega_i(\boldsymbol\omega\cdot\mathbf x)-|\boldsymbol\omega|^2x_i=F_i,
$$

so **$\mathbf F=\nabla\phi$**. To identify the [level sets](../../../../../../level-set.md), use the [cross product](../../../../../../cross-product.md) identity

$$
\phi=-\tfrac12|\boldsymbol\omega\times\mathbf x|^2.
$$

If $\boldsymbol\omega\ne0$, write $\mathbf x=\mathbf x_{\parallel}+\mathbf x_{\perp}$ relative to its direction. Then $\phi=-|\boldsymbol\omega|^2|\mathbf x_{\perp}|^2/2$. Thus **each negative level $\phi=c$ is a [circular cylinder](../../../../../../circular-cylinder.md) with axis $\mathbb R\boldsymbol\omega$ and radius $\sqrt{-2c}/|\boldsymbol\omega|$**. The zero level is the axis itself; positive levels are empty. If $\boldsymbol\omega=0$, the [scalar potential](../../../../../../scalar-potential.md) is identically zero, so its zero level is all of space and every other level is empty.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [9C](../../9c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
