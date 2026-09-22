# Empirical cross-entropy

↑ **Parent:** [Cross-entropy](cross-entropy.md)

For observations $X_1,\ldots,X_n$ of a [categorical variable](categorical-variable.md), [empirical cross-entropy](empirical-cross-entropy.md) is the average [logarithmic loss](logarithmic-loss.md) under the reported [probability mass function](probability-mass-function.md) $q$. Writing the [empirical distribution](type-information-theory.md) as $\hat p_i=n^{-1}\#\{t:X_t=i\}$ gives

$$
\widehat H_n(Q)=-\frac1n\sum_{t=1}^n\log_2q(X_t)
=-\sum_{i:\hat p_i>0}\hat p_i\log_2q_i=H(\widehat P_n,Q).
$$

Under [independent and identically distributed](independent-and-identically-distributed-random-variables.md) observations from $P$ and a fixed model with positive [probability](probability.md) for each possible outcome, the [law of large numbers](law-of-large-numbers.md) gives convergence to $H(P,Q)$. A finite [empirical distribution](type-information-theory.md) is an estimate of $P$, rather than the true source law; unobserved outcomes need not be impossible. If the same data are used to choose $Q$, evaluating the resulting [empirical cross-entropy](empirical-cross-entropy.md) on that data need not estimate its prediction performance on fresh observations without [bias](bias-of-an-estimator.md).

**Table of contents**

- [Cross-entropy and maximum likelihood](cross-entropy-and-maximum-likelihood.md)

## ↑ Ancestors (7)

1. [Cross-entropy](cross-entropy.md)
2. [Information entropy](information-entropy.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Cross-entropy and maximum likelihood](cross-entropy-and-maximum-likelihood.md)
- [Empirical cross-entropy](empirical-cross-entropy.md)
