# Expected relative entropy decomposition

↑ **Parent:** [Kullback-Leibler divergence](kullback-leibler-divergence.md)

Let $Q$ be a random [probability mass function](probability-mass-function.md) on a [finite alphabet](finite-alphabet.md), let $p=\mathbb E Q$, and suppose a fixed reference $r$ is positive on the [probability support](support-of-a-probability-distribution.md) of $p$. Then $Q$ vanishes [almost surely](almost-sure-convergence.md) wherever $p=0$, and

$$
D(Q\|r)-D(Q\|p)=\sum_{i:p_i>0}Q_i\log_2\frac{p_i}{r_i}.
$$

Taking [expected values](expected-value-split.md) yields the displayed decomposition. In particular it applies to an unbiased [empirical distribution](type-information-theory.md). It separates sampling fluctuation from reference mismatch: even perfect recovery of $p$ leaves the deterministic [relative entropy](kullback-leibler-divergence.md) $D(p\|r)$. A bound comparing different references must account for this term.

## ↑ Ancestors (6)

1. [Kullback-Leibler divergence](kullback-leibler-divergence.md)
2. [f-divergence](f-divergence-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-information-theory-course-of-the-university-of-oxford/2021/1/b/iii/solution.md)
