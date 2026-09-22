<h1 id="o/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Minimize $\|Y-X\theta\|^2$. Differentiation gives the [normal equations](../../../../normal-equation.md) $X^TX\widehat\theta=X^TY$. Full column rank makes $X^TX$ positive definite, so

$$
\boxed{\widehat\theta=(X^TX)^{-1}X^TY,\quad
\mathbb E\widehat\theta=\theta,\quad
\operatorname{Cov}(\widehat\theta)=\sigma^2(X^TX)^{-1}.}
$$

The expectation uses the zero error mean; the [covariance](../../../../covariance.md) uses $\operatorname{Cov}(\epsilon)=\sigma^2I$. With independent [Gaussian](../../../../normal-distribution.md) errors of common [variance](../../../../variance-split.md), maximizing likelihood minimizes exactly the same residual sum of squares, so this is also the maximum likelihood estimator, whether the common [variance](../../../../variance-split.md) is known or estimated.

For the quadratic design, decompose each group's residual sum of squares into its within-group constant plus the group size times the squared residual of its [sample mean](../../../../sample-mean.md). The three parameter combinations $\alpha$, $\alpha+\beta+\gamma$ and $\alpha-\beta+\gamma$ can fit all three group means exactly. Therefore

$$
\widehat\alpha=\overline Y_0,\qquad
\boxed{\widehat\beta=\frac{\overline Y_1-\overline Y_{-1}}2,\qquad
\widehat\gamma=\frac{\overline Y_1+\overline Y_{-1}-2\overline Y_0}2.}
$$

The group means are independent normal variables, with variances $\sigma^2/m,\sigma^2/n,\sigma^2/n$. Hence their two stated linear combinations are jointly normal, and

$$
\operatorname{Cov}(\widehat\beta,\widehat\gamma)
=\tfrac14(\sigma^2/n-\sigma^2/n)=0.
$$

Joint normality therefore proves **the two estimators are independent**. Their variances are $\sigma^2/(2n)$ and $\sigma^2/(2n)+\sigma^2/m$, respectively. Equal replication at the two off-center temperatures is what cancels the [covariance](../../../../covariance.md).

## ↑ Ancestors (12)

1. [4](../4.md)
2. [O](../../o.md)
3. [2006](../../../2006-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
