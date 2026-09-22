<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a [holomorphic function](../../../../../holomorphic-function-split.md), the derivative supplied by [complex differentiability](../../../../../complex-differentiability.md) must have the same value along real and imaginary increments. Those two computations give

$$
f'(z)=u_x+iv_x=\frac{u_y+iv_y}{i}=v_y-iu_y.
$$

Equating real and imaginary parts proves the [Cauchy-Riemann equations](../../../../../cauchy-riemann-equations.md):

$$
\boxed{u_x=v_y,\qquad u_y=-v_x.}
$$

Conversely, if the first partial [derivatives](../../../../../derivative.md) are continuous near a point and obey these equations there, real differentiability gives

$$
f(z+h)-f(z)=(u_x+iv_x)\operatorname{Re}h+(u_y+iv_y)\operatorname{Im}h+o(|h|)=f'(z)h+o(|h|),
$$

which proves complex differentiability under this regularity assumption.

The [gradients](../../../../../gradient.md) of the real and imaginary parts have [dot product](../../../../../dot-product.md)

$$
\nabla u\cdot\nabla v=u_xv_x+u_yv_y=v_yv_x-v_xv_y=0,
$$

and $|\nabla u|^2=|\nabla v|^2=|f'(z)|^2$. At every point with $f'(z)\ne0$, the two [level sets](../../../../../level-set.md) are regular curves, their [gradients](../../../../../gradient.md) are nonzero [normal vectors](../../../../../normal-vector.md), and their tangent directions are therefore perpendicular.

The printed phrase "at every point" needs this regular-point qualification. At a [critical point](../../../../../critical-point.md) with $f'(z)=0$, the [level sets](../../../../../level-set.md) may cross or fail to have a unique tangent. For example, $f(z)=z^2$ gives $u=x^2-y^2$ and $v=2xy$: at the origin the zero [level sets](../../../../../level-set.md) are respectively the diagonals and the coordinate axes. Thus the valid conclusion is $\boxed{\text{orthogonality at every regular intersection, where }f'(z)\ne0}$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [7](../../7.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
