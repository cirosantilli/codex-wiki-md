<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Set $\psi=e^{ikx+\mu\chi_1+O(\mu^2)}$. Substitution into the [Helmholtz equation](../../../../../../helmholtz-equation.md) gives the first [Rytov approximation](../../../../../../rytov-approximation.md) equation

$$
(\Delta+2ik\partial_x)\chi_1=-2k^2W.
$$

For the forward parabolic approximation, omit $\partial_x^2\chi_1$. With zero perturbation at $x=0$, the [Fresnel propagator](../../../../../../fresnel-propagator.md) then gives

$$
\boxed{\chi_1(x,\mathbf s)=ik\int_0^x
\exp\!\left[\frac{i(x-u)\Delta_\perp}{2k}\right]W(u,\mathbf s)\,du,
\qquad \psi_R=e^{ikx}e^{\mu\chi_1}.}
$$

A jointly [Gaussian random field](../../../../../../gaussian-random-field.md) makes $\chi_1$ a centered complex Gaussian variable. The [complex Gaussian exponential moment](../../../../../../complex-gaussian-exponential-moment.md) therefore gives the [first-Rytov coherent mean](../../../../../../first-rytov-coherent-mean.md)

$$
\boxed{\mathbb E[\psi_R]=e^{ikx}\exp\left(\frac{\mu^2}{2}\mathbb E[\chi_1^2]\right).}
$$

The second moment here has no complex conjugation. It cannot be replaced by the positive intensity variance $\mathbb E[|\chi_1|^2]$.

For example, let $\widehat C(u,v;\boldsymbol\kappa)$ be the transverse spectrum of the covariance between depths $u$ and $v$. The Fourier multiplier of the [Fresnel propagator](../../../../../../fresnel-propagator.md) is $e^{-i(x-u)|\boldsymbol\kappa|^2/(2k)}$, so

$$
\mathbb E[\chi_1^2]=-k^2\int_0^x\int_0^x du\,dv
\int\frac{d^2\boldsymbol\kappa}{(2\pi)^2}\widehat C(u,v;\boldsymbol\kappa)
\exp\left[-\frac{i|\boldsymbol\kappa|^2(2x-u-v)}{2k}\right].
$$

This supplies the requested mean in terms of medium statistics. For the longitudinal white-noise model, $\widehat C=\delta(u-v)\Phi$, which reduces the double longitudinal integral to one.

The exponential is the mean of the first-order logarithmic model. It is not a complete second-order perturbation expansion of the true mean: the omitted logarithmic term $\mu^2\chi_2$ can itself have a nonzero mean. Strictly at first order, $\mathbb E[\psi]=e^{ikx}+O(\mu^2)$. As an independent check, the closed white-noise parabolic model gives exactly

$$
\mathbb E[E]=\exp[-k^2\mu^2C(0)x/2]
$$

for plane-wave input. A truncated first-Rytov covariance expression with transverse diffraction need not equal this exact mean; omitted logarithmic terms account for the difference.

## ↑ Ancestors (11)

1. [C](../c.md)
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
