<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume thermal equilibrium, a three-dimensional [nondegenerate semiconductor](../../../../nondegenerate-semiconductor.md), one parabolic conduction extremum and one parabolic valence extremum, with two spin states in each. Use the supplied [effective masses](../../../../band-effective-mass.md) as scalar density-of-states parameters. With conduction energy $E=E_c+\varepsilon$, state counting gives the per-volume [density of states](../../../../density-of-states.md)

$$
D_c(\varepsilon)=\frac1{2\pi^2}\left(\frac{2m_e^*}{\hbar^2}\right)^{3/2}\sqrt\varepsilon.
$$

Since $E_c-\mu\gg k_BT$, replace the [Fermi-Dirac distribution](../../../../fermi-dirac-distribution.md) by its [Boltzmann factor](../../../../boltzmann-factor.md). Using $x=\varepsilon/(k_BT)$ and the supplied integral,

$$
n=e^{-(E_c-\mu)/(k_BT)}\int_0^\infty D_c(\varepsilon)e^{-\varepsilon/(k_BT)}d\varepsilon
=N_c e^{-(E_c-\mu)/(k_BT)},
$$



$$
N_c=2\left(\frac{m_e^*k_BT}{2\pi\hbar^2}\right)^{3/2}
=2\left(\frac{2\pi m_e^*k_BT}{h^2}\right)^{3/2}.
$$

The [electron hole](../../../../electron-hole.md) occupation is $1-f(E)$ in the [valence band](../../../../valence-band.md). Applying the same integration below $E_v$ gives

$$
p=N_v e^{-(\mu-E_v)/(k_BT)},\qquad
N_v=2\left(\frac{2\pi m_h^*k_BT}{h^2}\right)^{3/2}.
$$

Their product cancels the [chemical potential](../../../../chemical-potential-split.md), giving the [semiconductor mass-action law](../../../../semiconductor-mass-action-law.md)

$$
\boxed{np=4\left(\frac{2\pi k_B}{h^2}\right)^3
(m_e^*m_h^*)^{3/2}T^3e^{-E_g/(k_BT)}.}
$$

Thus, for masses expressed in ordinary mass units,

$$
\boxed{A=4\left(\frac{2\pi k_B}{h^2}\right)^3
=\frac{k_B^3}{2\pi^3\hbar^6},\qquad B=\frac32,\qquad C=3.}
$$

The labels $B,C$ in this last box are exponents, unrelated to the magnetic field or [Curie constant](../../../../curie-constant.md) above. [Valley degeneracy](../../../../valley-degeneracy.md) or multiple valence bands must be included in the [effective density of states](../../../../effective-density-of-states.md), or absorbed into suitable [density-of-states effective masses](../../../../density-of-states-effective-mass.md), not counted twice. Real silicon has anisotropic multiple valleys, so its conductivity mass is not automatically its density-of-states mass; the numerical answers below implement the paper's supplied scalar-mass model.[Slide 26, A Few Cautions: carrier counting uses the density-of-states effective mass, while silicon conductivity and cyclotron masses differ](../../../../ece-340-lecture-6-by-john-dallesasse.md)

The formula is not an identity for arbitrarily degenerate carriers. For a concrete counterexample, take $\mu-E_c=10k_BT$ while holes remain dilute. Fermi occupation gives $n/N_c\simeq24.1$, whereas the Boltzmann replacement would give $e^{10}\simeq22026$; the predicted product then differs by about three orders of magnitude. Separate electron and hole quasi-Fermi levels out of equilibrium would also prevent the cancellation used above.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the condensed matter physics course of the University of Oxford](../../../split.md)
5. [Condensed matter physics course of the University of Oxford](../../../../condensed-matter-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
