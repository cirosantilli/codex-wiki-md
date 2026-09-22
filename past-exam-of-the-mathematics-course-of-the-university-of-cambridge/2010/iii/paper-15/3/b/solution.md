<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use [coordinate charts](../../../../../../manifold-chart.md) from the chosen [oriented atlas](../../../../../../oriented-atlas.md). In each, the matrix $G_x=(g_{ij})$ of the [Riemannian metric](../../../../../../riemannian-metric.md) is smooth and [positive-definite](../../../../../../positive-definite-bilinear-form.md), so $\det G_x>0$ and its positive square root is smooth. Define the local [Riemannian volume form](../../../../../../riemannian-volume-form.md) by

$$
\omega_{g,x}=\sqrt{\det G_x}\,dx^1\wedge\cdots\wedge dx^n.
$$

If $y$ is another positive [coordinate chart](../../../../../../manifold-chart.md) and $J=\partial x/\partial y$, the transformation rule for the [metric tensor](../../../../../../metric-tensor.md) is $G_y=J^TG_xJ$. Taking [determinants](../../../../../../determinant.md) gives

$$
\det G_y=(\det J)^2\det G_x,
\qquad \sqrt{\det G_y}=|\det J|\sqrt{\det G_x}.
$$

The [oriented atlas](../../../../../../oriented-atlas.md) has $\det J>0$, so the [wedge product of differential forms](../../../../../../wedge-product-of-differential-forms.md) transformation from part (a) gives

$$
\sqrt{\det G_y}\,dy^1\wedge\cdots\wedge dy^n
=\sqrt{\det G_x}\,dx^1\wedge\cdots\wedge dx^n.
$$

The local expressions therefore glue to a global smooth top-degree [differential form](../../../../../../differential-form-split.md). Its local coefficient never vanishes, so it is a [volume form](../../../../../../volume-form.md). **The global answer is $\boxed{\omega_g=\sqrt{\det(g_{ij})}\,dx^1\wedge\cdots\wedge dx^n}$ in positive charts.** In an arbitrary negatively oriented chart the corresponding expression needs a minus sign; the orientation is essential to the form, although a positive metric volume density exists without it.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
