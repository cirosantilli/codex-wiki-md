<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $\mathbf r=(y,z)$ and prescribe a deterministic entrance field $E_0(\mathbf r)$. Substitution of the carrier into the [Helmholtz equation](../../../../../../helmholtz-equation.md) gives

$$
2ikE_x+E_{xx}+\Delta_\perp E+k^2(n^2-1)E=0.
$$

The usual weak-index paraxial model drops $E_{xx}$ and linearizes $n^2-1=2\mu W+O(\mu^2)$, giving

$$
E_x=DE+iaWE,\qquad D=\frac{i}{2k}\Delta_\perp,\quad a=k\mu.
$$

All the mean-field formulas below use this model. If the $\mu^2W^2$ term in $n^2$ is retained, its extra mean and fluctuations must also be included; Gaussian averaging of the linear random potential alone is then insufficient.

For a colored medium, taking [expectations](../../../../../../expected-value.md) gives the exact propagation identity

$$
\boxed{m_x=Dm+ia\langle WE\rangle,\qquad m(0)=E_0,\qquad m=\langle E\rangle.}
$$

[Stationarity](../../../../../../stationary-process.md) and Gaussianity alone do not close the last term. To make its dependence precise, let $C(s,\mathbf r)=\langle W(x+s,\mathbf r_0+\mathbf r)W(x,\mathbf r_0)\rangle$ and let $U_W(x,s;\mathbf r,\mathbf r')$ be the random paraxial propagator. Assuming a jointly [Gaussian random field](../../../../../../gaussian-random-field.md), rather than only Gaussian one-point marginals, the [functional derivative](../../../../../../functional-derivative.md) of the solution is

$$
\frac{\delta E(x,\mathbf r)}{\delta W(s,\mathbf r')}=ia\,U_W(x,s;\mathbf r,\mathbf r')E(s,\mathbf r'),\qquad0<s<x.
$$

The [Furutsu–Novikov formula](../../../../../../novikov-s-theorem.md) therefore yields

$$
\boxed{m_x(x,\mathbf r)=Dm(x,\mathbf r)-a^2\int_0^x ds\int_{\mathbb R^2}d\mathbf r'\,C(x-s,\mathbf r-\mathbf r')\left\langle U_W(x,s;\mathbf r,\mathbf r')E(s,\mathbf r')\right\rangle.}
$$

This is a propagation equation for the mean, with the remaining correlation displayed rather than silently replacing it by a product of means.

The general solution can be written explicitly as a Gaussian-averaged phase-screen product. Put $\Delta=x/N$, $x_j=j\Delta$, $\mathbf r_N=\mathbf r$ and let

$$
K_\Delta(\mathbf r)=\frac{k}{2\pi i\Delta}\exp\left(\frac{ik|\mathbf r|^2}{2\Delta}\right)
$$

be the [integral](../../../../../../integral.md) kernel of the [Fresnel propagator](../../../../../../fresnel-propagator.md). Successive free-propagation and random-phase steps, followed by Gaussian averaging, give the [colored Gaussian paraxial mean propagator](../../../../../../colored-gaussian-paraxial-mean-propagator.md)

$$
\boxed{m(x,\mathbf r)=\lim_{N\to\infty}\int_{(\mathbb R^2)^N}E_0(\mathbf r_0)\prod_{j=1}^N K_\Delta(\mathbf r_j-\mathbf r_{j-1})\,
\exp\left[-\frac{a^2\Delta^2}{2}\sum_{j,l=1}^N C(x_j-x_l,\mathbf r_j-\mathbf r_l)\right]\prod_{j=0}^{N-1}d\mathbf r_j.}
$$

For smooth colored media this is the time-slicing representation, with oscillatory [integrals](../../../../../../integral.md) understood by the usual Fresnel regularization. At finite $N$ the exponential follows directly from the [characteristic function](../../../../../../characteristic-function.md) of the jointly Gaussian phase sum. It exhibits why a general transverse [covariance](../../../../../../covariance.md) cannot be replaced by its value at zero separation along every diffraction path.

For completeness, the unlinearized paraxial model has $E_x=DE+iaWE+i(k\mu^2/2)W^2E$ and the corresponding mean equation includes $i(k\mu^2/2)\langle W^2E\rangle$. Its colored-medium solution uses the same time-slicing [integral](../../../../../../integral.md), replacing the Gaussian factor by

$$
\det\bigl(I-ik\mu^2\Delta\mathsf C\bigr)^{-1/2}\exp\left[-\frac{a^2\Delta^2}{2}\mathbf1^T\bigl(I-ik\mu^2\Delta\mathsf C\bigr)^{-1}\mathsf C\mathbf1\right],\qquad
\mathsf C_{jl}=C(x_j-x_l,\mathbf r_j-\mathbf r_l).
$$

This follows by completing the square in the finite-dimensional [Gaussian integral](../../../../../../gaussian-integral.md), with the determinant branch continuous from $\mu=0$. It supplies the generic colored-medium mean when the $W^2$ term is retained. A square of ideal [white noise](../../../../../../white-noise.md) is not defined by the [covariance](../../../../../../covariance.md) in part (b); that limit uses the linear random-potential model and its stated drift.

If transverse diffraction of the fluctuations is neglected, the simpler straight-ray approximation gives

$$
\boxed{m(x,\mathbf r)=E_0(\mathbf r)\exp\left[-a^2\int_0^x(x-s)C(s,\mathbf0)\,ds\right],\qquad m_x=-a^2\left[\int_0^x C(s,\mathbf0)ds\right]m.}
$$

Indeed $E=E_0\exp[ia\int_0^xW(s,\mathbf r)ds]$ and the [variance](../../../../../../variance-split.md) of its phase is $2a^2\int_0^x(x-s)C(s,\mathbf0)ds$. If $W$ is constant transversely, this formula is exact with $E_0$ replaced by the free diffracted field $e^{xD}E_0$. For example $W=Z$, a single standard normal variable constant throughout space, satisfies [stationarity](../../../../../../stationary-process.md) and unit [variance](../../../../../../variance-split.md) but gives $m=e^{-a^2x^2/2}e^{xD}E_0$. Thus **a constant-rate exponential attenuation is not a consequence of part (a)'s assumptions alone**. It becomes the closed paraxial result under the longitudinal white-noise assumption in the next part.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
