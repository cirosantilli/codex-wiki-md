<h1 id="27k/solution">Solution</h1>

↑ **Parent:** [27K](../27k.md)

A random row vector has a [multivariate normal distribution](../../../../../multivariate-normal-distribution.md) when every real linear combination of its coordinates is normally distributed, allowing a zero-variance constant. Its law is determined by its mean and [covariance](../../../../../covariance.md). For the conditional and testing formulas assume $\Sigma$ is positive definite, so both coordinate [variances](../../../../../variance-split.md) and the conditional [variance](../../../../../variance-split.md) are positive; the given ratio already requires $\sigma_{XX}>0$.

Put $Z=Y-\beta X$, with $\beta=\sigma_{XY}/\sigma_{XX}$. The pair $(X,Z)$ is jointly normal and $\operatorname{Cov}(X,Z)=\sigma_{XY}-\beta\sigma_{XX}=0$, so $Z$ is independent of $X$. Its mean is $\mu_Y-\beta\mu_X$, and its [variance](../../../../../variance-split.md) is $\sigma_{YY}-\sigma_{XY}^2/\sigma_{XX}$. Hence

$$
\boxed{Y\mid X=x\sim N\left(\mu_Y+\beta(x-\mu_X),\ \sigma_{YY}-\frac{\sigma_{XY}^2}{\sigma_{XX}}\right).}
$$

Standardize each coordinate with its own positive [standard deviation](../../../../../standard-deviation.md). The standardized pairs have mean zero and [covariance](../../../../../covariance.md) $\begin{pmatrix}1&\rho\\\rho&1\end{pmatrix}$. Subtracting means and multiplying coordinates by positive constants leaves the sample correlation unchanged. Therefore **the distribution of $r$ depends only on $\rho$**.

For $n>2$, the stated statistic reduces algebraically to

$$
\boxed{t=\frac{r\sqrt{n-2}}{\sqrt{1-r^2}}.}
$$

This is strictly increasing from $(-1,1)$ onto $\mathbb R$, with derivative $\sqrt{n-2}(1-r^2)^{-3/2}$. Under $\rho=0$, change variables in the given Student density: $1+t^2/(n-2)=1/(1-r^2)$. Hence

$$
\boxed{p_r(r)=\frac{\Gamma((n-1)/2)}{\sqrt\pi\,\Gamma((n-2)/2)}(1-r^2)^{(n-4)/2},\qquad-1<r<1.}
$$

The normalizing integral is $B(1/2,(n-2)/2)$. To test $\rho=0$ against a two-sided alternative at level $\alpha$, compute $t(r)$ and reject if $|t(r)|>t_{n-2,1-\alpha/2}$, equivalently if

$$
|r|>\frac{t_{n-2,1-\alpha/2}}{\sqrt{n-2+t_{n-2,1-\alpha/2}^2}}.
$$

A one-sided alternative uses the corresponding one-sided tail. Singular [covariance](../../../../../covariance.md) gives $|r|=1$ almost surely when both [variances](../../../../../variance-split.md) are nonzero, and is outside the nondegenerate density calculation.

## ↑ Ancestors (10)

1. [27K](../27k.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
