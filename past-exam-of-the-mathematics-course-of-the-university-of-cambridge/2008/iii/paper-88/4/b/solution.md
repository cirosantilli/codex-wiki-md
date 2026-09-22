<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a general colored medium and unit plane-wave input $E(0,\mathbf s)=1$, let $U_W(x,0)$ be the propagator of $\partial_x=i\Delta_\perp/(2k)+ik\mu W(x,\mathbf s)$. Then the solution is

$$
\Gamma(x;\mathbf s_1,\mathbf s_2)=\mathbb E\left[(U_W(x,0)1)(\mathbf s_1)(U_W(x,0)1)(\mathbf s_2)^*\right].
$$

A time-ordered operator exponential defines $U_W$. Its expectation depends on the full longitudinal covariance; the initial Gaussian and transverse-stationarity assumptions do not specify a universal closed expression.

With the stated longitudinal [Gaussian white noise](../../../../../../gaussian-white-noise.md) and transverse [statistical homogeneity](../../../../../../statistical-homogeneity.md), the moment depends only on $\boldsymbol\rho=\mathbf s_1-\mathbf s_2$. Hence $(\Delta_1-\Delta_2)\Gamma=0$. The closed equation in the previous part and initial value $\Gamma(0)=1$ give

$$
\boxed{\Gamma(x,\boldsymbol\rho)=\exp\{-k^2\mu^2x[C(0)-C(\boldsymbol\rho)]\}.}
$$

In particular $\Gamma(x,0)=1$: the ensemble mean intensity remains constant for plane-wave input, even though [coherent attenuation in a white-noise random medium](../../../../../../coherent-attenuation-in-a-white-noise-random-medium.md) reduces the mean complex field.

Use a consistent transverse [power spectrum](../../../../../../power-spectrum.md) convention,

$$
C(\boldsymbol\rho)=\int\frac{d^2\boldsymbol\kappa}{(2\pi)^2}\Phi(\boldsymbol\kappa)e^{i\boldsymbol\kappa\cdot\boldsymbol\rho}.
$$

For an isotropic spectrum, angular integration gives the [isotropic transverse covariance spectrum](../../../../../../isotropic-transverse-covariance-spectrum.md), $C(\rho)=(2\pi)^{-1}\int_0^\infty\Phi(\kappa)J_0(\kappa\rho)\kappa\,d\kappa$. Therefore

$$
\boxed{\Gamma(x,\rho)=\exp\left[-\frac{k^2\mu^2x}{2\pi}
\int_0^\infty\Phi(\kappa)(1-J_0(\kappa\rho))\kappa\,d\kappa\right].}
$$

The supplied two-dimensional [Fourier transform](../../../../../../fourier-transform.md) definition has angular factor $2\pi$, whereas the displayed radial transform pair omits it. The latter is a normalized [Hankel transform](../../../../../../hankel-transform.md) pair. If its radial spectrum is denoted $\Phi_H=\Phi/(2\pi)$, use $\Phi_H$ in the integral and omit the prefactor $1/(2\pi)$. These are equivalent conventions; mixing them changes the attenuation rate.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 88](../../../paper-88-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
