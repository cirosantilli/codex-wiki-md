<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a vertical interband transition, the [crystal momentum](../../../../crystal-momentum.md) is effectively unchanged because the [photon momentum](../../../../photon-momentum.md) is small. A stimulated downward transition needs an occupied upper state and an empty lower state, with factor $f_c(E_2)[1-f_v(E_1)]$; upward [photon absorption](../../../../photon-absorption.md) has factor $f_v(E_1)[1-f_c(E_2)]$. The two matrix elements agree by microscopic reversibility. Their difference is therefore

$$
f_c(1-f_v)-f_v(1-f_c)=f_c-f_v,
\qquad \boxed{\alpha(\omega)\propto g_j(\omega)[f_c(E_2)-f_v(E_1)].}
$$

A common slowly varying transition-strength factor is implicit. Broadening replaces the sharp transition by a convolution; multiple valence bands contribute separate terms.

For one isotropic pair of parabolic [energy bands](../../../../energy-band.md), write

$$
E_2=E_c+\frac{\hbar^2k^2}{2m_e^*},\qquad
E_1=E_v-\frac{\hbar^2k^2}{2m_h^*},\qquad
\frac1{m_r}=\frac1{m_e^*}+\frac1{m_h^*}.
$$

Thus $E_2-E_1=E_g+\hbar^2k^2/(2m_r)$. Including the usual twofold spin degeneracy, the number of paired states per volume inside a sphere of radius $k$ is $k^3/(3\pi^2)$. Differentiating with respect to transition [energy](../../../../energy-split.md) $E$ gives the [three-dimensional parabolic interband joint density of states](../../../../three-dimensional-parabolic-interband-joint-density-of-states.md)

$$
\boxed{g_j^{(E)}(E)=\frac{1}{2\pi^2}\left(\frac{2m_r}{\hbar^2}\right)^{3/2}\sqrt{E-E_g}\,\Theta(E-E_g).}
$$

For density per [angular frequency](../../../../angular-frequency.md), $g_j^{(\omega)}(\omega)=\hbar g_j^{(E)}(\hbar\omega)$. Stating the density convention avoids a missing factor of $\hbar$; other degeneracies multiply the formula.

At a common carrier [temperature](../../../../temperature-split.md), the [Fermi-Dirac distribution](../../../../fermi-dirac-distribution.md) is a strictly decreasing function of $E-F$. The [direct-gap semiconductor gain condition](../../../../direct-gap-semiconductor-gain-condition.md) follows:

$$
f_c(E_2)>f_v(E_1)
\iff E_2-F_c<E_1-F_v
\iff \boxed{E_g<\hbar\omega<F_c-F_v.}
$$

The lower inequality denotes a transition above the ideal band edge, where the displayed [joint density of states](../../../../joint-density-of-states.md) is nonzero. Thus [quasi-Fermi-level splitting](../../../../quasi-fermi-level-splitting.md) must exceed the transition [photon energy](../../../../photon-energy.md). Equality is transparency, rather than net amplification; at zero [temperature](../../../../temperature-split.md) an allowed transition must also lie within the occupied-electron and empty-valence windows.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
