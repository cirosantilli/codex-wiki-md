<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Each observation has [normal distribution](../../../../../normal-distribution.md) [probability density function](../../../../../probability-density-function.md)

$$
f(x_i\mid\mu)=\frac1{\sqrt{2\pi}}\exp\!\left[-\frac12(x_i-\mu)^2\right].
$$

The observations are [independent and identically distributed](../../../../../independent-and-identically-distributed-random-variables.md), so their joint [probability density function](../../../../../probability-density-function.md), viewed as a function of the unknown mean, is the product:

$$
\boxed{L(\mu)=\prod_{i=1}^nf(x_i\mid\mu)
=(2\pi)^{-n/2}\exp\!\left[-\frac12\sum_{i=1}^n(x_i-\mu)^2\right]}.
$$

Independence justifies multiplication; the common mean and known unit [variance](../../../../../variance-split.md) justify using this same density factor for every observation.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 3](../../../paper-3-split.md)
4. [2024](../../../split.md)
5. [Past exam of the systems biology course of the University of Cambridge](../../../../split.md)
6. [Systems Biology course of the University of Cambridge](../../../../../systems-biology-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
