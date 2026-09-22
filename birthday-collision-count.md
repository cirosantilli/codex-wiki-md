# Birthday collision count

↑ **Parent:** [Birthday problem](birthday-problem.md)

The [birthday collision count](birthday-collision-count.md) counts equal-label [unordered pairs](unordered-pair.md). Write it as a [sum](sum.md) of [indicator random variables](indicator-random-variable.md):

$$
C=\sum_{1\leq i<j\leq n}\mathbf1_{\{X_i=X_j\}},\qquad\mathbb E[C]=\sum_{i<j}\frac1m=\frac{n(n-1)}{2m}.
$$

This uses [linearity of expectation](linearity-of-expectation.md); mutual [independence](independent-random-variables.md) of the pair indicators is unnecessary. For 23 uniform calendar labels, $\mathbb E[C]=253/365\approx0.69315$, whereas $\mathbb P(C\geq1)\approx0.50730$. A configuration with three equal labels contributes three pairs, so counting pairs and recording whether any pair exists are different [random variables](random-variable-split.md).

Treating every pair event as mutually independent would give the wrong exact formula. For three draws, $X_1=X_2$ and $X_1=X_3$ force $X_2=X_3$. The probability that all three equalities hold is $1/m^2$, while the product of their individual probabilities is $1/m^3$ for $m>1$. This distinguishes [independence](independent-random-variables.md) of the original label draws from mutual [independence](independent-random-variables.md) of events built from overlapping draws.

## ↑ Ancestors (5)

1. [Birthday problem](birthday-problem.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Birthday collision count](birthday-collision-count.md)
