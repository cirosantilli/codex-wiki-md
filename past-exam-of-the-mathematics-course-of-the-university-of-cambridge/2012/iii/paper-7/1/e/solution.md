<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For the [free transport equation](../../../../../../free-transport-equation.md), the [mixed Lebesgue norm](../../../../../../mixed-lebesgue-norm.md) dispersion estimate is

$$
\boxed{\|f(t)\|_{L_x^\infty L_v^1}
\leq |t|^{-d}\|f_{\mathrm{in}}\|_{L_x^1L_v^\infty},\qquad t\ne0.}
$$

Indeed, use the [method of characteristics](../../../../../../method-of-characteristics.md) and then the [change of variables](../../../../../../change-of-variables-formula.md) $y=x-tv$:

$$
\int |f_{\mathrm{in}}(x-tv,v)|\,dv
=|t|^{-d}\int
\left|f_{\mathrm{in}}\left(y,\frac{x-y}{t}\right)\right|dy
\leq |t|^{-d}\int\sup_w|f_{\mathrm{in}}(y,w)|\,dy.
$$

Taking the [essential supremum](../../../../../../essential-supremum.md) over $x$ proves the result. This decay measures the spreading of a velocity average; the total [phase space](../../../../../../phase-space.md) [Lp norm](../../../../../../lp-norm.md) is conserved rather than decaying. The datum on the right is the initial datum, not the solution at the same time.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
