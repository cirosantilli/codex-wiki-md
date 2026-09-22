<h1 id="o/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $Q=\sum_iX_i^2$. For $\theta>0$, the [log-likelihood](../../../../../log-likelihood.md) is $\ell(\theta)=\text{constant}-(n/2)\log\theta-Q/(2\theta)$. Its derivative is $-n/(2\theta)+Q/(2\theta^2)$, changing from positive to negative at $Q/n$. Thus

$$
\boxed{\widehat\theta=\frac1n\sum_iX_i^2.}
$$

The known mean is zero, so no centring at the sample mean is needed. Taking the expected negative second derivative gives $I_n(\theta)=n/(2\theta^2)$. The large-sample variance is consequently $2\theta^2/n$. With $z_{1-\alpha/2}$ the indicated standard-normal [quantile](../../../../../quantile-function.md), a [Wald confidence interval](../../../../../wald-confidence-interval.md) is

$$
\boxed{\widehat\theta\ \pm\ z_{1-\alpha/2}\widehat\theta\sqrt{2/n}.}
$$

The interval may be restricted to the parameter space $\theta>0$. The parameter is the variance itself, so the standard error is proportional to $\widehat\theta$, not to its square root.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [O](../../../o.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
