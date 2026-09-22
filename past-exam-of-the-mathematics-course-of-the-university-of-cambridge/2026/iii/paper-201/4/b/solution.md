<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The variable $Z=\int_0^1B_t\,dt$ is the $L^2$ limit of [Riemann sums](../../../../../../riemann-sum.md) of the [Gaussian process](../../../../../../gaussian-process.md) $B$, so it is a [Gaussian random variable](../../../../../../normal-distribution.md). Its mean is zero, and [Fubini's theorem](../../../../../../fubini-s-theorem.md) with $\mathbb E[B_sB_t]=\min(s,t)$ gives

$$
\operatorname{Var}(Z)
=\int_0^1\!\int_0^1\min(s,t)\,ds\,dt
=2\int_0^1\!\int_0^t s\,ds\,dt
=\frac13.
$$

**Therefore $Z\sim N(0,1/3)$.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
