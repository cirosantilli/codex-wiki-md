# Monotonicity of expected empirical relative entropy

↑ **Parent:** [Type (information theory)](type-information-theory.md)

For [independent and identically distributed](independent-and-identically-distributed-random-variables.md) observations from a [probability mass function](probability-mass-function.md) $p$ on a [finite alphabet](finite-alphabet.md), expected [relative entropy](kullback-leibler-divergence.md) of the [empirical distribution](type-information-theory.md) from $p$ is nonincreasing in sample size. The [leave-one-out identity for empirical distributions](leave-one-out-identity-for-empirical-distributions.md) and [convexity of relative entropy in its first argument](convexity-of-relative-entropy-in-its-first-argument.md) give

$$
D(\widehat p_{n+1}\|p)\leq\frac1{n+1}\sum_{i=1}^{n+1}D(\widehat q_{n,i}\|p).
$$

Every deletion sample has the law of $n$ observations from $p$. Taking [expected values](expected-value-split.md) proves the assertion without requiring [independence](independent-random-variables.md) between deletion samples. Zero-probability symbols are absent [almost surely](almost-sure-convergence.md). Since $\mathbb E\widehat p_n=p$, the identity $\mathbb E D(\widehat p_n\|p)=H(p)-\mathbb E H(\widehat p_n)$ also shows that expected empirical [information entropy](information-entropy-split.md) increases towards the source [information entropy](information-entropy-split.md). Convergence follows from the [strong law of large numbers](strong-law-of-large-numbers.md) for empirical frequencies and boundedness and [continuity](continuous-function.md) of [information entropy](information-entropy-split.md) on a finite [probability simplex](probability-simplex.md).

## ↑ Ancestors (6)

1. [Type (information theory)](type-information-theory.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
