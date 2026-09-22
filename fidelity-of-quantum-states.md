# Fidelity of quantum states

↑ **Parent:** [Quantum information theory](quantum-information-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fidelity_of_quantum_states)

For [density operators](density-matrix-split.md) $\rho,\sigma$ on the same finite-dimensional [Hilbert space](hilbert-space-split.md), quantum fidelity measures how close their [quantum states](quantum-state.md) are. This article uses the unsquared convention:

$$
F(\rho,\sigma)=\operatorname{Tr}\sqrt{\sqrt\rho\,\sigma\sqrt\rho}=\|\sqrt\rho\sqrt\sigma\|_1,\qquad 0\leq F(\rho,\sigma)\leq1.
$$

Each square root is the [positive square root of an operator](positive-square-root-of-an-operator.md), and $\|\cdot\|_1$ is the [trace norm](trace-norm.md). [Quantum fidelity](fidelity-of-quantum-states.md) is symmetric in its inputs; it is one exactly when $\rho=\sigma$, and zero exactly when $\rho\sigma=0$, meaning that the [support of a positive operator](support-of-a-positive-operator.md) for one state is [orthogonal](orthogonal-vectors.md) to that for the other. Larger [quantum fidelity](fidelity-of-quantum-states.md) means greater similarity. The separate [squared quantum fidelity](squared-quantum-fidelity.md) is $F_{\mathrm{sq}}=F^2$. [Watrous, The Theory of Quantum Information, Definition 3.11 and Proposition 3.12](https://jhwatrous.github.io/TQI.3.pdf#page=16)

For two normalized [pure states](pure-state.md), [quantum fidelity](fidelity-of-quantum-states.md) is the magnitude of their [inner product](inner-product-split.md), $F=|\langle\psi|\varphi\rangle|$. Thus $|0\rangle$ compared with itself has $F=1$, while $|0\rangle$ and $|1\rangle$ have $F=0$. For $|+\rangle=(|0\rangle+|1\rangle)/\sqrt2$, comparison with $|0\rangle$ gives $F=1/\sqrt2$, $F_{\mathrm{sq}}=1/2$, and [trace distance](trace-distance.md) $D=1/\sqrt2$ by the [pure-state trace distance and fidelity identity](pure-state-trace-distance-and-fidelity-identity.md).

Why compare [density operators](density-matrix-split.md) rather than their entries? A change of coordinates should not make the same physical preparations look more or less alike. [Unitary invariance of trace distance and fidelity](unitary-invariance-of-trace-distance-and-fidelity.md) makes [quantum fidelity](fidelity-of-quantum-states.md) independent of a common basis choice. Multiplying a [pure state](pure-state.md) vector by a [global phase](global-phase.md) leaves its [density operator](density-matrix-split.md) unchanged, so its [quantum fidelity](fidelity-of-quantum-states.md) with the original state is one. These features make [quantum fidelity](fidelity-of-quantum-states.md) useful for checking whether [quantum channels](quantum-channel.md), state preparations, and [Schumacher compression](schumacher-compression.md) preserve a target [quantum state](quantum-state.md).

The connection to [Uhlmann's theorem](uhlmann-s-theorem.md) supplies another beautiful interpretation: [quantum fidelity](fidelity-of-quantum-states.md) is the largest absolute [inner product](inner-product-split.md) between pure vectors obtained from a [purification of a density operator](purification-of-a-density-operator.md) for each state, using a sufficiently large common reference space. Uhlmann's 1976 paper extended transition probability to algebraic states, including those of a [C-star algebra](c-star-algebra.md); for [density operators](density-matrix-split.md) its transition probability corresponds to our [squared quantum fidelity](squared-quantum-fidelity.md). The [measurement characterization of quantum fidelity](measurement-characterization-of-quantum-fidelity.md) gives a complementary description directly in terms of observable outcome statistics. [Uhlmann, The transition probability in the state space of a star-algebra, Reports on Mathematical Physics 9, 273–279, 1976](https://www.physik.uni-leipzig.de/~uhlmann/PDF/Uh76a.pdf)

**Table of contents**

- [Squared quantum fidelity](squared-quantum-fidelity.md)
- [Pure-state trace distance and fidelity identity](pure-state-trace-distance-and-fidelity-identity.md)
  - [Qubit fidelity along a Bloch meridian](qubit-fidelity-along-a-bloch-meridian.md)
- [Unitary invariance of trace distance and fidelity](unitary-invariance-of-trace-distance-and-fidelity.md)
- [Fidelity of commuting mixed states](fidelity-of-commuting-mixed-states.md)
- [Measurement characterization of quantum fidelity](measurement-characterization-of-quantum-fidelity.md)
- [Fuchs-van de Graaf inequalities](fuchs-van-de-graaf-inequalities.md)
- [Joint concavity of quantum fidelity](joint-concavity-of-quantum-fidelity.md)
- [Monotonicity of quantum fidelity under partial trace](monotonicity-of-quantum-fidelity-under-partial-trace.md)
- [Pure-state gentle measurement bound](pure-state-gentle-measurement-bound.md)

## ↑ Ancestors (5)

1. [Quantum information theory](quantum-information-theory-split.md)
2. [Quantum theory](quantum-theory-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Squared quantum fidelity](squared-quantum-fidelity.md)
