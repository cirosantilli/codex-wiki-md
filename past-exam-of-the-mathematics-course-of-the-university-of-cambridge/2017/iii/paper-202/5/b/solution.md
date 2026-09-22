<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Before the lifetime, $X>0$, so apply the [Itô formula](../../../../../../ito-s-lemma.md) to $g(x)=\sqrt{x}$ after stopping inside compact subintervals of $(0,\infty)$. The derivatives are $g'(x)=1/(2\sqrt{x})$ and $g''(x)=-1/(4x^{3/2})$. Since the [quadratic variation](../../../../../../quadratic-variation.md) of $X$ satisfies $d[X]_t=X_tdt$, we get

$$
\boxed{dY_t=\frac12\,dB_t-\frac1{8Y_t}\,dt,\qquad Y_0=\sqrt{x_0},\quad t<T.}
$$

The negative drift is the second-order correction in the [Itô formula](../../../../../../ito-s-lemma.md). This is a [Lamperti transform](../../../../../../lamperti-transform-diffusion.md) up to a constant scale: the [square root](../../../../../../square-root.md) transformation makes the noise coefficient constant. Its drift is singular at zero, which is why this [stochastic differential equation](../../../../../../stochastic-differential-equation.md) is stated only before the boundary lifetime.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
