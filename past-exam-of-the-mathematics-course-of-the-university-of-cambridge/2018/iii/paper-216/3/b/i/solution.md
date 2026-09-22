<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the printed parameterization $\lambda=\sigma^2$, $v=\sigma_0^2$, and $a=\sqrt\rho$. Let $T=365$, $X$ be the [design matrix](../../../../../../../design-matrix.md) with rows $x_i^T$, and $r=\theta-X\beta$. Conditional on $\theta$ and the parameters, $Y$ contributes no extra dependence on $Z$ by [conditional independence](../../../../../../../conditional-independence.md).

The stationary autoregressive [normal distribution](../../../../../../../normal-distribution.md) has prior density proportional to

$$
\exp\left[-\frac12\left(z_1^2+\frac1{1-a^2}\sum_{i=2}^T(z_i-az_{i-1})^2\right)\right].
$$

Its [Gaussian autoregressive conditional precision](../../../../../../../gaussian-autoregressive-conditional-precision.md) is the [tridiagonal matrix](../../../../../../../tridiagonal-matrix.md) $J$ with

$$
J_{11}=J_{TT}=\frac1{1-a^2},\quad
J_{ii}=\frac{1+a^2}{1-a^2}\ (1<i<T),\quad
J_{i,i+1}=J_{i+1,i}=-\frac a{1-a^2}.
$$

Combining this prior with $r\mid Z\sim N(\lambda Z,vI)$ and completing the square gives

$$
\boxed{Z\mid\beta,\sigma^2,\sigma_0^2,\rho,\theta,x,Y
\sim N(Q^{-1}h,Q^{-1}),\quad Q=J+\frac{\sigma^4}{\sigma_0^2}I,\quad h=\frac{\sigma^2}{\sigma_0^2}(\theta-X\beta).}
$$

The [precision matrix](../../../../../../../precision-matrix.md) $Q$ is positive definite. Compute its lower [Cholesky decomposition](../../../../../../../cholesky-decomposition.md) $Q=LL^T$, solve $Qm=h$, draw $\xi\sim N(0,I_T)$, and solve $L^T\eta=\xi$. Then return $Z=m+\eta$. This [Gaussian sampling from a precision Cholesky factor](../../../../../../../gaussian-sampling-from-a-precision-cholesky-factor.md) is exact because $\operatorname{Cov}(\eta)=L^{-T}L^{-1}=Q^{-1}$. Tridiagonal structure gives linear cost in $T$ and preserves the conditional correlation between days. Notice that the solve uses $L^T$, not $L$.

These conditionals are normalized for every fixed positive $\sigma^2,\sigma_0^2$, despite the joint posterior impropriety explained in part (a). If the intended model uses $\sigma Z_i$ instead, replace the observation coefficient $\lambda$ by $\sigma$ throughout; the information and precision terms then use $\sigma/v$ and $\sigma^2/v$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 216](../../../../paper-216-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
