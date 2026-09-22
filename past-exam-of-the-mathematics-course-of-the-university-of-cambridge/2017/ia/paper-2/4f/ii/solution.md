<h1 id="4f/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [conditional density](../../../../../../conditional-density.md) gives

$$
\mathbb E[Y\mid X=x]=\int_0^\infty yxe^{-xy}\,dy=\frac1x,
$$

using either [integration by parts](../../../../../../integration-by-parts.md) or the [expected value](../../../../../../expected-value.md) of an [exponential distribution](../../../../../../exponential-distribution.md). Hence

$$
\boxed{\mathbb E[Y\mid X]=\frac1X\quad\text{almost surely}.}
$$

This is a finite value for almost every realization of $X$, but not an integrable [random variable](../../../../../../random-variable-split.md): $\mathbb E[1/X]=\int_0^\infty e^{-x}/x\,dx=\infty$. Since $Y\geq0$, its [conditional expectation](../../../../../../conditional-expectation.md) remains well-defined in the nonnegative, extended-expectation sense; the [tower property of conditional expectation](../../../../../../law-of-total-expectation.md) then gives $\mathbb EY=\infty$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4F](../../4f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
