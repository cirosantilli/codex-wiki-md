<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Under [homoskedasticity](../../../../../../homoskedasticity.md), write

$$
C=\sigma_{\mathrm{int}}^2+\sigma_m^2+\sigma_C^2,
\qquad H=\sigma_{\mathrm{int}}^2+\sigma_m^2.
$$

Then $\widehat M_0=\bar q$ and $\widehat\theta=\bar q-\bar r$. Both are [unbiased estimators](../../../../../../unbiased-estimator.md), and their [covariance matrix](../../../../../../covariance-matrix.md) is

$$
\boxed{
\operatorname{Cov}\begin{pmatrix}\widehat M_0\\\widehat\theta\end{pmatrix}
=\begin{pmatrix}
C/K&C/K\\
C/K&C/K+H/N
\end{pmatrix}.}
$$

Indeed the [Fisher information](../../../../../../fisher-information-matrix.md) is

$$
I(M_0,\theta)=
\begin{pmatrix}K/C+N/H&-N/H\\-N/H&N/H\end{pmatrix},
$$

and its inverse is exactly the displayed covariance matrix. The estimators therefore attain the multivariate [Cramér-Rao bound](../../../../../../cramer-rao-bound.md) and are [efficient estimators](../../../../../../efficient-estimator.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
