<h1 id="12h/solution">Solution</h1>

↑ **Parent:** [12H](../12h.md)

The [Rao-Blackwell theorem](../../../../../rao-blackwell-theorem.md) says that, for a [sufficient statistic](../../../../../sufficient-statistic.md) $T$ and a finite-second-moment estimator $\delta(X)$, the conditional estimator $\delta_T(T)=E_\theta[\delta(X)\mid T]$ can be chosen independently of the unknown parameter and has no greater [mean squared error](../../../../../mean-squared-error.md) for estimating any specified function $g(\theta)$. Sufficiency makes the [conditional distribution](../../../../../conditional-distribution.md) of the data given $T$ parameter-independent. [Conditional expectation](../../../../../conditional-expectation.md) preserves the [expectation](../../../../../expected-value.md), hence preserves unbiasedness. Writing $\delta-g=(\delta-\delta_T)+(\delta_T-g)$, the cross term has [expectation](../../../../../expected-value.md) zero, because $E[\delta-\delta_T\mid T]=0$. Therefore

$$
E_\theta[(\delta-g)^2]
=E_\theta[(\delta_T-g)^2]+E_\theta[(\delta-\delta_T)^2]
\ge E_\theta[(\delta_T-g)^2].
$$

Equality holds exactly when $\delta=\delta_T$ almost surely. This proves the squared-loss form, including the usual unbiased-estimator [variance](../../../../../variance-split.md) statement.

Here $\theta>0$ is necessary for the stated uniform interval. Put $L=X_{(1)}=\min_iX_i$ and $R=X_{(n)}=\max_iX_i$. The joint density factors as

$$
p_\theta(x)=(2\theta)^{-n}\mathbf1\{\theta<L,\ R<3\theta\}
=(2\theta)^{-n}\mathbf1\{R/3<\theta<L\}.
$$

The [factorization theorem for sufficient statistics](../../../../../fisher-neyman-factorization-theorem.md) shows that **$T=(L,R)$ is sufficient**. Also $E[X_1]=2\theta$, so $X_1/2$ is unbiased and has [variance](../../../../../variance-split.md) $\theta^2/12$.

For $n\ge2$, conditional on distinct extrema $l,r$, [exchangeability](../../../../../exchangeable-random-variables.md) gives probability $1/n$ that $X_1$ is each endpoint; with probability $(n-2)/n$ it is one of the remaining observations, uniform on $(l,r)$. Its conditional mean is consequently

$$
E[X_1\mid L=l,R=r]=\frac{l+r}{n}+\frac{n-2}{n}\frac{l+r}{2}=\frac{l+r}{2}.
$$

Thus the [Rao-Blackwell estimator for a uniform scale interval](../../../../../rao-blackwell-estimator-for-a-uniform-scale-interval.md) is

$$
\boxed{\widetilde\theta=\frac{L+R}{4}},
$$

which is unbiased and has no greater [mean squared error](../../../../../mean-squared-error.md). For $n=1$, $L=R=X_1$ and the same formula reduces to the original estimator. As a quantitative check, the [covariance of two uniform order statistics](../../../../../covariance-of-two-uniform-order-statistics.md) gives

$$
\operatorname{Var}(\widetilde\theta)=\frac{\theta^2}{2(n+1)(n+2)}\le\frac{\theta^2}{12}.
$$

For instance, after writing $X_i=\theta+2\theta U_i$, both extreme uniform [variances](../../../../../variance-split.md) are $n/[(n+1)^2(n+2)]$ and their [covariance](../../../../../covariance.md) is $1/[(n+1)^2(n+2)]$. These formulas follow by integrating the joint extreme density $n(n-1)(r-l)^{n-2}$ on $0<l<r<1$; they also display strict improvement for $n>1$.

## ↑ Ancestors (10)

1. [12H](../12h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
