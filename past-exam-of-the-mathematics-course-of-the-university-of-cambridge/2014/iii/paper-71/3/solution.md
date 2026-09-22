<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let the electrolyte [permittivity](../../../../../permittivity.md) be $\varepsilon$ and let $\kappa_D=1/\ell_D$ be the inverse [Debye–Hückel screening length](../../../../../debye-huckel-screening-length.md). We reserve $k$ for the imposed lateral [wavevector](../../../../../wavevector.md). In the [Debye–Hückel approximation](../../../../../debye-huckel-approximation.md), linearization about an electrically neutral bulk electrolyte gives

$$
(\nabla^2-\kappa_D^2)\phi=0
$$

away from fixed charges. For ionic species of valence $z_i$ and bulk number density $n_i$, $\kappa_D^2=\sum_i n_i z_i^2e^2/(\varepsilon k_BT)$; the approximation requires $|z_ie\phi|\ll k_BT$. Substitution of a lateral cosine into this screened [Poisson equation](../../../../../poisson-equation.md) leaves a vertical decay constant

$$
\boxed{p=\sqrt{k^2+\kappa_D^2}.}
$$

The [screened sinusoidal surface-charge mode](../../../../../screened-sinusoidal-surface-charge-mode.md) thus decays faster than a laterally uniform charge mode. A nonzero $k$ retains a finite decay length even in the zero-salt limit.

The exterior media and their boundary conditions are not specified in the paper. Specifying the two [surface charge densities](../../../../../surface-charge-density.md) alone does not fix the normal derivative on the inside unless the outside response is also fixed. We first take the confined-gap idealization, with the prescribed charge supplying all the displacement flux into the electrolyte between the sheets. The [electrostatic interface boundary conditions](../../../../../electrostatic-interface-boundary-conditions.md) are then

$$
\varepsilon\phi_z(x,d/2)=\sigma_+(x),\qquad
-\varepsilon\phi_z(x,-d/2)=\sigma_-(x).
$$

This is, for example, the limit of negligible exterior displacement admittance. The [electrostatic potential](../../../../../electric-potential.md) solving these conditions and the [Debye–Hückel approximation](../../../../../debye-huckel-approximation.md) equation is

$$
\boxed{\phi(x,z)=\frac{\alpha}{\varepsilon p\sinh(pd)}
\left[\cos(kx)\cosh\bigl(p(z+d/2)\bigr)
+\cos(kx+\theta)\cosh\bigl(p(z-d/2)\bigr)\right],\quad |z|<d/2.}
$$

Differentiation checks the two surface signs directly. This solution allows a sine as well as a cosine lateral component when the phase is nonzero.

In linear screened [electrostatics](../../../../../electrostatics.md), the quadratic charging free energy is $\tfrac12\int\sigma\phi\,dA$. It is equivalently $\tfrac\varepsilon2\int[(\nabla\phi)^2+\kappa_D^2\phi^2]\,dV$ with the stated boundary conditions. The second term represents the linearized ionic response; integrating only the bare [electric field](../../../../../electric-field.md) energy would omit it. If $\mathcal A$ denotes membrane area, the wavelength-averaged energy density is

$$
\frac E{\mathcal A}=\frac12\left\langle\sigma_+\phi(x,d/2)+\sigma_-\phi(x,-d/2)\right\rangle_x.
$$

Using $\langle\cos^2(kx)\rangle_x=1/2$ and $\langle\cos(kx)\cos(kx+\theta)\rangle_x=\cos\theta/2$ gives the [phase registration of screened charged sheets](../../../../../phase-registration-of-screened-charged-sheets.md) energy

$$
\boxed{\frac E{\mathcal A}=\frac{\alpha^2}{2\varepsilon p}
\left[\coth(pd)+\frac{\cos\theta}{\sinh(pd)}\right].}
$$

The positive cosine coefficient shows that, for nonzero charge amplitude and finite separation,

$$
\boxed{\theta_{\min}=\pi\pmod{2\pi},\qquad
\frac{E_{\min}}{\mathcal A}=\frac{\alpha^2}{2\varepsilon p}\tanh(pd/2).}
$$

At the minimum the [electrostatic potential](../../../../../electric-potential.md) simplifies to $\phi=\alpha\cos(kx)\sinh(pz)/[\varepsilon p\cosh(pd/2)]$. Positive and negative charge patches face opposite signs across the gap. The two charge patterns therefore favor a half-wavelength lateral offset rather than like-charge alignment.

For comparison, if identical electrolyte fills all of space on both sides of infinitesimally thin charge sheets, the [electrostatic interface boundary conditions](../../../../../electrostatic-interface-boundary-conditions.md) are continuity of $\phi$, decay at infinity, and the charge-induced derivative jumps

$$
\phi_z(z_s^+)-\phi_z(z_s^-)=-\sigma_s(x)/\varepsilon.
$$

Superposing the two [screened sinusoidal surface-charge modes](../../../../../screened-sinusoidal-surface-charge-mode.md) gives, in particular between the sheets,

$$
\boxed{\phi(x,z)=\frac{\alpha}{2\varepsilon p}
\left[\cos(kx)e^{-p(d/2-z)}+\cos(kx+\theta)e^{-p(d/2+z)}\right].}
$$

Its full-space continuation replaces each vertical distance by the corresponding absolute distance. Evaluating the [electrostatic potential](../../../../../electric-potential.md) on both sheets now yields

$$
\boxed{\frac E{\mathcal A}=\frac{\alpha^2}{4\varepsilon p}
\left[1+e^{-pd}\cos\theta\right],\qquad \theta_{\min}=\pi\pmod{2\pi}.}
$$

The constant term is the two isolated-sheet self energies, and the cosine term is their screened interaction. The energy depends on the exterior convention, but both stated physical idealizations give the same [phase registration of screened charged sheets](../../../../../phase-registration-of-screened-charged-sheets.md): unlike charge patches oppose each other. In the full-space convention the optimum interaction energy is $-\alpha^2e^{-pd}/(4\varepsilon p)$, giving an attractive normal [force](../../../../../force.md) density $-\alpha^2e^{-pd}/(4\varepsilon)$. Phase sensitivity becomes exponentially weak for $pd\gg1$; if $\alpha=0$ or the separation tends to infinity there is no selected phase.

One can also display how an exterior dielectric response interpolates between these cases. Let $Y_o\ge0$ be its normal displacement admittance for this lateral [Fourier mode](../../../../../fourier-mode.md): $Y_o=0$ for the confined-gap idealization, $Y_o=\varepsilon p$ for identical exterior electrolyte, and $Y_o=\varepsilon_o|k|$ for an ion-free exterior dielectric. Define

$$
D_s=\varepsilon p\tanh(pd/2)+Y_o,\qquad
D_a=\varepsilon p\coth(pd/2)+Y_o.
$$

The symmetric and antisymmetric surface-charge combinations give

$$
\frac E{\mathcal A}=\frac{\alpha^2}{4}
\left[\frac{1+\cos\theta}{D_s}+\frac{1-\cos\theta}{D_a}\right].
$$

Since $D_s<D_a$, its cosine coefficient is positive. This makes the phase-minimizing conclusion robust while exposing the boundary information needed for an absolute [electrostatic energy](../../../../../electrostatic-energy.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 71](../../paper-71-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
