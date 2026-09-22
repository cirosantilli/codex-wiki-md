<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [density of states](../../../../density-of-states.md) $g(E)$ counts one-electron states per energy interval, including both [electron spin](../../../../electron-spin.md) orientations. It may be a total or a per-volume quantity; $U$ must have the matching normalization. The [Fermi-Dirac distribution](../../../../fermi-dirac-distribution.md)

$$
f(E,T)=\frac1{e^{(E-\mu(T))/(k_BT)}+1}
$$

is the occupation probability of such a state. In the fixed-volume [free electron model](../../../../free-electron-model.md), the integration variable $E$ and the [density of states](../../../../density-of-states.md) do not depend on $T$. The occupation depends explicitly on $T$ and implicitly through the [chemical potential](../../../../chemical-potential-split.md) $\mu(T)$ needed to preserve electron number. Thermal expansion or a changing [electronic band structure](../../../../electronic-band-structure.md) would require additional effects outside this model.

At $T\ll T_F$, only states within order $k_BT$ of the [Fermi energy](../../../../fermi-energy.md) change their occupation. There are order $g(E_F)k_BT$ such states, each carrying an excitation energy of order $k_BT$. Thus $U(T)-U(0)\propto g(E_F)(k_BT)^2$ and the [electronic heat capacity](../../../../electronic-heat-capacity.md) is proportional to $g(E_F)k_B^2T$. Using the supplied coefficient,

$$
\boxed{C_V=\gamma T,\qquad\gamma=\frac{\pi^2}{3}k_B^2g(E_F),\qquad
U(T)-U(0)=\frac12\gamma T^2.}
$$

The shell argument fixes the scaling, not the numerical coefficient; the controlled [Sommerfeld expansion](../../../../sommerfeld-expansion.md) fixes that coefficient at fixed electron number. Filled states far below $E_F$ cannot accept arbitrary thermal excitations because of the [Pauli exclusion principle](../../../../pauli-exclusion-principle.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
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
