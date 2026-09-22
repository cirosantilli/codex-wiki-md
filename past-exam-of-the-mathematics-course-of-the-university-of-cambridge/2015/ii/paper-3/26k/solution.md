<h1 id="26k/solution">Solution</h1>

↑ **Parent:** [26K](../26k.md)

Let initial wealth be $w$ and let $\theta_i$ be the number of units held of risky asset $i$; the bank investment is $w-\theta^TS_0$. Put $b=\mu-(1+r)S_0$. Terminal wealth is normal, with mean $(1+r)w+\theta^Tb$ and variance $\theta^TV\theta$. The expectation of the [exponential utility](../../../../../constant-absolute-risk-aversion-utility.md) is

$$
\mathbb EU(W_1)=-\exp\left[-\gamma((1+r)w+\theta^Tb)+\frac{\gamma^2}{2}\theta^TV\theta\right].
$$

For $\gamma>0$ and positive definite [covariance matrix](../../../../../covariance-matrix.md) $V$, maximizing this is equivalent to maximizing the [certainty equivalent](../../../../../certainty-equivalent.md) $\theta^Tb-\gamma\theta^TV\theta/2$. Thus **the optimal investment is**

$$
\boxed{\theta^*=\frac1\gamma V^{-1}b,\qquad \hbox{bank investment}=w-(\theta^*)^TS_0.}
$$

All investors have proportional risky holdings. A [market portfolio](../../../../../market-portfolio.md) can therefore be represented by $\theta_M=V^{-1}b$, with any positive scalar multiple giving the same return. Suppose its initial value $P=\theta_M^TS_0$ is positive and $b\ne0$. Set $B=b^TV^{-1}b$. For returns $R_i=S_1^i/S_0^i-1$ and $R_M=\theta_M^TS_1/P-1$,

$$
\mathbb E(R_i-r)=\frac{b_i}{S_0^i},\quad \mathbb E(R_M-r)=\frac BP,\quad \operatorname{Var}R_M=\frac B{P^2},\quad\operatorname{Cov}(R_i,R_M)=\frac{b_i}{S_0^iP}.
$$

The [beta of an asset](../../../../../beta-of-an-asset.md) is its covariance with the market return divided by the market variance. Consequently

$$
\boxed{\beta_i=\frac{b_iP}{S_0^iB},\qquad \mathbb E(R_i-r)=\beta_i\mathbb E(R_M-r).}
$$

This is the [capital asset pricing model](../../../../../capital-asset-pricing-model.md). Since $\beta_i=\rho_i\sigma_i/\sigma_M$, dividing the excess-return identity by $\sigma_i$ gives **the [Sharpe ratio](../../../../../sharpe-ratio.md) identity**

$$
\boxed{\frac{\mathbb E(R_i-r)}{\sigma_i}=\rho_i\frac{\mathbb E(R_M-r)}{\sigma_M}.}
$$

These ratio statements require nonzero variances and nonzero initial portfolio value. If $V$ is singular and $b$ is in its range, replace $V^{-1}$ by its pseudoinverse; any kernel holding can be added to an optimizer. If $b$ has a component in the kernel, it gives a deterministic excess gain that can be scaled without bound, so there is no finite optimal portfolio. If $b=0$, there is no distinguished risky market portfolio and its beta ratios are undefined.

## ↑ Ancestors (10)

1. [26K](../26k.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
