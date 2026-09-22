<h1 id="20h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $S=\sum_iX_i$. The [likelihood function](../../../../../../likelihood-function.md) for the [Poisson distribution](../../../../../../poisson-distribution.md) is proportional to $e^{-n\theta}\theta^S$. For $S>0$, differentiation of the [log-likelihood](../../../../../../log-likelihood.md) gives $-n+S/\theta=0$, and its second derivative is negative. For $S=0$, the likelihood decreases with $\theta$ and has its maximum at the boundary zero. Hence

$$
\boxed{\widehat\theta=\overline X=\frac Sn.}
$$

The estimator is **unbiased**, since $\mathbb E\widehat\theta=n^{-1}\sum_i\mathbb EX_i=\theta$. Its variance is $\theta/n$. If the parameter space excludes zero, an all-zero sample gives a supremum as $\theta\downarrow0$ rather than an attained maximum.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [20H](../../20h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
