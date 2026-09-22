<h1 id="16/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

The $i$th screen distance is $x_0/2^i$, starting at $i=1$. The previous [expected value](../../../../../expected-value-split.md) therefore scales to $E[Y_i]=x_0\ln3/(\pi2^i)$. To justify the infinite [linearity of expectation](../../../../../linearity-of-expectation.md), note that $|\tan\theta_i|\le\sqrt3$ throughout the restricted angular interval. Thus

$$
\sum_{i=1}^\infty|Y_i|\le\sqrt3x_0\sum_{i=1}^\infty2^{-i}=\sqrt3x_0.
$$

This deterministic integrable bound justifies the [expectation of an absolutely summable random series](../../../../../expectation-of-an-absolutely-summable-random-series.md), even without assuming independent firing angles. Summing the [geometric series](../../../../../geometric-series.md) gives

$$
\boxed{E\left[\sum_{i=1}^\infty Y_i\right]=\frac{x_0\ln3}{\pi}\sum_{i=1}^\infty2^{-i}=\frac{x_0\ln3}{\pi}.}
$$

## ↑ Ancestors (13)

1. [G](../g.md)
2. [16](../../16.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
