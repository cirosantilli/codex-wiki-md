<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $\beta=k\xi\mu$. The [random phase screen](../../../../../../random-phase-screen.md) produces

$$
E(0,z)=e^{i\beta W(z)},\qquad
\widehat E(x,\nu)=e^{-i\nu^2x/(2k)}\widehat E(0,\nu).
$$

Interpret the normality assumption as a jointly [Gaussian process](../../../../../../gaussian-process.md), not merely Gaussian one-point [marginal distributions](../../../../../../marginal-distribution.md). Write its normalized [autocorrelation](../../../../../../autocorrelation.md) as $\rho(\zeta)=\langle W(z+\zeta)W(z)\rangle$. The difference $W(z+\zeta)-W(z)$ is a zero-mean [Gaussian random variable](../../../../../../gaussian-random-variable.md) with [variance](../../../../../../variance-split.md) $2(1-\rho(\zeta))$. Its [characteristic function](../../../../../../characteristic-function.md) therefore gives the [Gaussian phase-screen correlation](../../../../../../gaussian-phase-screen-correlation.md)

$$
\boxed{C_E(\zeta):=\langle E(0,z+\zeta)\overline{E(0,z)}\rangle
=\exp\{-\beta^2[1-\rho(\zeta)]\}.}
$$

Without joint Gaussianity the [autocorrelation](../../../../../../autocorrelation.md) alone does not determine this expectation.

For an acoustic pressure amplitude $\psi$, with background mass density $\rho_0$, the time-averaged [acoustic energy flux](../../../../../../acoustic-energy-flux.md) is

$$
I_x=\frac{1}{2\rho_0\omega}\operatorname{Im}(\overline\psi\,\partial_x\psi).
$$

An acoustic potential convention changes the dimensional prefactor. The physical field includes the carrier $e^{ikx}$: a transverse [Fourier transform](../../../../../../fourier-transform.md) mode has axial [wavenumber](../../../../../../wavenumber.md) $\kappa_\nu=k-\nu^2/(2k)$ in the [parabolic wave equation](../../../../../../parabolic-wave-equation.md). Thus its [spectral acoustic flux](../../../../../../spectral-acoustic-flux.md) is proportional to $\kappa_\nu|\widehat E(x,\nu)|^2$, or to $k|\widehat E(x,\nu)|^2$ at leading paraxial order. Differentiating the reduced field alone would omit the carrier contribution.

The infinite stationary illumination has a [spectral measure of a stationary random field](../../../../../../spectral-measure-of-a-stationary-random-field.md), rather than a finite ordinary value of $\langle|\widehat E|^2\rangle$ at each $\nu$. To specify the normalization, truncate the screen to an aperture of length $L$, propagate this truncated initial field, and set

$$
\widehat E_L(0,\nu)=\frac1{2\pi}\int_{-L/2}^{L/2}E(0,z)e^{-i\nu z}\,dz.
$$

The propagation multiplier has modulus one. Using the [Gaussian phase-screen correlation](../../../../../../gaussian-phase-screen-correlation.md) and the overlap of the two aperture intervals gives

$$
\boxed{\langle|\widehat E_L(x,\nu)|^2\rangle
=\frac1{4\pi^2}\int_{-L}^{L}(L-|\zeta|)
e^{-\beta^2[1-\rho(\zeta)]}e^{-i\nu\zeta}\,d\zeta,\qquad x>0.}
$$

Multiplication by $\kappa_\nu/(2\rho_0\omega)$ gives the ensemble-averaged pressure-normalized modal [acoustic energy flux](../../../../../../acoustic-energy-flux.md) for this finite-aperture convention.

The [infinite-aperture spectral normalization](../../../../../../infinite-aperture-spectral-normalization.md) consistent with the specified [Fourier transform](../../../../../../fourier-transform.md) is

$$
\boxed{S_E(\nu)=\lim_{L\to\infty}\frac{2\pi}{L}
\langle|\widehat E_L(x,\nu)|^2\rangle
=\frac1{2\pi}\int_{\mathbb R}e^{-\beta^2[1-\rho(\zeta)]}e^{-i\nu\zeta}\,d\zeta.}
$$

The integral and limit are understood as [spectral measures of a stationary random field](../../../../../../spectral-measure-of-a-stationary-random-field.md) when necessary. By [Parseval's identity](../../../../../../parseval-identity.md), this is power per unit transverse length: $\int_{\mathbb R}S_E(d\nu)=C_E(0)=1$. **The ensemble-averaged axial [spectral acoustic flux](../../../../../../spectral-acoustic-flux.md) is independent of $x$:**

$$
\boxed{\frac{d\langle I_x\rangle}{d\nu}
=\frac{\kappa_\nu}{2\rho_0\omega}S_E(\nu)
\simeq I_{\rm inc}S_E(\nu),\qquad I_{\rm inc}=\frac{k}{2\rho_0\omega}.}
$$

Here the notation includes [Dirac delta distributions](../../../../../../dirac-delta-function.md) in the [spectral measure of a stationary random field](../../../../../../spectral-measure-of-a-stationary-random-field.md); the leading-order total flux is $I_{\rm inc}$. The $\kappa_\nu$ correction is meaningful within $|\nu|\ll k$, the range of the [paraxial approximation](../../../../../../paraxial-approximation.md).

If $\rho(\zeta)\to0$ and $e^{\beta^2\rho(\zeta)}-1$ is integrable, the [stationary phase-screen power spectrum](../../../../../../stationary-phase-screen-power-spectrum.md) separates into [coherent and diffuse wave fields](../../../../../../coherent-and-diffuse-wave-fields.md):

$$
S_E(\nu)=e^{-\beta^2}\delta(\nu)
+\frac{e^{-\beta^2}}{2\pi}\int_{\mathbb R}
[e^{\beta^2\rho(\zeta)}-1]e^{-i\nu\zeta}\,d\zeta.
$$

The coherent fraction is $e^{-\beta^2}$ and the diffuse fraction is $1-e^{-\beta^2}$. If additionally $|\beta|\ll1$, the [stationary phase-screen power spectrum](../../../../../../stationary-phase-screen-power-spectrum.md) is $(1-\beta^2)\delta+\beta^2\widehat\rho+O(\beta^4)$ with the same [Fourier transform](../../../../../../fourier-transform.md) convention. Small $\mu$ alone does not imply small accumulated phase $k\xi\mu$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
