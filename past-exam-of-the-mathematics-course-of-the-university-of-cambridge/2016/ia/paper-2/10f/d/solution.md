<h1 id="10f/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

If $C=0$, every bin contains at most one ball, so the total number of balls is at most $m$. Since $n=dm>m$, the [pigeonhole principle](../../../../../../pigeonhole-principle.md) makes that event impossible:

$$
\boxed{\mathbb P(C=0)=0.}
$$

As $n\to\infty$ along these values, $m\to\infty$ and the mean occupancy $n/m$ is $d$. Apply part (b):

$$
\frac{\mathbb E[C]}m=1-\left(1-\frac1m\right)^{dm}-d\left(1-\frac1m\right)^{dm-1}.
$$

Both powers tend to $e^{-d}$. Hence

$$
\boxed{\frac{\mathbb E[C]}m\longrightarrow1-(1+d)e^{-d}.}
$$

The [Poisson limit for occupancy fractions](../../../../../../poisson-limit-for-occupancy-fractions.md) interprets the answer as the probability that a [Poisson distribution](../../../../../../poisson-distribution.md) variable with mean $d$ is at least two.

## ↑ Ancestors (11)

1. [D](../d.md)
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
