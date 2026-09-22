<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Hamiltonian density](../../../../hamiltonian-density.md) is $\mathcal H=[\dot\phi^2+(\partial_x\phi)^2+m^2\phi^2]/2$. In the vacuum only $\langle a_na_m^\dagger\rangle=\delta_{nm}$ contributes. Hence

$$
\langle\dot\phi^2\rangle=\sum_n\frac{\omega_n}{L}\sin^2(k_nx),\quad
\langle(\partial_x\phi)^2\rangle=\sum_n\frac{k_n^2}{\omega_nL}\cos^2(k_nx),\quad
\langle\phi^2\rangle=\sum_n\frac{\sin^2(k_nx)}{\omega_nL}.
$$

Substitution, using $\omega_n^2=k_n^2+m^2$, yields

$$
\boxed{\langle\mathcal H(x)\rangle
=\sum_{n=1}^\infty\left[\frac{\omega_n}{2L}-\frac{m^2}{2\omega_nL}\cos(2k_nx)\right].}
$$

This [Dirichlet scalar vacuum energy density](../../../../dirichlet-scalar-vacuum-energy-density.md) illustrates why a massive field's local unregularized energy density need not be uniform. The cosine integrates to zero over the interval, so

$$
\boxed{E_0^{\rm BC}(L)=\int_0^Ldx\,\langle\mathcal H(x)\rangle
=\frac12\sum_{n=1}^\infty\omega_n.}
$$

These divergent expressions are understood with a common regulator before exchanging sums, integrals or derivatives. [Normal ordering](../../../../normal-ordering.md) the [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md) separately in each geometry would erase the vacuum terms one is trying to compare; a common regulated subtraction is used instead in [c](../c.md) and [d](../d.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [7](../../7.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
