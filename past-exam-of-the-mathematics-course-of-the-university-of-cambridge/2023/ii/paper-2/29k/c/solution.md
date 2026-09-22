<h1 id="29k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Set $a=\Sigma_{11}$, $c=\Sigma_{12}$, and $b=\Sigma_{22}$. The estimator is the sample mean of the independent random vectors

$$
W_i=(X_i^2,X_iY_i,Y_i^2)^T,
\qquad
\mathbb EW_i=(a,c,b)^T.
$$

The supplied fourth moments give

$$
\begin{aligned}
\operatorname{Var}(X^2)&=2a^2,&
\operatorname{Cov}(X^2,XY)&=2ac,&
\operatorname{Cov}(X^2,Y^2)&=2c^2,\\
\operatorname{Var}(XY)&=ab+c^2,&
\operatorname{Cov}(XY,Y^2)&=2bc,&
\operatorname{Var}(Y^2)&=2b^2.
\end{aligned}
$$

Therefore the [multivariate central limit theorem](../../../../../../multivariate-central-limit-theorem.md) gives

$$
\boxed{
\sqrt n
\left[
\begin{pmatrix}
\widehat\Sigma_{11}\\
\widehat\Sigma_{12}\\
\widehat\Sigma_{22}
\end{pmatrix}
-
\begin{pmatrix}a\\c\\b\end{pmatrix}
\right]
\xrightarrow d
N_3\!\left(0,
\begin{pmatrix}
2a^2&2ac&2c^2\\
2ac&ab+c^2&2bc\\
2c^2&2bc&2b^2
\end{pmatrix}\right).}
$$

This is the [asymptotic covariance of the bivariate Gaussian covariance estimator](../../../../../../asymptotic-covariance-of-the-bivariate-gaussian-covariance-estimator.md).

## ↑ Ancestors (11)

1. [C](../c.md)
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
