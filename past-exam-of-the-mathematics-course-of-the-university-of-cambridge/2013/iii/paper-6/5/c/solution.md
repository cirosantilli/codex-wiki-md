<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Interpret $L$ as the velocity operator appearing in the equation and in the stated quadratic-form hypothesis. Let $E(t)=\int\!\!\int|f(t,x,v)|^2\,dx\,dv$. Smoothness turns the distributional equation into the usual equation. Multiply it by $f$ and integrate; for complex functions use the real part of the [inner product](../../../../../../inner-product.md). Spatial [integration by parts](../../../../../../integration-by-parts.md) gives $\int v\cdot\nabla_x(f^2)=0$, while the coercivity hypothesis at each $x$ gives

$$
\frac12E'(t)=-\int\!\!\int (Lf)f\,dv\,dx\leq-\delta E(t).
$$

Thus $e^{2\delta t}E(t)$ is nonincreasing. The [coercive energy estimate for kinetic transport](../../../../../../coercive-energy-estimate-for-kinetic-transport.md) is

$$
\boxed{\|f(t_2)\|_2\leq e^{-\delta(t_2-t_1)}\|f(t_1)\|_2,\qquad t_1\leq t_2}.
$$

No division by $E$ is required, so the zero solution causes no exception. Compact spatial support, or sufficient decay to eliminate the boundary flux, is enough; [compact support](../../../../../../compact-support.md) in time is unnecessary.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
