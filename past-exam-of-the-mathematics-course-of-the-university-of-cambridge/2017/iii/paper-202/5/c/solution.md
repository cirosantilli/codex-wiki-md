<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Integrating the stopped [stochastic differential equation](../../../../../../stochastic-differential-equation.md) for $Y$ and then taking a common full-probability event for a [localizing sequence](../../../../../../localizing-sequence.md) gives, simultaneously for every $t<T$,

$$
Y_t=\sqrt{x_0}+\frac12B_t-\frac18\int_0^t\frac{ds}{Y_s}.
$$

The integral is finite on each compact time interval before $T$: the continuous positive path has a positive minimum there. Its integrand is nonnegative, so

$$
\boxed{W_t-Y_t=\frac18\int_0^tY_s^{-1}\,ds\geq0\quad\text{for every }0\leq t<T\text{ almost surely}.}
$$

This is a pathwise comparison using the same [Brownian motion](../../../../../../brownian-motion-split.md), not a comparison of independent distributions. Continuity lets the identities established initially at rational stopped times hold on the entire [stochastic interval](../../../../../../stochastic-interval.md).

## ↑ Ancestors (11)

1. [C](../c.md)
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
