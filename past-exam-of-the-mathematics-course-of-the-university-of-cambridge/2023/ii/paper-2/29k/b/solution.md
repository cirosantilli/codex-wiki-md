<h1 id="29k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $Z_i=(X_i,Y_i)^T$ for the independent observations and put $\Omega=\Sigma^{-1}$. Apart from constants, the log-likelihood is

$$
\ell(\Omega)=\frac n2\log|\Omega|
-\frac12\sum_{i=1}^n Z_i^T\Omega Z_i.
$$

Using the stated matrix derivatives, its [score function](../../../../../../informant-function.md) is

$$
\frac{\partial\ell}{\partial\Omega}
=\frac n2\Omega^{-1}
-\frac12\sum_{i=1}^nZ_iZ_i^T.
$$

At a root of the score, $\Omega^{-1}=n^{-1}\sum_iZ_iZ_i^T$. Hence the [maximum-likelihood covariance estimator for centered Gaussian data](../../../../../../maximum-likelihood-covariance-estimator-for-centered-gaussian-data.md) is

$$
\boxed{
\widehat\Sigma=\frac1n\sum_{i=1}^nZ_iZ_i^T
=\begin{pmatrix}
 n^{-1}\sum_iX_i^2&n^{-1}\sum_iX_iY_i\\
 n^{-1}\sum_iX_iY_i&n^{-1}\sum_iY_i^2
\end{pmatrix}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [29K](../../29k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
