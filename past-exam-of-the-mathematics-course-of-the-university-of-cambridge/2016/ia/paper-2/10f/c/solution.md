<h1 id="10f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

There are more bins than balls, so the [pigeonhole principle](../../../../../../pigeonhole-principle.md) forces at least one empty bin. In fact $E\geq m-n=(a-1)n$. Consequently

$$
\boxed{\mathbb P(E=0)=0.}
$$

For the expected fraction, substitute $m=an$ into part (b). The elementary exponential limit, obtained by taking logarithms, gives

$$
\boxed{\frac{\mathbb E[E]}m=\left(1-\frac1{an}\right)^n\longrightarrow e^{-1/a}.}
$$

This is the empty-bin case of the [Poisson limit for occupancy fractions](../../../../../../poisson-limit-for-occupancy-fractions.md), with limiting mean occupancy $1/a$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [10F](../../10f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
