<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

At $\sigma=1$, complete the square:

$$
x^2+y^2-2\rho xy=(x-\rho y)^2+(1-\rho^2)y^2.
$$

For fixed $y$, all factors not involving $x$ enter its conditional [normalizing constant](../../../../../../normalizing-constant.md). Interchanging the roles of the coordinates gives

$$
\boxed{X\mid Y=y\sim N(\rho y,1-\rho^2),\qquad Y\mid X=x\sim N(\rho x,1-\rho^2).}
$$

These are the [full conditional distributions](../../../../../../full-conditional-distribution.md) of the standard [bivariate normal distribution](../../../../../../bivariate-normal-distribution.md) with correlation $\rho$.

A systematic [Gibbs sampler](../../../../../../gibbs-sampler.md) starts at a chosen $(x_0,y_0)$ and, at each sweep, draws [independent](../../../../../../independent-random-variables.md) standard normals $Z_{1,n},Z_{2,n}$ and sets

$$
x_{n+1}=\rho y_n+\sqrt{1-\rho^2}\,Z_{1,n},\qquad y_{n+1}=\rho x_{n+1}+\sqrt{1-\rho^2}\,Z_{2,n}.
$$

The second update uses the newly drawn $x_{n+1}$. Both coordinate updates preserve the target by part (a), hence so does the sweep. The [Gaussian two-coordinate Gibbs recursion](../../../../../../gaussian-two-coordinate-gibbs-recursion.md) is explicitly

$$
y_{n+1}=\rho^2y_n+\sqrt{1-\rho^2}(\rho Z_{1,n}+Z_{2,n}),
$$

an [AR(1)](../../../../../../autoregressive-process-of-order-one.md) recursion with innovation [variance](../../../../../../variance-split.md) $1-\rho^4$. Its stationary [variance](../../../../../../variance-split.md) is one, and its correlation at sweep lag $k$ is $\rho^{2k}$, displaying the dependence of the sample.

The printed general-$\sigma$ expression has a separate normalization defect: for $\sigma>0$ its integral is $\sigma$, not one, since the exponent has [covariance](../../../../../../covariance.md) $\sigma^2\begin{pmatrix}1&\rho\\\rho&1\end{pmatrix}$, whose normalizing denominator is $2\pi\sigma^2\sqrt{1-\rho^2}$. Retaining that exponent requires $\sigma^2$ in the prefactor. The requested $\sigma=1$ target is already normalized, so this defect does not alter the [conditional distributions](../../../../../../conditional-distribution.md) above.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
