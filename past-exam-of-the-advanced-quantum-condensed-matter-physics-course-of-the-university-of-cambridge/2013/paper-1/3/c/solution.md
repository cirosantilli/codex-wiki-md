<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[Density functional theory](../../../../../density-functional-theory.md) replaces the interacting many-electron [ground state](../../../../../ground-state.md) [wavefunction](../../../../../wave-function-split.md) by its spatial density $n(\mathbf r)$. For fixed interaction and a nondegenerate ground state, the [Hohenberg-Kohn theorem](../../../../../hohenberg-kohn-theorem.md) fixes the external potential up to an additive constant. If two distinct potentials gave the same density, their strict variational energy inequalities would sum to the contradiction $E_0+E'_0<E_0+E'_0$.

The [density functional variational principle](../../../../../density-functional-variational-principle.md) minimizes

$$
E_v[n]=F[n]+\int v(\mathbf r)n(\mathbf r)\,d^3r,\qquad
F[n]=\min_{\Psi\to n}\langle\Psi|T+W|\Psi\rangle,
$$

over admissible densities of the correct particle number. The universal $F$ contains the kinetic and interaction energies. This is exact in principle; an explicit useful functional is the practical difficulty.[1964: density-potential uniqueness and density variational principle](../../../../../inhomogeneous-electron-gas-by-pierre-hohenberg-and-walter-kohn.md)

The [Kohn-Sham equations](../../../../../kohn-sham-equations.md) introduce noninteracting orbitals with the same density and decompose $F=T_s+E_H+E_{\rm xc}$. With $n=\sum_i f_i|\phi_i|^2$,

$$
\left[-\frac{\hbar^2\nabla^2}{2m_e}+v+v_H[n]+v_{\rm xc}[n]\right]\phi_i=\epsilon_i\phi_i,\qquad
v_H=\frac{e^2}{4\pi\epsilon_0}\int\frac{n(\mathbf r')}{|\mathbf r-\mathbf r'|}\,d^3r',\quad
v_{\rm xc}=\frac{\delta E_{\rm xc}}{\delta n}.
$$

The [exchange-correlation functional](../../../../../exchange-correlation-functional.md) includes exchange, correlation and the interacting kinetic-energy correction relative to $T_s$. Guess a density, construct the potentials, solve and occupy orbitals, then mix and iterate to [self-consistent field](../../../../../self-consistent-field.md) convergence. The [local density approximation](../../../../../local-density-approximation.md) uses $E_{\rm xc}^{\rm LDA}=\int n\epsilon_{\rm xc}^{\rm uniform}(n)\,d^3r$; a [generalized gradient approximation](../../../../../generalized-gradient-approximation.md) also depends on density gradients.

**Kohn–Sham orbital energies are not generally excitation energies**, and their sum double counts interactions. The [Kohn-Sham energy double-counting correction](../../../../../kohn-sham-energy-double-counting-correction.md) is

$$
\boxed{E=\sum_i f_i\epsilon_i-E_H+E_{\rm xc}-\int n v_{\rm xc}\,d^3r,}
$$

with ion–ion energy added for a total crystal energy. Approximate functionals can miss self-interaction cancellation, band gaps and strong correlation; convergence alone does not prove the global ground state.[1965: auxiliary noninteracting system and effective density-dependent equations](../../../../../self-consistent-equations-including-exchange-and-correlation-effects-by-walter-kohn-and-lu-jeu-sham.md)

## ↑ Ancestors (14)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
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
