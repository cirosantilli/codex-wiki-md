<h1 id="28k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [risk function](../../../../../../risk-function.md) of an estimator $\widehat\theta$ under the stated [quadratic loss](../../../../../../squared-error-loss.md) is

$$
R(\theta,\widehat\theta)
=\mathbb E_\theta
\lVert\widehat\theta(X)-\theta\rVert_2^2.
$$

The [multivariate normal density](../../../../../../multivariate-normal-density.md) is proportional, as a function of $\theta$, to

$$
\exp\left(-\frac12\lVert X-\theta\rVert^2\right),
$$

so [maximum likelihood estimation](../../../../../../maximum-likelihood-estimation.md) gives $\widehat\theta_{\rm MLE}=X$. Writing $X=\theta+Z$ with $Z\sim N_p(0,I_p)$,

$$
\boxed{R(\theta,\widehat\theta_{\rm MLE})
=\mathbb E\lVert Z\rVert^2=p}
$$

for every $\theta\in\mathbb R^p$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [28K](../../28k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
