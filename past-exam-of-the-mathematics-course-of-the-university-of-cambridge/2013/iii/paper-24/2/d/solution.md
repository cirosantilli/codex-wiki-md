<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Take two independent rate-one [Poisson processes](../../../../../../poisson-process.md) $N^+$ and $N^-$, and let

$$
X_t=N_t^+-N_t^-.
$$

The [difference of independent Poisson processes](../../../../../../difference-of-independent-poisson-processes.md) starts at zero and has [stationary increments](../../../../../../stationary-increments.md) and [independent increments](../../../../../../independent-increments.md). Its paths are [càdlàg](../../../../../../cadlag.md). For an interval of length $h$, the probability of any jump is $1-e^{-2h}\to0$, proving [stochastic continuity](../../../../../../stochastic-continuity.md). Thus $X$ is a [Lévy process](../../../../../../levy-process.md). The [characteristic function](../../../../../../characteristic-function.md) of a [Poisson distribution](../../../../../../poisson-distribution.md) with mean $t$ is $\exp(t(e^{iu}-1))$, so [independence](../../../../../../independent-random-variables.md) gives

$$
\boxed{\mathbb E e^{iuX_t}
=\exp\bigl(t(e^{iu}-1)+t(e^{-iu}-1)\bigr)
=e^{2t(\cos u-1)}.}
$$

The [sample paths](../../../../../../sample-path.md) are integer-valued step functions with jumps $+1$ or $-1$. On every bounded interval there are only finitely many jumps, and independent Poisson arrival times coincide with probability zero. The combined arrival rate is two: holding times are independent exponentials of rate two, and each jump direction has probability $1/2$, independently of the holding times. This is equivalently a [Compound Poisson process](../../../../../../compound-poisson-process.md) of rate two with [Rademacher distribution](../../../../../../rademacher-distribution.md) jump sizes. Its paths have [finite variation](../../../../../../total-variation-of-a-function.md) on compact time intervals, although there are infinitely many jumps over the whole half-line [almost surely](../../../../../../almost-sure-convergence.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
