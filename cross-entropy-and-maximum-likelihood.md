# Cross-entropy and maximum likelihood

↑ **Parent:** [Empirical cross-entropy](empirical-cross-entropy.md)

For a [parametric statistical model](parametric-statistical-model.md) with [probability mass function](probability-mass-function.md) $q_\theta$ and an [independent and identically distributed](independent-and-identically-distributed-random-variables.md) model, minimizing [empirical cross-entropy](empirical-cross-entropy.md) is [maximum likelihood estimation](maximum-likelihood-estimation-split.md). The [logarithm](logarithm.md) is strictly increasing, so maximizing $\prod_tq_\theta(X_t)$ is equivalent to maximizing $\sum_t\log_2q_\theta(X_t)$. Negating and dividing by $n$ gives the displayed minimization. Restricting the model family can prevent the optimum from matching the [empirical distribution](type-information-theory.md), and a finite optimizing parameter need not exist. This algebra does not by itself establish accuracy on new data.[§1, printed p. 360: optimum-score estimation and maximum likelihood](strictly-proper-scoring-rules-prediction-and-estimation-by-tilmann-gneiting-and-others.md)

## ↑ Ancestors (8)

1. [Empirical cross-entropy](empirical-cross-entropy.md)
2. [Cross-entropy](cross-entropy.md)
3. [Information entropy](information-entropy-split.md)
4. [Information theory](information-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
