<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For three odd [fermionic operators](../../../../fermionic-operator.md), the identity

$$
[A,BC]=\{A,B\}C-B\{A,C\}
$$

converts the [commutator](../../../../commutator.md) with a quadratic [Hamiltonian](../../../../hamiltonian.md) into the given [canonical anticommutation relations](../../../../canonical-anticommutation-relations.md). Writing a mode label as $i=(\mathbf p,s)$, this yields

$$
[a_i,a_j^\dagger a_j]=\delta_{ij}a_j,\qquad
[b_i^\dagger,b_j^\dagger b_j]=-\delta_{ij}b_j^\dagger.
$$

The opposite-species number terms commute with each [fermionic creation operator](../../../../fermionic-creation-operator.md) or [fermionic annihilation operator](../../../../fermionic-annihilation-operator.md), because two anticommutations give a positive sign. Restoring the continuous normalization, the [Dirac delta distribution](../../../../dirac-delta-function.md) in the mode brackets cancels $d^3\mathbf q/(2\pi)^3$. Consequently

$$
\boxed{[a^s_{\mathbf p},H]=E_{\mathbf p}a^s_{\mathbf p},\qquad[b^{s\dagger}_{\mathbf p},H]=-E_{\mathbf p}b^{s\dagger}_{\mathbf p}.}
$$

Substitute these into the [mode expansion of a Dirac field](../../../../mode-expansion-of-a-dirac-field.md). The result is

$$
[\psi(x),H]=\int\frac{d^3\mathbf p}{(2\pi)^3\sqrt{2E_{\mathbf p}}}\sum_s E_{\mathbf p}
\left[e^{-ip\cdot x}a^s_{\mathbf p}u^s(\mathbf p)-e^{ip\cdot x}b^{s\dagger}_{\mathbf p}v^s(\mathbf p)\right].
$$

Since $i\partial_t e^{-ip\cdot x}=E_{\mathbf p}e^{-ip\cdot x}$ and $i\partial_t e^{ip\cdot x}=-E_{\mathbf p}e^{ip\cdot x}$, this is exactly

$$
\boxed{i\partial_t\psi(t,\mathbf x)=[\psi(t,\mathbf x),H].}
$$

The [Heisenberg equation of motion](../../../../heisenberg-equation-of-motion.md) uses an ordinary [commutator](../../../../commutator.md) with the even [Hamiltonian](../../../../hamiltonian.md), despite the odd [fermionic operators](../../../../fermionic-operator.md) obeying [anticommutators](../../../../anticommutator.md) among themselves.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
