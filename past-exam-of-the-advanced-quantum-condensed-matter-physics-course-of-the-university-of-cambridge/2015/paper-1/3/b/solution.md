<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Expand the field operator in orthonormal localized orbitals, $\hat\psi(\mathbf r)=\sum_i\phi_i(\mathbf r)c_i$. For a one-electron continuum [Hamiltonian](../../../../../hamiltonian.md) $h_0=\hat p^2/(2m^*)+V(\mathbf r)$, projection gives

$$
H_0=\sum_{ij}h_{ij}c_i^\dagger c_j,\qquad
h_{12}=\int d^3r\,\phi_1^*(\mathbf r)
\left[\frac{\hat p^2}{2m^*}+V(\mathbf r)\right]\phi_2(\mathbf r).
$$

The coefficient in the displayed [lattice](../../../../../lattice.md) [Hamiltonian](../../../../../hamiltonian.md) is $-t_{12}$. Thus the [projected hopping matrix element and sign convention](../../../../../projected-hopping-matrix-element-and-sign-convention.md) require

$$
\boxed{-t_{12}=h_{12}=K_{12}+V_{12},\qquad
K_{12}=\int d^3r\,\phi_1^*\frac{\hat p^2}{2m^*}\phi_2.}
$$

[Orthogonality](../../../../../orthogonal-vectors.md) states $\int\phi_1^*\phi_2=0$; it does not imply $\int\phi_1^*V\phi_2=0$ for a spatially varying potential. If the off-diagonal potential is assumed zero, for example when it is a constant, the hopping coefficient is $h_{12}=K_{12}$. This is the kinetic integral requested by the paper, but it equals $-t_{12}$ under the paper's own leading-minus convention. A convention writing the hopping term with a plus sign would instead call $h_{12}$ itself $t_{12}$.

**The printed positive equality is not a consequence of the stated [orthogonality](../../../../../orthogonal-vectors.md) assumption and the displayed sign convention.** [Orthogonality does not diagonalize a varying potential](../../../../../orthogonality-does-not-diagonalize-a-varying-potential.md) gives an explicit counterexample to the underlying inference. The general projected relation above states the supported result; setting $V_{12}=0$ still leaves $-t_{12}=K_{12}$ in the question's convention. Rephasing an orbital changes both $h_{12}$ and the coefficient of the corresponding operator together; it does not remove this algebraic sign mismatch in a fixed convention. The spectrum in the remaining two-site calculation depends on $|t|^2$, so those parts are unaffected.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the advanced Quantum Condensed Matter Physics course of the University of Cambridge](../../../../split.md)
6. [Advanced Quantum Condensed Matter Physics course of the University of Cambridge](../../../../../advanced-quantum-condensed-matter-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
