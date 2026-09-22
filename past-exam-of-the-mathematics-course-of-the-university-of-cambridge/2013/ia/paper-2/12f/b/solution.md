<h1 id="12f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a finite stopping time $n$ with target $k\geq1$, necessarily $n\geq k$. The last toss must be a head and the preceding $n-1$ tosses must contain $k-1$ heads. The [negative binomial stopping argument](../../../../../../negative-binomial-stopping-argument.md) therefore gives [likelihood](../../../../../../likelihood-function.md) $\binom{n-1}{k-1}p^k(1-p)^{n-k}$ for the biased coin, and $\binom{n-1}{k-1}2^{-n}$ for the fair coin. Applying [Bayes' theorem](../../../../../../bayes-theorem.md) again yields

$$
\boxed{\mathbb P(B\mid\text{the }k\text{th head occurs at toss }n)
=\frac{p^k(1-p)^{n-k}}{p^k(1-p)^{n-k}+2^{-n}}}.
$$

The two experiments have different combinatorial coefficients, but each coefficient is independent of the coin parameter. Thus [posterior equality for proportional likelihoods](../../../../../../posterior-equality-for-proportional-likelihoods.md) explains their identical posterior formula. If $p=0$, a finite positive-head stopping observation has zero [likelihood](../../../../../../likelihood-function.md) under the biased coin, consistently giving posterior zero. If the target is $k=0$, the experiment stops at $n=0$ without a toss and the posterior remains $1/2$; a positive stopping time would then be impossible.

## ↑ Ancestors (11)

1. [B](../b.md)
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
