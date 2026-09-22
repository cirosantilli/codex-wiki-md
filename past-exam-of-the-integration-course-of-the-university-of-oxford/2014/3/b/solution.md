<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assign any value, for example zero, at $(0,0)$, where the displayed quotient is undefined. A single point is a [Lebesgue null set](../../../../lebesgue-null-set.md), so this choice does not affect [Lebesgue integrability](../../../../integrability.md). Elsewhere the [function](../../../../function-split.md) is continuous, hence it is [Lebesgue measurable](../../../../lebesgue-measurable-set.md) on the plane after this extension.

In [polar coordinates](../../../../polar-coordinates.md), $x^2+y^2=r^2$ and the area element is $r\,dr\,d\theta$. Applying the nonnegative [change of variables formula](../../../../change-of-variables-formula.md) to the [absolute value](../../../../absolute-value.md) gives

$$
\int_{\mathbb R^2}|k(x,y)|\,dx\,dy
=2\pi\int_0^\infty|\sin(r^2)|r^{1-2\alpha}\,dr.
$$

For $0<r\leq1$, $|\sin(r^2)|\leq r^2$, so the radial [integrand](../../../../integrand.md) is bounded by $r^{3-2\alpha}$. This is integrable at zero when $\alpha<2$. For $r\geq1$, $|\sin(r^2)|\leq1$, giving the integrable tail bound $r^{1-2\alpha}$ when $\alpha>1$. In particular,

$$
\begin{aligned}
\|k\|_1
&\leq2\pi\left(\int_0^1r^{3-2\alpha}\,dr+\int_1^\infty r^{1-2\alpha}\,dr\right)\\
&=\pi\left(\frac1{2-\alpha}+\frac1{\alpha-1}\right)<\infty.
\end{aligned}
$$

Therefore

$$
\boxed{k\in L^1(\mathbb R^2)\qquad(1<\alpha<2).}
$$

Equivalently, the [substitution rule](../../../../integration-by-substitution.md) $u=r^2$ reduces its exact [L1 norm](../../../../l1-norm.md) to

$$
\|k\|_1=\pi\int_0^\infty\frac{|\sin u|}{u^\alpha}\,du.
$$

This is [radial sine-power kernel integrability](../../../../radial-sine-power-kernel-integrability.md), reducing a two-dimensional question to the [sine power kernel integrability](../../../../sine-power-kernel-integrability.md) thresholds at zero and infinity.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the integration course of the University of Oxford](../../../split.md)
5. [Integration course of the University of Oxford](../../../../integration-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
