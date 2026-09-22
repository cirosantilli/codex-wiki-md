# Multinomial aggregation

↑ **Parent:** [Multinomial distribution](multinomial-distribution.md)

If $(N_1,\ldots,N_k)$ has a [multinomial distribution](multinomial-distribution.md) with $n$ trials, group its categories into disjoint nonempty [sets](set-split.md) $G_1,\ldots,G_m$ covering all categories. The grouped counts in the displayed equation have the [multinomial distribution](multinomial-distribution.md)

$$
(M_1,\ldots,M_m)\sim\operatorname{Mult}(n;q_1,\ldots,q_m).
$$

Each original trial belongs to exactly one group, its group [probability](probability.md) is the sum of its category [probabilities](probability.md), and grouping preserves [independence](independent-random-variables.md) between trials. This gives the rule without summing the original [probability mass function](probability-mass-function.md) over every possible internal count pattern.

For the four-trial example with [probabilities](probability.md) $(1/2,3/10,1/5)$, merge the last two categories. Their total $M=N_2+N_3$ has the [binomial distribution](binomial-distribution.md) $\operatorname{Bin}(4,1/2)$, so $\mathbb E M=2$ and $\operatorname{Var}(M)=1$. The same [variance](variance-split.md) follows from the [variance of a sum](variance-of-a-sum.md):

$$
\operatorname{Var}(N_2+N_3)=0.84+0.64+2(-0.24)=1.
$$

Ignoring the negative [covariance](covariance.md) would give $1.48$, although the two counts share a fixed total. [Multinomial aggregation](multinomial-aggregation.md) lets the resolution of category labels change while retaining a consistent model for the counts.

## ↑ Ancestors (8)

1. [Multinomial distribution](multinomial-distribution.md)
2. [Discrete probability distribution](discrete-probability-distribution-split.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Multinomial aggregation](multinomial-aggregation.md)
- [Multinomial distribution](multinomial-distribution.md)
