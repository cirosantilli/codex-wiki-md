# Collision probability of two independent categorical draws

↑ **Parent:** [Birthday problem](birthday-problem.md)

Suppose two [independent random variables](independent-random-variables.md) have the same [categorical distribution](categorical-distribution.md), with label probabilities $p_1,\ldots,p_m$. The disjoint equal-label events give

$$
\mathbb P(X=Y)=\sum_{i=1}^m p_i^2.
$$

For the original chosen probabilities $(1/2,1/4,1/8,1/8)$, this is $11/32=0.34375$, rather than the uniform four-label value $1/4$. The [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) gives $1=(\sum_i p_i)^2\leq m\sum_i p_i^2$, so uniform probabilities minimize this two-draw collision probability. This pair formula alone does not supply the entire group collision probability for a nonuniform model.

## ↑ Ancestors (5)

1. [Birthday problem](birthday-problem.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)
