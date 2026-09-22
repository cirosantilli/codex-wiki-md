# Chernoff affinity

↑ **Parent:** [Chernoff information](chernoff-information.md)

For [probability mass functions](probability-mass-function.md) $P,Q$, their [Chernoff affinity](chernoff-affinity.md) at $0<s<1$ is the [sum](sum.md) $Z(s)=\sum_xP(x)^sQ(x)^{1-s}$. It weights pointwise agreement between the two laws. The [weighted arithmetic-geometric mean inequality](weighted-arithmetic-geometric-mean-inequality.md) gives $P(x)^sQ(x)^{1-s}\leq sP(x)+(1-s)Q(x)$, hence $Z(s)\leq1$. With positive common support, $Z(0)=Z(1)=1$. Smaller affinity means a stronger separation at that weighting.

At $s=1/2$, $Z(1/2)=\sum_x\sqrt{P(x)Q(x)}$ is the [Bhattacharyya coefficient](bhattacharyya-coefficient.md). The quantity $-\ln Z(1/2)$ is the [Bhattacharyya distance](bhattacharyya-distance.md). Allowing all weights $s$ gives [Chernoff information](chernoff-information.md) at least this large. Symmetry under exchanging $P,Q$ sends $s$ to $1-s$, so [Chernoff information](chernoff-information.md) is symmetric even though an optimizing weight need not be $1/2$.

## ↑ Ancestors (7)

1. [Chernoff information](chernoff-information.md)
2. [Binary hypothesis testing in information theory](binary-hypothesis-testing-in-information-theory.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Chernoff affinity](chernoff-affinity.md)
- [Chernoff information for complementary Bernoulli distributions](chernoff-information-for-complementary-bernoulli-distributions.md)
