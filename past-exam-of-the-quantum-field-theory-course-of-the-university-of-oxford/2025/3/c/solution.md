<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $i<j$, interchange the entries in slots $i,j$ while preserving the order of all intermediate [fermionic creation operators](../../../../fermionic-creation-operator.md). Move $a_j^\dagger$ left through $j-i$ factors, then move $a_i^\dagger$ right through the remaining $j-i-1$ intermediate factors. The [canonical anticommutation relations](../../../../canonical-anticommutation-relations.md) give the overall [fermionic sign](../../../../fermionic-sign.md)

$$
(-1)^{(j-i)+(j-i-1)}=(-1)^{2(j-i)-1}=-1.
$$

Hence

$$
\boxed{|1,\ldots,j,\ldots,i,\ldots,n\rangle=-|1,\ldots,i,\ldots,j,\ldots,n\rangle.}
$$

More generally any [permutation](../../../../permutation.md) $\pi$ gives

$$
\boxed{|\pi(1),\ldots,\pi(n)\rangle=\operatorname{sgn}(\pi)|1,\ldots,n\rangle.}
$$

The [sign of a permutation](../../../../sign-of-a-permutation.md) is independent of its decomposition into adjacent interchanges. Thus the $n$-[particle](../../../../particle-physics.md) sector is an [exterior power](../../../../exterior-power.md) of the one-[particle](../../../../particle-physics.md) state space, the defining antisymmetry of [fermionic Fock space](../../../../fermionic-fock-space.md). Repeated complete mode labels make the state zero, so they satisfy the same identity trivially.

## ↑ Ancestors (12)

1. [C](../c.md)
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
