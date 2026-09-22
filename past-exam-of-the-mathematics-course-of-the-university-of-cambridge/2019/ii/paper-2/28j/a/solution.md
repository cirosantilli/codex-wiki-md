<h1 id="28j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $X_1\sim\operatorname{Poisson}(\theta)$, its [probability generating function](../../../../../../probability-generating-function.md) is

$$
G(s)=\exp(\theta(s-1)).
$$

Thus $\mathbb E[X_1]=G'(1)=\theta$ and

$$
\operatorname{Var}(X_1)=G''(1)+G'(1)-G'(1)^2=\theta.
$$

The [log-likelihood](../../../../../../log-likelihood.md) is, up to an additive constant,

$$
\ell(\theta)=-n\theta+\left(\sum_{i=1}^nX_i\right)\log\theta,
$$

so the [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md) is $\widehat\theta_{\rm MLE}=\overline X$. The [central limit theorem](../../../../../../central-limit-theorem.md) gives

$$
\boxed{\sqrt n(\widehat\theta_{\rm MLE}-\theta)
\xrightarrow{d}N(0,\theta).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [28J](../../28j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
