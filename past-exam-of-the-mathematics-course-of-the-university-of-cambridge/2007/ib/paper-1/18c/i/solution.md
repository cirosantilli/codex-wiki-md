<h1 id="18c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $K=\sum_iX_i$ and $\bar X=K/n$. The [likelihood](../../../../../../likelihood-function.md) is $\theta^K(1-\theta)^{n-K}$, so for $0<K<n$ its unique maximizer is $\widehat\theta=K/n$. By invariance of [maximum likelihood estimation](../../../../../../maximum-likelihood-estimation.md),

$$
\boxed{\widehat\phi=\widehat\theta(1-\widehat\theta)=\frac{K(n-K)}{n^2}.}
$$

For $K=0$ or $n$, the strict parameter interval $(0,1)$ has no attained [likelihood](../../../../../../likelihood-function.md) maximum; the usual extended estimate takes the limiting endpoint and gives $\widehat\phi=0$. Thus the displayed estimator is the conventional extended MLE on those samples, an important boundary qualification. This is the first estimator in [estimating Bernoulli variance](../../../../../../estimating-bernoulli-variance.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [18C](../../18c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
