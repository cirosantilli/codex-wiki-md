<h1 id="14/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Under [independence](../../../../../../independent-random-variables.md), there are two disjoint ways to score two goals in total. One game can contain both, with [probability](../../../../../../probability.md)

$$
10\left(e^{-\lambda}\frac{\lambda^2}{2}\right)(e^{-\lambda})^9
=5\lambda^2e^{-10\lambda}.
$$

Alternatively, two different games can contain one goal each, with [probability](../../../../../../probability.md)

$$
\binom{10}{2}(\lambda e^{-\lambda})^2(e^{-\lambda})^8
=45\lambda^2e^{-10\lambda}.
$$

Adding gives

$$
\boxed{P(\text{two goals in the season})=50\lambda^2e^{-10\lambda}}.
$$

This also follows from the [Sum of independent Poisson random variables](../../../../../../addition-of-independent-poisson-random-variables.md): the season total is Poisson with parameter $10\lambda$, whose [probability](../../../../../../probability.md) at two is $e^{-10\lambda}(10\lambda)^2/2!$.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [14](../../../14.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
