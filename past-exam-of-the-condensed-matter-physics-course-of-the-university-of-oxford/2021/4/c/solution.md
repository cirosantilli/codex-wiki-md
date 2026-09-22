<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In the [hydrogenic donor state](../../../../hydrogenic-donor-state.md) approximation, the screened [Coulomb potential energy](../../../../coulomb-potential-energy.md) is $-e^2/(4\pi\epsilon_0\epsilon_r r)$ and the kinetic term uses $m^*=0.067m_e$. Rescaling the [hydrogen atom](../../../../hydrogen-atom.md) gives the [effective Bohr radius of a hydrogenic donor](../../../../effective-bohr-radius-of-a-hydrogenic-donor.md) and the positive binding [energy](../../../../energy-split.md)

$$
a_b=\frac{4\pi\epsilon_0\epsilon_r\hbar^2}{m^*e^2}
=\frac{12.9}{0.067}a_0,
\qquad
E_b=\frac{\hbar^2}{2m^*a_b^2}
=13.6057\,\mathrm{eV}\frac{0.067}{12.9^2}.
$$

Therefore

$$
\boxed{a_{\rm binding}=10.19\,\mathrm{nm},\qquad E_{\rm binding}=5.48\,\mathrm{meV}.}
$$

The radius here is the exponential length of the ground-state [wavefunction](../../../../wave-function-split.md), not its root-mean-square radius. With $\psi(r)=(\pi a_b^3)^{-1/2}e^{-r/a_b}$, radial integration gives $\langle r^2\rangle=3a_b^2$ and $\langle x^2+y^2\rangle=2a_b^2$.

For dilute independent donors of number [density](../../../../density.md) $n$, a bound [spin](../../../../spin.md) one-half [electron](../../../../electron.md) has [magnetic moment](../../../../magnetic-dipole-moment.md) magnitude $\mu_s=|g|\mu_B/2$, with the [Bohr magneton](../../../../bohr-magneton.md) defined using the bare [electron mass](../../../../electron-mass.md). Its weak-field [Curie law](../../../../curie-s-law.md) response is

$$
\chi_{\rm spin}=\frac{\mu_0n g^2\mu_B^2}{4k_BT}.
$$

For the orbital response, expand the [effective mass](../../../../band-effective-mass.md) [Hamiltonian](../../../../hamiltonian.md) $(\mathbf p+e\mathbf A)^2/(2m^*)$ in a uniform [magnetic field](../../../../magnetic-field-split.md), using $\mathbf A=\mathbf B\times\mathbf r/2$. The spherical ground state has zero orbital [angular momentum](../../../../angular-momentum.md); the quadratic term raises its [energy](../../../../energy-split.md) by

$$
\Delta E_{\rm orb}=\frac{e^2B^2}{8m^*}\langle x^2+y^2\rangle
=\frac{e^2a_b^2}{4m^*}B^2.
$$

Differentiating this [energy](../../../../energy-split.md) twice and using $B\simeq\mu_0H$ gives

$$
\chi_{\rm orb}=-\frac{\mu_0ne^2a_b^2}{2m^*}.
$$

The donor-only [magnetic susceptibility](../../../../magnetic-susceptibility.md) cancels when

$$
\boxed{T_* =\frac{g^2\mu_B^2m^*}{2k_Be^2a_b^2}
=\frac{g^2}{4}\left(\frac{m^*}{m_e}\right)^2\frac{E_b}{k_B}
\simeq1.44\times10^{-2}\,\mathrm K.}
$$

The negative sign of $g=-0.45$ drops out of the linear [magnetic susceptibility](../../../../magnetic-susceptibility.md). This crossover is far below $E_b/k_B\simeq63.6\,\mathrm K$, consistent with donor binding. It assumes sufficiently weak [magnetic field](../../../../magnetic-field-split.md), negligible exchange between donors and a thermal scale above any inter-donor splitting; sufficiently dilute donors can satisfy those assumptions. The background [diamagnetism](../../../../diamagnetism.md) from part (b) is excluded from this cancellation.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the condensed matter physics course of the University of Oxford](../../../split.md)
5. [Condensed matter physics course of the University of Oxford](../../../../condensed-matter-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
