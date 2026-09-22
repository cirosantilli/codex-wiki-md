<h1 id="12f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $B$ mean that the selected coin is biased and $F$ that it is fair. Both have prior [probability](../../../../../../probability.md) $1/2$. Conditional on either coin, tosses are independent. For the observed head count, the two [binomial distribution](../../../../../../binomial-distribution.md) [likelihoods](../../../../../../likelihood-function.md) are $\binom nk p^k(1-p)^{n-k}$ and $\binom nk2^{-n}$. [Bayes' theorem](../../../../../../bayes-theorem.md) cancels the common coefficient and equal prior weights, giving

$$
\boxed{\mathbb P(B\mid k\text{ heads in }n\text{ tosses})
=\frac{p^k(1-p)^{n-k}}{p^k(1-p)^{n-k}+2^{-n}}}.
$$

This applies for $0\leq k\leq n$, including endpoint coin biases with zero-power factors interpreted by the corresponding [likelihood](../../../../../../likelihood-function.md). The fair-coin [likelihood](../../../../../../likelihood-function.md) is positive, so the denominator cannot vanish.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [12F](../../12f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
