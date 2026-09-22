# Convergence in probability implies convergence in distribution

↑ **Parent:** [Convergence in probability](convergence-in-probability.md)

For real [random variables](random-variable-split.md) on one [probability space](probability-space-split.md), fix a [continuity](continuous-function.md) point $x$ of the [cumulative distribution function](cumulative-distribution-function.md) $F_X$. For every $\varepsilon>0$, inclusions of [events](event.md) give

$$
F_X(x-\varepsilon)-\mathbb P(|X_n-X|>\varepsilon)\leq F_{X_n}(x)\leq F_X(x+\varepsilon)+\mathbb P(|X_n-X|>\varepsilon).
$$

Take the lower and upper [limits](limit-of-a-function.md) as $n\to\infty$, using [convergence in probability](convergence-in-probability.md), and then let $\varepsilon\downarrow0$. [Continuity](continuous-function.md) at $x$ makes both bounds $F_X(x)$, proving [convergence in distribution](convergence-in-distribution.md). The two modes of convergence have different information: [convergence in probability](convergence-in-probability.md) concerns the coupling on one [probability space](probability-space-split.md), whereas [convergence in distribution](convergence-in-distribution.md) concerns only the marginal [probability distributions](probability-distribution-split.md).

## ↑ Ancestors (7)

1. [Convergence in probability](convergence-in-probability.md)
2. [Convergence of random variables](convergence-of-random-variables-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-probability-course-of-the-university-of-oxford/2014/1/a/iii/solution.md)
