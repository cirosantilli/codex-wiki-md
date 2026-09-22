<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Dielectric screening](../../../../dielectric-screening.md) is the rearrangement of a medium's charges in response to an applied charge. In a metal, mobile [electrons](../../../../electron.md) accumulate near a positive perturbation and reduce its long-range potential. [Thomas-Fermi screening](../../../../thomas-fermi-screening.md) treats the [electron gas](../../../../electron-gas.md) locally as an equilibrium gas whose density responds to the local [electrostatic potential](../../../../electric-potential.md), ignoring gradients of the density on the microscopic wavelength scale.

Take $e>0$, background [permittivity](../../../../permittivity-split.md) $\varepsilon_b$, and [electrostatic potential](../../../../electric-potential.md) $\phi$. An [electron](../../../../electron.md)'s [potential energy](../../../../potential-energy.md) is $-e\phi$, so the local kinetic [Fermi energy](../../../../fermi-energy.md) becomes $\mu+e\phi$. For a three-dimensional spin-degenerate parabolic band at zero [temperature](../../../../temperature-split.md),

$$
n(\phi)=\frac1{3\pi^2}\left[\frac{2m(\mu+e\phi)}{\hbar^2}\right]^{3/2},\qquad \delta n\simeq e\,g(E_F)\phi,
$$

where $g(E_F)=dn/d\mu$ is the **[spin-summed density of states](../../../../spin-summed-density-of-states.md) per volume per [energy](../../../../energy-split.md)**. The induced charge is $\rho_{\mathrm{ind}}=-e\delta n=-e^2g(E_F)\phi$. Combining it with [Poisson equation](../../../../poisson-s-equation.md) gives

$$
\boxed{(\nabla^2-k_{\mathrm{TF}}^2)\phi=-\frac{\rho_{\mathrm{ext}}}{\varepsilon_b},\qquad k_{\mathrm{TF}}^2=\frac{e^2g(E_F)}{\varepsilon_b}.}
$$

For a point external charge $Q$, [spherical symmetry](../../../../spherical-symmetry.md) and decay at infinity select

$$
\boxed{\phi(r)=\frac{Q}{4\pi\varepsilon_b r}e^{-r/\lambda_{\mathrm{TF}}},\qquad \lambda_{\mathrm{TF}}=\sqrt{\frac{\varepsilon_b}{e^2g(E_F)}}.}
$$

Thus the bare $1/r$ potential is cut off exponentially. [Fourier transformation](../../../../fourier-transform-split.md) makes the same result transparent: $\phi(\mathbf q)=\rho_{\mathrm{ext}}(\mathbf q)/[\varepsilon_b(q^2+k_{\mathrm{TF}}^2)]$, so the static longitudinal dielectric factor is $1+k_{\mathrm{TF}}^2/q^2$ relative to the background. For a free [electron](../../../../electron.md) band, $g(E_F)=3n/(2E_F)$ and $\lambda_{\mathrm{TF}}^2=2\varepsilon_bE_F/(3ne^2)$.

<a id="2/a/image-local-thomas-fermi-screening-and-optical-acoustic-modes-of-an-illustrative-diatomic-chain"></a>
![](../../../../past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2017-screening-and-phonons.png)

**[Figure 2](#2/a/image-local-thomas-fermi-screening-and-optical-acoustic-modes-of-an-illustrative-diatomic-chain). Local Thomas-Fermi screening and optical/acoustic modes of an illustrative diatomic chain**.

The local linear approximation requires a weak perturbation and slowly varying fields on the relevant microscopic scale. It omits nonlocal [Friedel oscillations](../../../../friedel-oscillations.md) and atom-scale structure; a nonlinear local-density treatment is needed near a sufficiently strong charge. Finite [temperature](../../../../temperature-split.md) replaces $g(E_F)$ by the appropriate [compressibility](../../../../compressibility.md) derivative $\partial n/\partial\mu$. The nondegenerate limit gives classical screening rather than the degenerate Thomas-Fermi length. A larger [density of states](../../../../density-of-states.md) means that a smaller potential can move more carriers, hence stronger screening.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the quantum condensed matter course of the University of Cambridge](../../../split.md)
5. [Quantum Condensed Matter course of the University of Cambridge](../../../../quantum-condensed-matter-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
