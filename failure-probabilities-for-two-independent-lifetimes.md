# Failure probabilities for two independent lifetimes

↑ **Parent:** [Order statistic](order-statistic.md)

For independent [survival times](survival-time.md) $T_1,T_2$ with [cumulative distribution functions](cumulative-distribution-function.md) $F_1,F_2$, the probability both components have failed by time $t$ is

$$
P(\max(T_1,T_2)\leq t)=F_1(t)F_2(t).
$$

The probability at least one has failed is

$$
P(\min(T_1,T_2)\leq t)=1-(1-F_1(t))(1-F_2(t)).
$$

The first equality uses [independence of random variables](independent-random-variables.md); the second applies it to the complementary event that both survive. These are the distributions of the two extreme [order statistics](order-statistic.md).

Marginal distributions alone do not determine these probabilities. Without independence, the [Fréchet inequalities](frechet-inequalities.md) give $\max(0,F_1+F_2-1)\leq P(\text{both})\leq\min(F_1,F_2)$, and [inclusion-exclusion](inclusion-exclusion-principle.md) gives $P(\text{at least one})=F_1+F_2-P(\text{both})$.

## ↑ Ancestors (6)

1. [Order statistic](order-statistic.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-2/14/e/solution.md)
