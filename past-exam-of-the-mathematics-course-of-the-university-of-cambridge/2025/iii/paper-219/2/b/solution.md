<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First integrate out $\eta_i$: conditional on $\xi_i$, $y_i\sim N(\alpha+\beta\xi_i,s^2)$ with $s^2=\sigma^2+\sigma_y^2$. Since $(x_i,y_i)$ is an affine transformation of independent normal variables, it is [bivariate normal](../../../../../../multivariate-normal-distribution.md) with mean

$$
m=\binom{\mu}{\alpha+\beta\mu}
$$

and covariance

$$
\Sigma=
\begin{pmatrix}
A&B\\B&C
\end{pmatrix},
\quad
A=\tau^2+\sigma_x^2,
\quad B=\beta\tau^2,
\quad C=\beta^2\tau^2+s^2.
$$

Its determinant simplifies to

$$
D=AC-B^2=(\tau^2+\sigma_x^2)s^2+\beta^2\tau^2\sigma_x^2.
$$

For $r_i=(x_i-\mu,y_i-\alpha-\beta\mu)^T$, the observed-data likelihood is therefore

$$
L=(2\pi)^{-N}D^{-N/2}
\exp\!\left[-\frac12\sum_{i=1}^N
r_i^T\Sigma^{-1}r_i\right],
\qquad
\Sigma^{-1}=\frac1D\begin{pmatrix}C&-B\\-B&A\end{pmatrix}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
