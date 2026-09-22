# Matrix and wave mechanics equivalence

↑ **Parent:** [Matrix mechanics](matrix-mechanics.md)

In 1926, [Erwin Schrödinger](erwin-schrodinger.md) constructed arrays from differential operators and complete orthogonal function systems, showing how their products reproduce the array calculus. His paper connected [wave mechanics](wave-mechanics.md) with [matrix mechanics](matrix-mechanics.md); the translation's sections 2–3 develop the product and commutation rules.[Collected Papers on Wave Mechanics, On the Relation between the Quantum Mechanics of Heisenberg, Born, and Jordan, and that of Schrödinger, pp. 48–51, equations (6)–(10)](on-the-relation-between-the-quantum-mechanics-of-heisenberg-born-and-jordan-and-that-of-schrodinger-by-erwin-schrodinger.md)

The modern proof is a change of [orthonormal basis](orthonormal-basis.md). If $\phi_n(x)$ form a complete [orthonormal basis](orthonormal-basis.md) of the physical [Hilbert space](hilbert-space-split.md), map a [wavefunction](wave-function-split.md) to its coefficients:

$$
c_n=\int\phi_n(x)^*\psi(x)\,dx,\qquad A_{mn}=\int\phi_m(x)^*(A\phi_n)(x)\,dx.
$$

Completeness makes this map [unitary](unitary-connection.md): it preserves the [inner product](inner-product-split.md) and reconstructs $\psi$ from its coefficients. Inserting the complete [orthonormal basis](orthonormal-basis.md) proves the [matrix multiplication](matrix-multiplication.md) rule. The [Schrödinger equation](schrodinger-equation.md) becomes

$$
i\hbar\dot c_m=\sum_nH_{mn}c_n.
$$

For a time-independent [Hamiltonian operator](hamiltonian-quantum-mechanics.md), the [Heisenberg picture](heisenberg-picture.md) transfers the same evolution to the [observables](observable.md), preserving measurement predictions. [Unitary equivalence](unitary-equivalence.md) requires matching [operator domains](operator-domain.md) as well as formal entries. A finite selection of [eigenfunctions](eigenfunction.md) gives a compression, not an exact replacement of the full [Hilbert space](hilbert-space-split.md); a [continuous spectrum](continuous-spectrum.md) needs its spectral integrals. This equivalence concerns representations of specified operators, and does not remove the ordering question when quantizing an arbitrary classical expression, as [Weyl ordering](weyl-ordering.md) illustrates.

## ↑ Ancestors (6)

1. [Matrix mechanics](matrix-mechanics.md)
2. [Operator formalism](operator-formalism.md)
3. [Quantum mechanics](quantum-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
