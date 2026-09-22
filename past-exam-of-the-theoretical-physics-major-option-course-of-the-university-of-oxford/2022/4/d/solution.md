<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Preserve the primary [constraints](../../../../constraint-mechanics.md) using the corrected [Hamiltonian](../../../../hamiltonian.md) from [solution](../c/solution.md). After a spatial integration by parts, the $B_0$ terms in its density are $B_0\partial_i\pi_i+B_0^*\partial_i\pi_i^*-M^2B_0^*B_0$. [Hamilton's equations](../../../../hamilton-s-equations.md) give

$$
0=\dot\pi_0=-\partial_i\pi_i+M^2B_0^*,\qquad0=\dot\pi_0^*=-\partial_i\pi_i^*+M^2B_0.
$$

With the definitions of $E^i,E^{*i}$ in the paper, the actual massive [Gauss law](../../../../gauss-s-law.md) is therefore

$$
\boxed{\partial_iE^{*i}=M^2B_0^*,\qquad\partial_iE^i=M^2B_0.}
$$

This is also the $\nu=0$ component of the [Proca equation](../../../../proca-equation.md). The zero right-hand sides printed in the source apply only to the massless theory or to special configurations with $B_0=0$.

For a concrete counterexample, take $k\ne0$, $\omega^2=k^2+M^2$, and the longitudinal on-shell [plane wave](../../../../plane-wave.md)

$$
B^\mu=\left(\frac kM,0,0,\frac\omega M\right)e^{-i\omega t+ikz}.
$$

It satisfies $\partial_\mu B^\mu=0$, but $E^3=-iM e^{-i\omega t+ikz}$ and $\partial_iE^i=kM e^{-i\omega t+ikz}\ne0$. Imposing the printed zero-divergence condition would incorrectly remove the physical longitudinal [particle polarization](../../../../particle-polarization.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
