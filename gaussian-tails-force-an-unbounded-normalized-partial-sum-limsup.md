# Gaussian tails force an unbounded normalized partial-sum limsup

↑ **Parent:** [Central limit theorem](central-limit-theorem.md)

For independent identically distributed mean-zero variables with finite positive variance, the [central limit theorem](central-limit-theorem.md) gives a positive eventual lower bound for $\mathbb P(S_n/\sqrt n\geq K)$ for every finite $K$. The decreasing events $\bigcup_{n\geq m}\{S_n/\sqrt n\geq K\}$ have probabilities bounded below, so [continuity from above of a measure](continuity-from-above-of-a-measure.md) gives positive probability that the limsup is at least $K$. The limsup itself is unchanged by removing any finite initial sum, hence is tail measurable. [Kolmogorov zero-one law](kolmogorov-s-zero-one-law.md) makes each event “limsup at least $K$” certain; intersect over integer $K$. The result is false for zero variance. One should apply the zero-one law to the limsup, rather than assume the exact threshold infinitely-often event is unaffected by a vanishing change.

## ↑ Ancestors (7)

1. [Central limit theorem](central-limit-theorem.md)
2. [Convergence of random variables](convergence-of-random-variables-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
