<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let independent [Bernoulli random variables](../../../../../../bernoulli-distribution.md) $Y_n$ have success probabilities $2^{-n}$, for $n\geq1$, and use their [natural filtration](../../../../../../natural-filtration.md). Define

$$
\boxed{X_0=0,\qquad X_n=\sum_{k=1}^n(1-2^kY_k).}
$$

Each increment is integrable, finite, and independent of the previous [filtration](../../../../../../filtration-probability-theory.md), with [expectation](../../../../../../expected-value.md)

$$
\mathbb E(1-2^nY_n)=1-2^n2^{-n}=0.
$$

Thus $X$ is a [martingale](../../../../../../martingale-split.md). The increments have no common finite bound, since a success produces a jump of size $2^n-1$.

Since $\sum_n\mathbb P(Y_n=1)<\infty$, the [First Borel-Cantelli lemma](../../../../../../borel-cantelli-first-lemma.md) says that only finitely many successes occur [almost surely](../../../../../../almost-sure-convergence.md). Consequently

$$
X_n=n-\sum_{k\geq1}2^kY_k
$$

for all sufficiently large $n$, with the random sum finite [almost surely](../../../../../../almost-sure-convergence.md). Therefore **$X_n\to+\infty$ [almost surely](../../../../../../almost-sure-convergence.md)**, so neither finite convergence nor two-sided oscillation occurs. This [rare-jump martingale divergence](../../../../../../rare-jump-martingale-divergence.md) example gives probability zero, rather than one, for the union in (i).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
