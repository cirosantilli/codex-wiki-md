# Observable matrices in an energy basis

↑ **Parent:** [Matrix mechanics](matrix-mechanics.md)

Choose normalized [energy eigenstates](energy-eigenstate.md) $|n\rangle$ of a time-independent [Hamiltonian operator](hamiltonian-quantum-mechanics.md), with $H|n\rangle=E_n|n\rangle$, and assume first that they form a complete [orthonormal basis](orthonormal-basis.md). For a [pure state](pure-state.md) and an [observable](observable.md) $A$,

$$
|\psi\rangle=\sum_n c_n|n\rangle,\qquad A_{mn}=\langle m|A|n\rangle,\qquad (A\psi)_m=\sum_n A_{mn}c_n,\qquad \langle A\rangle=\sum_{m,n}c_m^*A_{mn}c_n.
$$

The column index $n$ labels the input [basis vector](basis-vector.md), and row $m$ labels the output component. [Self-adjointness](self-adjoint-operator.md) gives $A_{nm}=A_{mn}^*$, so a finite example is a [Hermitian matrix](hermitian-operator.md). A [matrix element](matrix-element.md) can be negative or complex; by itself it is not generally a [probability](probability.md). The [Born rule](born-rule.md) assigns measurement [probabilities](probability.md) using the [eigenstates](eigenstate.md) of $A$, which need not be [energy eigenstates](energy-eigenstate.md). For an unbounded [observable](observable.md), these expressions require a suitable [operator domain](operator-domain.md); a system with [continuous spectrum](continuous-spectrum.md) also needs the corresponding spectral integrals.

**Table of contents**

- [Transition frequencies and matrix multiplication](transition-frequencies-and-matrix-multiplication.md)
- [Three-level observable and missing spectral line](three-level-observable-and-missing-spectral-line.md)

## ↑ Ancestors (6)

1. [Matrix mechanics](matrix-mechanics.md)
2. [Operator formalism](operator-formalism.md)
3. [Quantum mechanics](quantum-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
