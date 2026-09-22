<h1 id="10a/solution">Solution</h1>

↑ **Parent:** [10A](../10a.md)

Choose coordinates that measure the curved boundary and the slope of a ray:

$$
\boxed{u=xy^2,\qquad v=y/x.}
$$

On the positive interior, the inverse [change of variables](../../../../../change-of-variables-formula.md) is

$$
x=u^{1/3}v^{-2/3},\qquad y=u^{1/3}v^{1/3}.
$$

The two rays become $v=a$ and $v=1$, while the curve becomes $u=1$. The interior of $S$ therefore maps to the rectangle $0<u<1$, $a<v<1$. For $a=0$, the lower edge $v=0$ describes a limiting boundary, since the original region is unbounded; the origin also has no uniquely defined ratio $y/x$. For $a=1$ the region has zero area. These endpoint cases do not invalidate the [change of variables](../../../../../change-of-variables-formula.md) on the positive interior.

For the three-dimensional [integral](../../../../../integral.md), retain $z$ as the third coordinate. The transformed region is

$$
0<z<1,\qquad z<v<1,\qquad0<u<1.
$$

The planar [Jacobian determinant](../../../../../jacobian-determinant.md) is

$$
\frac{\partial(u,v)}{\partial(x,y)}
=\det\begin{pmatrix}y^2&2xy\\-y/x^2&1/x\end{pmatrix}
=\frac{3y^2}{x},\qquad
\left|\frac{\partial(x,y)}{\partial(u,v)}\right|=\frac{x}{3y^2}.
$$

The integrand cancels this [Jacobian determinant](../../../../../jacobian-determinant.md) especially simply:

$$
\frac{y^2z^2}{x}\,dx\,dy\,dz=\frac{z^2}{3}\,du\,dv\,dz.
$$

Hence

$$
\boxed{\int_D\frac{y^2z^2}{x}\,dx\,dy\,dz
=\frac13\int_0^1z^2(1-z)\,dz=\frac1{36}.}
$$

One can first use the [change of variables formula](../../../../../change-of-variables-formula.md) with $z\geq\varepsilon>0$ and then pass to the limit. The nonnegative integrand allows this by the [monotone convergence theorem](../../../../../monotone-convergence-theorem.md), so the unbounded limiting slice at $z=0$ causes no omitted contribution.

## ↑ Ancestors (10)

1. [10A](../10a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
