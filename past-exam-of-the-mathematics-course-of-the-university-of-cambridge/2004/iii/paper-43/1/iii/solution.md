<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $\sigma_i^2=V_{ii}$ and $V_{ij}=\rho_{ij}\sigma_i\sigma_j$. Apply the [Schur complement covariance](../../../../../../schur-complement-covariance.md) to the first two coordinates, conditioning on the third. The [conditional covariance](../../../../../../conditional-covariance.md) and [conditional variances](../../../../../../conditional-variance.md) are

$$
\begin{aligned}
\operatorname{Cov}(X_1,X_2\mid X_3=x_3)&=\sigma_1\sigma_2(\rho_{12}-\rho_{13}\rho_{23}),\\
\operatorname{Var}(X_1\mid X_3=x_3)&=\sigma_1^2(1-\rho_{13}^2),\\
\operatorname{Var}(X_2\mid X_3=x_3)&=\sigma_2^2(1-\rho_{23}^2).
\end{aligned}
$$

Divide the [conditional covariance](../../../../../../conditional-covariance.md) by the product of the conditional [standard deviations](../../../../../../standard-deviation.md). The [conditional correlation](../../../../../../conditional-correlation.md) is therefore

$$
\boxed{\operatorname{Corr}(X_1,X_2\mid X_3=x_3)=\frac{\rho_{12}-\rho_{13}\rho_{23}}{\sqrt{(1-\rho_{13}^2)(1-\rho_{23}^2)}}.}
$$

This is the [partial correlation](../../../../../../partial-correlation.md) after removing the linear effect of $X_3$. For a nonsingular [multivariate normal distribution](../../../../../../multivariate-normal-distribution.md), both residual [variances](../../../../../../variance-split.md) are positive and the answer is independent of $x_3$. If a residual [variance](../../../../../../variance-split.md) vanishes, the requested [correlation coefficient](../../../../../../pearson-correlation-coefficient.md) is undefined, even though the residual [covariance](../../../../../../covariance.md) formula remains valid.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
