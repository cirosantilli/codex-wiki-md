# Fresnel diffraction phase curvature

↑ **Parent:** [Fresnel diffraction](fresnel-diffraction.md)

The quadratic [wave phase](phase-waves.md) follows from an ordinary distance calculation. Write $\rho^2=(x-\xi)^2+(y-\eta)^2$. The [Taylor expansion](taylor-expansion.md) of the distance to a screen [point](point-geometry.md) is

$$
r=\sqrt{z^2+\rho^2}=z+\frac{\rho^2}{2z}-\frac{\rho^4}{8z^3}+O\!\left(\frac{\rho^6}{z^5}\right).
$$

In the slowly varying propagation prefactor, $r\simeq z$ suffices. In the [complex exponential](complex-exponential-function.md) $e^{ikr}$, however, a small distance error is multiplied by the large [wavenumber](wavenumber.md) $k$. Retaining the quadratic term while dropping the quartic term requires both $\rho/z\ll1$ and $k\rho^4/(8z^3)\ll1$ over the contributing [aperture](aperture.md) and the screen region being considered. The second condition is a [wave phase](phase-waves.md) accuracy requirement; the first is the geometric [paraxial approximation](paraxial-approximation.md).

Expanding the retained quadratic term separates three effects:

$$
U(x,y,z)\simeq\frac{e^{ikz}e^{i\pi(x^2+y^2)/(\lambda z)}}{i\lambda z}\iint_{\mathbb R^2}\underbrace{U_0(\xi,\eta)e^{i\pi(\xi^2+\eta^2)/(\lambda z)}}_{\text{field with aperture phase curvature}}e^{-2\pi i(x\xi+y\eta)/(\lambda z)}d\xi\,d\eta.
$$

The outside quadratic factor changes the [wave phase](phase-waves.md) at each screen [point](point-geometry.md) but has unit [complex modulus](complex-modulus.md), so it leaves that screen's [light intensity](light-intensity.md) unchanged. The quadratic factor inside the [integral](integral-split.md) changes relative [wave phases](phase-waves.md) between contributions from different aperture [points](point-geometry.md), so it changes their [wave interference](interference-wave-propagation.md). The remaining linear factor supplies a [Fourier transform](fourier-transform-split.md). [Fraunhofer diffraction](fraunhofer-diffraction.md) drops the aperture quadratic factor when it is nearly constant; it does not require dropping the screen quadratic factor when predicting a later coherent field.

There is also a useful proof from the [Helmholtz equation](helmholtz-equation.md). Substituting $U=e^{ikz}u$ gives $u_{zz}+2iku_z+u_{xx}+u_{yy}=0$. Neglecting $u_{zz}$ yields the [parabolic wave equation](parabolic-wave-equation.md). A transverse [Fourier transform](fourier-transform-split.md) evolves each [spatial frequency](spatial-frequency.md) $\boldsymbol\nu$ by $\exp[-iz|\boldsymbol\nu|^2/(2k)]$, using the transform kernel $e^{-i\boldsymbol\nu\cdot\mathbf x}$. Its inverse [Fourier transform](fourier-transform-split.md) is the quadratic [Fresnel propagator](fresnel-propagator.md) kernel above. Thus quadratic [wave phase](phase-waves.md) in space and quadratic [wave phase](phase-waves.md) in [spatial frequency](spatial-frequency.md) are two views of the same propagation.

## ↑ Ancestors (6)

1. [Fresnel diffraction](fresnel-diffraction.md)
2. [Physical optics](physical-optics-split.md)
3. [Optics](optics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
