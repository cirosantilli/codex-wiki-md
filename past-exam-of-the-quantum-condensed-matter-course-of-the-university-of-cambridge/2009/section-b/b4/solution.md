<h1 id="section-b/b4/solution">Solution</h1>

↑ **Parent:** [B4](../b4.md)

In a conductor, mobile [electrons](../../../../electron.md) redistribute in response to an [electric potential](../../../../electric-potential.md), producing an induced [charge density](../../../../charge-density.md) that opposes its source. Finite electronic compressibility means a finite density change requires a change of local kinetic [Fermi energy](../../../../fermi-energy.md). Screening is therefore not perfect at every microscopic distance. On scales comparable to atomic structure or the [Fermi wavelength](../../../../fermi-wavelength.md), a continuum local-density model itself fails.

[Thomas-Fermi screening](../../../../thomas-fermi-screening.md) treats electrons as a locally uniform degenerate [free electron gas](../../../../free-electron-model.md), replaces the ionic background by a smooth neutralizing charge, and neglects nonlocal response, exchange and correlation corrections. The electrochemical [chemical potential](../../../../chemical-potential-split.md) is uniform in equilibrium. Because an electron has charge $-e$, its electrostatic energy is $-eV$, giving

$$
\mu=E_F(n)-eV,\qquad E_F(n)=\frac{\hbar^2}{2m}(3\pi^2n)^{2/3}.
$$

At zero potential $\mu=E_{F0}$. Linearizing at fixed $\mu$, with $|eV|\ll E_{F0}$, gives

$$
\frac{2E_{F0}}{3n_0}\delta n=eV,\qquad
\boxed{\rho_{\rm ind}=-e\delta n=-\frac{3e^2n_0}{2E_{F0}}V.}
$$

Insert this in [Poisson's equation](../../../../poisson-s-equation.md) to obtain $(\nabla^2-\xi^{-2})V=-\rho_{\rm free}/\epsilon_0$, where the [Thomas-Fermi screening length](../../../../thomas-fermi-screening-length.md) is

$$
\boxed{\xi=\sqrt{\frac{2\epsilon_0E_{F0}}{3e^2n_0}}.}
$$

Away from a point source, direct radial differentiation shows $\nabla^2(e^{-r/\xi}/r)=\xi^{-2}e^{-r/\xi}/r$. The decaying solution is therefore $V=Ce^{-r/\xi}/r$. Integrating [Poisson's equation](../../../../poisson-s-equation.md) over a small sphere containing charge $Q$ fixes $C=Q/(4\pi\epsilon_0)$. For a sufficiently large source, the linearized formula is only a far-field approximation, not a justified description of its singular core.

For monovalent [sodium](../../../../sodium.md), the electron number density is its atomic number density,

$$
n_0=\frac{968}{0.023}N_A=2.53\times10^{28}\ \mathrm{m^{-3}}.
$$

This gives $E_{F0}=3.15\ \mathrm{eV}$ and

$$
\boxed{\xi=6.76\times10^{-11}\ \mathrm m=0.0676\ \mathrm{nm}.}
$$

Room temperature is far below the corresponding [Fermi temperature](../../../../fermi-temperature.md), so degeneracy is well justified, and sodium's simple conduction band makes a free-electron estimate useful. However $k_F\xi=0.615$ and the mean atomic spacing is $n_0^{-1/3}=0.340\ \mathrm{nm}$. The potential varies on a scale shorter than $k_F^{-1}$ and the atomic spacing, so the slowly varying local-density and continuum assumptions are not quantitatively controlled at the screening length itself. A nonlocal treatment includes [Friedel oscillations](../../../../friedel-oscillations.md), absent from the pure exponential.

Nearly unchanged interlayer force constants in two-layer and twenty-layer films are consistent with very local screening and bonding forces: reducing the distant bulk need not strongly change the force between adjacent layers. They also indicate that metallic electronic response can survive in the thin film. The observation does not by itself validate the numerical Thomas-Fermi approximation, establish an identical full phonon spectrum, or rule out surface-induced electronic changes; it directly constrains the measured local force constant.

## ↑ Ancestors (13)

1. [B4](../b4.md)
2. [Section B](../../section-b.md)
3. [2009](../../../2009-split.md)
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
