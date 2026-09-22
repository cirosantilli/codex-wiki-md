<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Under $H_0$, the [Hilbert-space central limit theorem](../../../../../../hilbert-space-central-limit-theorem.md) gives

$$
\sqrt n(\widehat\mu-\mu_0)\xrightarrow dG,
$$

where $G$ is a centered [Gaussian random element](../../../../../../gaussian-random-element.md) with covariance $C_X$. Distinct leading eigenvalues imply consistency of the empirical eigenvalues and eigenfunctions, up to irrelevant signs. The first $K$ standardized [functional principal component scores](../../../../../../functional-principal-component-score.md) of $G$ are independent $N(0,1)$ variables, so [Slutsky theorem](../../../../../../slutsky-theorem.md) yields

$$
T_{PC}\xrightarrow d\chi_K^2.
$$

An asymptotic level-$\alpha$ test rejects above the $(1-\alpha)$ quantile of the [chi-squared distribution](../../../../../../chi-squared-distribution.md).

Under a fixed alternative, put $\delta=\mu-\mu_0$. The [weak law of large numbers](../../../../../../weak-law-of-large-numbers.md) and eigenpair consistency give

$$
\frac{T_{PC}}n\xrightarrow p
\sum_{k=1}^K\frac{\langle\delta,\phi_k\rangle^2}{\lambda_k}.
$$

**Thus the statistic diverges and the test is consistent whenever at least one retained projection is nonzero. A fixed alternative orthogonal to the first $K$ eigenfunctions is invisible to this fixed-$K$ statistic.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 225](../../../paper-225-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
