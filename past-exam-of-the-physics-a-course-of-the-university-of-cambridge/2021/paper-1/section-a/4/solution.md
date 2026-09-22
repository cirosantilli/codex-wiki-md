<h1 id="section-a/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Assume independent background events at a known constant rate, so the background count follows a [Poisson distribution](../../../../../poisson-distribution.md). In five months its mean is $\mu_b=0.3\times5=1.5$. The [null hypothesis](../../../../../null-hypothesis.md) of background alone assigns the observed upward fluctuation the [P-value](../../../../../p-value.md)

$$
p=P(N\geq8\mid\mu_b=1.5)
=1-e^{-1.5}\sum_{n=0}^{7}\frac{1.5^n}{n!}
\simeq1.696\times10^{-4}.
$$

Thus

$$
\boxed{p\simeq1.7\times10^{-4}>10^{-6}:\quad\text{the discovery criterion is not met}.}
$$

The tail includes counts above eight because they would be at least as discrepant with the background-only prediction. Even the probability of exactly eight, $e^{-1.5}1.5^8/8!\simeq1.42\times10^{-4}$, exceeds the specified threshold, though it is not the appropriate tail test. The [Poisson tail discovery probability](../../../../../poisson-tail-discovery-probability.md) is a probability of data under a background model; it is not a posterior probability that the background model is true. This interprets the question's discovery rule in its usual [statistical significance](../../../../../statistical-significance.md) sense.

## ↑ Ancestors (14)

1. [4](../4.md)
2. [Section A](../../section-a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2021](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
