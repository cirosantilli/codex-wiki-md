<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Stack the observations as $y=(y_1^T,y_2^T)^T$ and set

$$
\mu_\theta=
\begin{pmatrix}c\mathbf1\\(c+\Delta m)\mathbf1\end{pmatrix}.
$$

Let $K_f(a,b)$ and $K_g(a,b)$ denote matrices obtained by evaluating the two [Gaussian process](../../../../../../gaussian-process.md) [covariance kernels](../../../../../../covariance-kernel.md). Independence of the [quasar light curve](../../../../../../quasar-light-curve.md), [gravitational microlensing](../../../../../../gravitational-microlensing.md), and [Gaussian noise](../../../../../../gaussian-noise.md) processes gives

$$
C_\theta=
\begin{pmatrix}
K_f(t,t)+K_g(t,t)+E_1&K_f(t,t-\Delta t)\\
K_f(t-\Delta t,t)&K_f(t-\Delta t,t-\Delta t)+K_g(t,t)+E_2
\end{pmatrix},
$$

where $E_i=\operatorname{diag}(\sigma_{i,1}^2,\ldots,\sigma_{i,N}^2)$. Thus $y\mid\theta$ is a [multivariate normal distribution](../../../../../../multivariate-normal-distribution.md) and its [Gaussian-process marginal likelihood](../../../../../../gaussian-process-marginal-likelihood.md) is

$$
\boxed{p(y_1,y_2\mid\theta)
=(2\pi)^{-N}|C_\theta|^{-1/2}
\exp\!\left[-\frac12(y-\mu_\theta)^TC_\theta^{-1}(y-\mu_\theta)\right].}
$$

The off-diagonal blocks are essential: both images contain the same delayed [Ornstein-Uhlenbeck process](../../../../../../ornstein-uhlenbeck-process.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
