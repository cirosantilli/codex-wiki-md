<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Using the [probability density function](../../../../../probability-density-function.md) of the [Erlang distribution](../../../../../erlang-distribution.md), the [expected value](../../../../../expected-value-split.md) is

$$
\mathbb E X=\theta^2\int_0^\infty x^2e^{-\theta x}\,dx
=\frac1\theta\int_0^\infty u^2e^{-u}\,du
=\boxed{\frac2\theta}.
$$

Here $u=\theta x$, and two applications of [integration by parts](../../../../../integration-by-parts.md) give $\int_0^\infty u^2e^{-u}\,du=2\int_0^\infty ue^{-u}\,du=2$. The boundary terms vanish because [exponential decay](../../../../../exponential-decay.md) dominates these powers.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
