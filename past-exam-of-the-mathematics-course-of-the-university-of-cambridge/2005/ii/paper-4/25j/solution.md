<h1 id="25j/solution">Solution</h1>

↑ **Parent:** [25J](../25j.md)

The [Fubini theorem](../../../../../fubini-s-theorem.md) for an integrable Borel-measurable function states that, if $\int_{\mathbb R^2}|f|<\infty$, its sections are integrable for almost every coordinate and

$$
\int_{\mathbb R^2}f\,d(x,y)
=\int_{\mathbb R}\left(\int_{\mathbb R}f(x,y)\,dx\right)dy
=\int_{\mathbb R}\left(\int_{\mathbb R}f(x,y)\,dy\right)dx.
$$

For a nonnegative measurable function, [Tonelli theorem](../../../../../tonelli-theorem.md) gives the same equalities with infinity allowed before integrability is established.

Here $f$ is the [continuous](../../../../../continuous-function.md) exponential multiplied by the indicator of a [Borel set](../../../../../borel-set.md), so it is Borel-measurable and nonnegative. Tonelli and integration in $x$ give

$$
\int_{\mathbb R^2}f=\int_a^b\int_0^\infty e^{-xy}\,dx\,dy
=\int_a^b\frac{dy}{y}=\log(b/a)<\infty.
$$

This proves integrability. We may now integrate in the reverse order; for $x>0$ the inner integral is $(e^{-ax}-e^{-bx})/x$. Hence the [Frullani integral](../../../../../frullani-integral.md) is

$$
\boxed{\int_0^\infty\frac{e^{-ax}-e^{-bx}}x\,dx=\log\frac ba}.
$$

The apparent singularity at zero is removable in the integrand's limiting value $b-a$.

## ↑ Ancestors (10)

1. [25J](../25j.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
