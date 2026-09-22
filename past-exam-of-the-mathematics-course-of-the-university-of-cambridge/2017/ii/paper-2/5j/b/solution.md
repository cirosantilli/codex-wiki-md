<h1 id="5j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [orthogonal projections](../../../../../../orthogonal-projection.md) of the [Gaussian noise](../../../../../../gaussian-noise.md) onto the column space of $X$ and its [orthogonal complement](../../../../../../orthogonal-complement.md) are [independent](../../../../../../independent-random-variables.md). Consequently $\widehat\beta_0$ and the residual sum of squares are [independent](../../../../../../independent-random-variables.md), and

$$
Z=\frac{\widehat\beta_0-\beta_0}{\sigma\sqrt{V_{00}}}\sim N(0,1),\qquad
U=\frac{\nu s^2}{\sigma^2}\sim\chi^2_\nu.
$$

Thus under the alternative,

$$
\boxed{T=\frac{Z+\delta}{\sqrt{U/\nu}},\qquad\delta=\frac{\beta_0}{\sigma\sqrt{V_{00}}},\quad Z\perp U.}
$$

This is the [noncentral t-distribution](../../../../../../noncentral-t-distribution.md). The rejection region is fixed by the design, $\nu$ and the chosen level, while this [probability distribution](../../../../../../probability-distribution.md) depends on $\beta$ only through $\beta_0$. Therefore **the [statistical power](../../../../../../statistical-power.md) does not depend on the other regression coefficients**, with the design and $\sigma$ fixed.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5J](../../5j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
