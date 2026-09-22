<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

In the [integral](../../../../integral-split.md) from part (d), set $y=\sinh^2u$. Its upper endpoint is $u_x=\operatorname{arsinh}\sqrt x$, equal to $\theta/2$ in part (b). The [hyperbolic function](../../../../hyperbolic-function.md) identity

$$
\left(\frac{y}{1+y}\right)^{3/2}dy
=2\frac{\sinh^4u}{\cosh^2u}\,du
=2(\cosh^2u-2+\operatorname{sech}^2u)\,du
$$

gives the [antiderivative](../../../../antiderivative.md)

$$
I(x)=\left[\frac12\sinh(2u)-3u+2\tanh u\right]_0^{u_x}
=\sqrt{x(1+x)}+2\sqrt{\frac{x}{1+x}}-3\operatorname{arsinh}\sqrt x.
$$

Multiplication by $\delta_1$ therefore yields

$$
\boxed{\delta_2(x)=1+\frac3x-3\sqrt{\frac{1+x}{x^3}}\operatorname{arsinh}\sqrt x
=1+\frac3x-3\sqrt{\frac{1+x}{x^3}}\ln(\sqrt x+\sqrt{1+x}).}
$$

At small $x$, cancellation between the terms leaves the [Taylor series](../../../../taylor-series.md) $\delta_2=2x/5-8x^2/35+16x^3/105+O(x^4)$. At large $x$, $\operatorname{arsinh}\sqrt x=\tfrac12\ln(4x)+O(x^{-1})$, so the correction to one is $[3-\tfrac32\ln(4x)]/x+O(\ln x/x^2)$. Both checks agree with part (d); the [integral](../../../../integral-split.md) or the small-$x$ [Taylor series](../../../../taylor-series.md) is preferable to subtracting large nearly equal terms in a numerical evaluation near zero.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the cosmology course of the University of Oxford](../../../split.md)
5. [Cosmology course of the University of Oxford](../../../../cosmology-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
