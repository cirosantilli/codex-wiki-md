# Mismatched asymptotic equipartition property

↑ **Parent:** [Cross-entropy](cross-entropy.md)

For [independent and identically distributed random variables](independent-and-identically-distributed-random-variables.md) with [probability mass function](probability-mass-function.md) $p$ on a [finite alphabet](finite-alphabet.md), evaluate their realized strings under a fixed product model $q_n(x^n)=\prod_iq(x_i)$. If $q$ is positive on the [probability support](support-of-a-probability-distribution.md) of $p$, the [strong law of large numbers](strong-law-of-large-numbers.md) gives

$$
\frac1n\log_2q_n(X^n)=\frac1n\sum_i\log_2q(X_i)\longrightarrow-H(p,q)=-H(p)-D_{\mathrm{KL}}(p\Vert q)
$$

[almost surely](almost-sure-convergence.md), using [cross-entropy equals entropy plus relative entropy](cross-entropy-equals-entropy-plus-relative-entropy.md). If $q$ vanishes at an outcome of positive $p$ [probability](probability.md), that outcome eventually appears [almost surely](almost-sure-convergence.md), making all subsequent product likelihoods zero and the limit $-\infty$. This matches infinite [cross-entropy](cross-entropy.md).

## ↑ Ancestors (7)

1. [Cross-entropy](cross-entropy.md)
2. [Information entropy](information-entropy-split.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-information-theory-course-of-the-university-of-oxford/2023/2/b/solution.md)
