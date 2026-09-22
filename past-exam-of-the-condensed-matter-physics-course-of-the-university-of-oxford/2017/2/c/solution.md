<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $g_v(E)$ denote the spin-summed [density of states](../../../../density-of-states.md) per volume. An electron moment with magnitude the [Bohr magneton](../../../../bohr-magneton.md) $\mu_B$ has [Zeeman energies](../../../../zeeman-energy.md) $\mp\mu_B B$. At low [temperature](../../../../temperature-split.md), the two spin populations are

$$
n_\pm=\frac12\int_0^{\mu\pm\mu_B B}g_v(E)\,dE,
\qquad
n_+-n_-=g_v(E_F)\mu_B B+O(B^3).
$$

The common [chemical potential](../../../../chemical-potential-split.md) changes only at order $B^2$, so it does not affect this linear imbalance. The [magnetization](../../../../magnetization.md) is $M=\mu_B(n_+-n_-)=\mu_B^2g_v(E_F)B$. Define SI volume [magnetic susceptibility](../../../../magnetic-susceptibility.md) by $M=\chi_p H$ and take the weak applied field as $B\simeq\mu_0H$. Then [Pauli paramagnetism](../../../../pauli-paramagnetism.md) gives

$$
\boxed{\chi_p=\mu_0\mu_B^2g_v(E_F)=\frac{3\mu_0n\mu_B^2}{2E_F}.}
$$

The last equality uses the three-dimensional parabolic [free electron model](../../../../free-electron-model.md), $g_v(E_F)=3n/(2E_F)$. This susceptibility is nearly independent of [temperature](../../../../temperature-split.md) for $T\ll T_F$, unlike the [Curie law](../../../../curie-s-law.md) for localized independent moments. The displayed result excludes orbital [diamagnetism](../../../../diamagnetism.md) and interaction enhancements. If susceptibility instead denotes $\partial M/\partial B$, omit $\mu_0$; confusing that convention with $\partial M/\partial H$ changes the units.

## ↑ Ancestors (12)

1. [C](../c.md)
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
