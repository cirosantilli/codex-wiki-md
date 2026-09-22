<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write the perturbation as $\eta e^{ikx+st}$ and use the same factor for all velocity and pressure amplitudes. At the upper interface, the linearized [kinematic boundary condition](../../../../../kinematic-boundary-condition.md), zero tangential traction, and normal-stress balance are

$$
v=s\eta,
\qquad
u_y+v_x=0,
\qquad
-p+2\mu v_y
=\left(\frac{3V}{h_0^4}-\gamma k^2\right)\eta
\quad(y=h_0).
$$

The first term in the normal stress is the linearization of the attractive [disjoining pressure](../../../../../disjoining-pressure.md) $V/h^3$, while the second is the stabilizing [capillary pressure](../../../../../capillary-pressure.md). Symmetry about $y=0$ makes $u$ even and $v$ odd, and supplies the lower-interface conditions.

For a two-dimensional Fourier mode, the [Papkovich–Neuber representation](../../../../../papkovich-neuber-representation.md) is equivalently expressed by the odd [biharmonic stream function for planar Stokes flow](../../../../../biharmonic-stream-function-for-planar-stokes-flow.md)

$$
\psi(y)=A\sinh(ky)+By\cosh(ky),
\qquad
u=\psi_y,
\qquad
v=-ik\psi.
$$

The tangential-stress condition at $y=h_0$, with $K=kh_0$, gives

$$
Ak\sinh K+B(\sinh K+K\cosh K)=0,
$$

whereas the kinematic condition gives $iB\sinh K=s\eta$. The associated normal traction is

$$
-p+2\mu v_y
=\mu k s\eta\frac{2K+\sinh2K}{\sinh^2K}.
$$

Equating this with the linearized interfacial traction yields the [dispersion relation](../../../../../dispersion-relation.md)

$$
\boxed{
s=\frac{3V}{\mu h_0^3}
\frac{(1-\Gamma K^2)\sinh^2K}
{K(2K+\sinh2K)},
\qquad
\Gamma=\frac{\gamma h_0^2}{3V}.}
$$

This is the [Van der Waals rupture instability of a viscous sheet](../../../../../van-der-waals-rupture-instability-of-a-viscous-sheet.md).

For $\Gamma=0$, the growth rate is positive, starts from $3V/(4\mu h_0^3)$ as $K\to0$, and decreases to zero like $3V/(2\mu h_0^3K)$ as $K\to\infty$. For $\Gamma=1$, it has the same long-wave limit, vanishes at $K=1$, and is negative for $K>1$: [surface tension](../../../../../surface-tension.md) damps wavelengths shorter than the cutoff. Long waves feel the attractive interaction but require coherent flow over a large distance; at short wavelengths viscous resistance suppresses the clean-film instability, while capillarity adds direct decay. A finite film size, [fluid inertia](../../../../../navier-stokes-equation.md), surrounding-fluid stresses, gravity, surface viscosity, and failure of the continuum [disjoining pressure](../../../../../disjoining-pressure.md) law can shift the observable most unstable wavelength.

During a growing thin spot, interfacial flow stretches the surface and dilutes its [surfactant](../../../../../surfactant.md), thereby increasing the local surface tension above $\gamma_0$. Adjacent less-stretched regions retain more surfactant and lower tension. The resulting [surface-tension gradient](../../../../../marangoni-effect.md) pulls toward the thin spot and opposes the outward flow that drives thinning. This is [surfactant stabilization of film rupture](../../../../../surfactant-stabilization-of-film-rupture.md); in the strong limit the surfaces behave almost as immobile boundaries.

For strong surfactant and $\Gamma\gg1$, instability requires $K=O(\Gamma^{-1/2})$. The [Taylor expansion](../../../../../taylor-expansion.md)

$$
\frac{\sinh2K-2K}{4K\cosh^2K}
=\frac{K^2}{3}+O(K^4)
$$

reduces the supplied relation to

$$
s\sim\frac{V}{\mu h_0^3}K^2(1-\Gamma K^2).
$$

It is maximal at

$$
\boxed{K_{\max}^2=\frac1{2\Gamma},
\qquad
s_{\max}=\frac{V}{4\mu h_0^3\Gamma}
=\frac{3V^2}{4\mu\gamma_0h_0^5}.}
$$

Thus the characteristic rupture time is $s_{\max}^{-1}=4\mu\gamma_0h_0^5/(3V^2)$. Surfactant greatly extends the life of a soap bubble while its film is moderately thick, but the $h_0^{-5}$ growth-rate dependence predicts rapid final rupture after drainage has made the film sufficiently thin.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 329](../../paper-329-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
