<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Equal [effective masses](../../../../band-effective-mass.md) and equal [spin](../../../../spin.md) and [valley degeneracies](../../../../valley-degeneracy.md) give [electron-hole symmetry](../../../../electron-hole-symmetry.md). In the [intrinsic semiconductor](../../../../intrinsic-semiconductor.md), [charge neutrality](../../../../charge-neutrality.md) requires equal numbers of [conduction band](../../../../conduction-band.md) [electrons](../../../../electron.md) and [valence band](../../../../valence-band.md) [holes](../../../../electron-hole.md). It therefore pins the [chemical potential](../../../../chemical-potential-split.md) to the band touching point, $\mu=0$. The [Fermi-Dirac distribution](../../../../fermi-dirac-distribution.md) gives

$$
N_c=D\int_0^\infty\frac{dE}{e^{E/(k_BT)}+1}
=Dk_BT\ln2,
\qquad
\boxed{N_c(T)=\frac{Am^*k_BT}{\pi\hbar^2}\ln2.}
$$

Measured relative to the filled [valence band](../../../../valence-band.md) at zero [temperature](../../../../temperature-split.md), the thermal [internal energy](../../../../internal-energy-split.md) includes both species. Removing a [valence band](../../../../valence-band.md) [electron](../../../../electron.md) at $-E$ costs the positive [hole](../../../../electron-hole.md) [energy](../../../../energy-split.md) $E$, just as adding a [conduction band](../../../../conduction-band.md) [electron](../../../../electron.md) at $E$ does. Hence

$$
\Delta U=2D\int_0^\infty\frac{E\,dE}{e^{E/(k_BT)}+1}
=\frac{\pi^2}{6}D(k_BT)^2.
$$

Differentiate at fixed area and fixed total electronic [particle number](../../../../particle-number.md), allowing creation of [electron-hole pairs](../../../../electron-hole-pair.md):

$$
C_v^{\rm tot}=\frac{\pi^2}{3}Dk_B^2T,\qquad
\boxed{\frac{C_v^{\rm tot}}{N_c}=\frac{\pi^2}{3\ln2}k_B\simeq4.746\,k_B.}
$$

There is no conflict with the [equipartition theorem](../../../../equipartition-theorem.md). The normalization $N_c$ counts only the excited [conduction band](../../../../conduction-band.md) [electrons](../../../../electron.md), while the [heat capacity](../../../../heat-capacity.md) includes both [electrons](../../../../electron.md) and [holes](../../../../electron-hole.md); moreover, $N_c\propto T$ is not fixed. In fact $\Delta U/N_c=\pi^2k_BT/(6\ln2)$, and differentiating $N_c(T)$ supplies another equal contribution to the [heat capacity](../../../../heat-capacity.md). Finally, $\mu=0$ gives occupation $1/2$ at the touching point, so the excitation gas is not in the classical dilute limit even though $k_BT$ exceeds the vanishing [band gap](../../../../band-gap.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
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
