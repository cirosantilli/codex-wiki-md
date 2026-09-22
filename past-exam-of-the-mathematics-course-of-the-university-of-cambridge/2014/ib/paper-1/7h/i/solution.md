<h1 id="7h/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For an [estimator](../../../../../../estimator.md) with finite second moment, its [bias](../../../../../../bias-of-an-estimator.md) and [mean squared error](../../../../../../mean-squared-error.md) are

$$
b_\theta=\mathbb E_\theta\widehat\theta-\theta,\qquad R_\theta=\mathbb E_\theta[(\widehat\theta-\theta)^2].
$$

Write $\widehat\theta-\theta=(\widehat\theta-\mathbb E_\theta\widehat\theta)+b_\theta$. On squaring and taking expectations, the cross term vanishes. This proves the [bias-variance decomposition of mean squared error](../../../../../../bias-variance-decomposition-of-mean-squared-error.md):

$$
\boxed{R_\theta=\operatorname{Var}_\theta(\widehat\theta)+b_\theta^2.}
$$

For the [sample mean](../../../../../../sample-mean.md), independence gives $\mathbb E\bar X=\theta$, $\operatorname{Var}(\bar X)=\theta^2/n$. Thus $k\bar X$ has bias $(k-1)\theta$. Unbiasedness throughout the parameter family requires

$$
\boxed{k=1,\qquad \operatorname{MSE}(\bar X)=\theta^2/n.}
$$

At the single parameter value $\theta=0$, all these estimators are zero almost surely; that special value does not change the requirement of unbiasedness for all $\theta$.

## ↑ Ancestors (11)

1. [I](../i.md)
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
