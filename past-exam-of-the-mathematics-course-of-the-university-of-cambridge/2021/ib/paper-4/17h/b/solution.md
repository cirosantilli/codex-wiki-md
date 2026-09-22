<h1 id="17h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The estimator is unbiased because $\mathbb E_\theta X=n\theta$, and

$$
\operatorname{Var}_\theta(\widehat\theta)
=\frac1{n^2}\operatorname{Var}_\theta(X)
=\frac{\theta(1-\theta)}n.
$$

The [bias-variance decomposition of mean squared error](../../../../../../bias-variance-decomposition-of-mean-squared-error.md) therefore gives

$$
\boxed{f(\theta)
=\mathbb E_\theta[(\widehat\theta-\theta)^2]
=\frac{\theta(1-\theta)}n}.
$$

The quadratic $\theta(1-\theta)$ is maximized at $\theta=1/2$, so

$$
\boxed{\sup_{0<\theta<1}f(\theta)=\frac1{4n}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [17H](../../17h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
