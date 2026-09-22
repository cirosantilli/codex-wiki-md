<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For every zero-starting [continuous local martingale](../../../../../../continuous-local-martingale.md) $M$, there is a unique, up to indistinguishability, continuous adapted increasing process $[M]$, with $[M]_0=0$, such that

$$
\boxed{M_t^2-[M]_t\text{ is a local martingale}.}
$$

This is its [quadratic variation](../../../../../../quadratic-variation.md). It also satisfies, for deterministic partitions whose mesh tends to zero,

$$
[M]_t=\lim\sum_j\big(M_{t_{j+1}\wedge t}-M_{t_j\wedge t}\big)^2,
$$

with convergence uniformly on compact time intervals in probability. The theorem includes existence and finiteness on each compact interval; monotonicity is understood pathwise outside one null set.

Uniqueness follows because the difference of two candidate increasing continuous processes is both a [finite-variation process](../../../../../../finite-variation-process.md) and a [continuous local martingale](../../../../../../continuous-local-martingale.md), hence is identically zero from its zero initial value. For a [continuous semimartingale](../../../../../../continuous-semimartingale.md) $X=X_0+M+A$, its [quadratic variation](../../../../../../quadratic-variation.md) is $[X]=[M]$, since continuous finite-variation terms have zero [quadratic variation](../../../../../../quadratic-variation.md). Polarization defines the [quadratic covariation](../../../../../../quadratic-covariation.md) by $[M,N]=([M+N]-[M-N])/4$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
