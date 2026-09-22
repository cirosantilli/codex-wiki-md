<h1 id="7h/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

By the [bias-variance decomposition of mean squared error](../../../../../../bias-variance-decomposition-of-mean-squared-error.md),

$$
\operatorname{MSE}(k\bar X)=\theta^2\left[(k-1)^2+\frac{k^2}{n}\right].
$$

For $\theta\ne0$, comparison with the unbiased estimator reduces to

$$
(n+1)k^2-2nk+n-1<0.
$$

Its roots are $(n-1)/(n+1)$ and $1$, so

$$
\boxed{\frac{n-1}{n+1}<k<1.}
$$

Equality at either endpoint gives the same risk as $\bar X$. At $\theta=0$, every risk is zero, so no strict improvement is possible. This illustrates [shrinking a sample mean with variance proportional to mean squared](../../../../../../shrinking-a-sample-mean-with-variance-proportional-to-mean-squared.md): allowing a small [bias](../../../../../../bias-of-an-estimator.md) can reduce [variance](../../../../../../variance-split.md) enough to improve total risk. The best constant is $k=n/(n+1)$, whose [mean squared error](../../../../../../mean-squared-error.md) is $\theta^2/(n+1)$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [7H](../../7h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
