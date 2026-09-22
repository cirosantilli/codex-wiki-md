<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the standard [canonical anticommutation relations](../../../../canonical-anticommutation-relations.md) for the two distinct [fermionic](../../../../fermion.md) orbitals. In particular $\{a,b^\dagger\}=\{a^\dagger,b\}=0$, in addition to the relations explicitly listed in the paper; these mixed relations are part of the usual two-orbital [fermionic Fock space](../../../../fermionic-fock-space.md) interpretation. Normalize the original [vacuum state](../../../../vacuum-state.md) by $\langle0|0\rangle=1$ and fix the ordering

$$
|n_a n_b\rangle=(a^\dagger)^{n_a}(b^\dagger)^{n_b}|0\rangle.
$$

The [canonical anticommutation relations](../../../../canonical-anticommutation-relations.md) give $a^2=(a^\dagger)^2=0$ and $aa^\dagger=1-a^\dagger a$. Consequently the [number operator](../../../../number-operator.md) is an [orthogonal projector](../../../../orthogonal-projection.md):

$$
N_a^2=a^\dagger aa^\dagger a
=a^\dagger(1-a^\dagger a)a=N_a.
$$

The same holds for $N_b$. Hence each [eigenvalue](../../../../eigenvalue.md) obeys $n^2=n$ and is either $0$ or $1$, expressing the [Pauli exclusion principle](../../../../pauli-exclusion-principle.md). Also $[N_a,N_b]=0$, so the two [number operators](../../../../number-operator.md) have a simultaneous [orthonormal basis](../../../../orthonormal-basis.md) of [Fock states](../../../../fock-state.md):

$$
\begin{array}{c|c|c}
\text{state}&N_a\text{ eigenvalue}&N_b\text{ eigenvalue}\\\hline
|00\rangle=|0\rangle&0&0\\
|10\rangle=a^\dagger|0\rangle&1&0\\
|01\rangle=b^\dagger|0\rangle&0&1\\
|11\rangle=a^\dagger b^\dagger|0\rangle&1&1
\end{array}
$$

**Each [number operator](../../../../number-operator.md) has [eigenvalues](../../../../eigenvalue.md) $0,1$, each with [state degeneracy](../../../../state-degeneracy.md) two.** For $N_a$, the zero [eigenspace](../../../../eigenspace.md) is spanned by $|00\rangle,|01\rangle$ and the unit [eigenspace](../../../../eigenspace.md) by $|10\rangle,|11\rangle$; for $N_b$, these are respectively $|00\rangle,|10\rangle$ and $|01\rangle,|11\rangle$. Any normalized [linear combination](../../../../linear-combination.md) within one such [eigenspace](../../../../eigenspace.md) is also an [eigenstate](../../../../eigenstate.md) of that [number operator](../../../../number-operator.md).

The ordering convention will matter below: $b^\dagger a^\dagger|0\rangle=-|11\rangle$ and

$$
ab|11\rangle=aba^\dagger b^\dagger|0\rangle
=-aa^\dagger bb^\dagger|0\rangle=-|0\rangle.
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../../advanced-quantum-theory-path-integrals-and-many-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
