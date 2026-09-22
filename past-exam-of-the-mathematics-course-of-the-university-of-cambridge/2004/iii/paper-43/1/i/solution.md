<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write the [expected value](../../../../../../expected-value.md) as $\mu^T=(\mu_1^T,\mu_2^T)$ and assume the relevant [covariance matrix](../../../../../../covariance-matrix.md) $V_{22}$ is invertible. Remove the linear predictor from the first block by defining

$$
Y=X_1-\mu_1-V_{12}V_{22}^{-1}(X_2-\mu_2).
$$

A [linear image of a multivariate normal vector](../../../../../../linear-image-of-a-multivariate-normal-vector.md) is again [multivariate normal](../../../../../../multivariate-normal-distribution.md). Direct [covariance](../../../../../../covariance.md) calculation gives

$$
\operatorname{Cov}(Y,X_2)=V_{12}-V_{12}V_{22}^{-1}V_{22}=0.
$$

Thus $Y$ and $X_2$ are [independent](../../../../../../independent-random-variables.md): [uncorrelated jointly Gaussian variables are independent](../../../../../../uncorrelated-jointly-normal-variables-are-independent.md). Expanding the [covariance matrix](../../../../../../covariance-matrix.md) of $Y$, using $V_{21}=V_{12}^T$, gives

$$
\begin{aligned}
\operatorname{Cov}(Y)
&=V_{11}-V_{12}V_{22}^{-1}V_{21}-V_{12}V_{22}^{-1}V_{21}
 +V_{12}V_{22}^{-1}V_{22}V_{22}^{-1}V_{21}\\
&=V_{11}-V_{12}V_{22}^{-1}V_{21}.
\end{aligned}
$$

Conditioning on $X_2=x_2$ translates $Y$ by the fixed vector $\mu_1+V_{12}V_{22}^{-1}(x_2-\mu_2)$ and leaves its [covariance matrix](../../../../../../covariance-matrix.md) unchanged. Consequently the [conditional multivariate normal distribution](../../../../../../conditional-multivariate-normal-distribution.md) is

$$
X_1\mid X_2=x_2\sim N\!\left(\mu_1+V_{12}V_{22}^{-1}(x_2-\mu_2),\ \boxed{V_{11}-V_{12}V_{22}^{-1}V_{21}}\right).
$$

The [conditional covariance](../../../../../../conditional-covariance.md) is the [Schur complement](../../../../../../schur-complement.md) and does not depend on $x_2$.

## ↑ Ancestors (11)

1. [I](../i.md)
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
