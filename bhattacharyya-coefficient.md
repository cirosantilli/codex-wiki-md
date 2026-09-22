# Bhattacharyya coefficient

↑ **Parent:** [Information theory](information-theory-split.md)

For [probability distributions](probability-distribution.md) $p,q$ on the same finite alphabet, the Bhattacharyya coefficient measures their square-root overlap:

$$
B(p,q)=\sum_i\sqrt{p_iq_i}.
$$

The vectors $(\sqrt{p_i})_i$ and $(\sqrt{q_i})_i$ have unit [Euclidean norm](euclidean-norm.md), so the [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) gives $0\leq B\leq1$. Equality $B=1$ holds exactly when the distributions agree; $B=0$ holds exactly when they assign positive [probability](probability.md) to disjoint outcomes. For $p=(0.9,0.1)$ and $q=(0.6,0.4)$, $B=\sqrt{0.54}+0.2\approx0.934847$. This overlap is not the probability that two independent draws agree, which here is $0.58$.

The [fidelity of commuting mixed states](fidelity-of-commuting-mixed-states.md) reduces to this coefficient. More generally, the [measurement characterization of quantum fidelity](measurement-characterization-of-quantum-fidelity.md) minimizes it over outcome distributions of a common [measurement in quantum mechanics](quantum-measurement-split.md), connecting classical overlap to the [unsquared quantum fidelity](fidelity-of-quantum-states.md).

**Table of contents**

- [Bhattacharyya distance](bhattacharyya-distance.md)

## ↑ Ancestors (5)

1. [Information theory](information-theory-split.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Bhattacharyya distance](bhattacharyya-distance.md)
- [Chernoff affinity](chernoff-affinity.md)
- [Measurement characterization of quantum fidelity](measurement-characterization-of-quantum-fidelity.md)
