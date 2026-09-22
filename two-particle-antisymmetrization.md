# Two-particle antisymmetrization

↑ **Parent:** [Pauli exclusion principle](pauli-exclusion-principle.md)

The [particle exchange operator](particle-exchange-operator.md) $P_{12}$ swaps the complete particle slots, including [spin](spin.md). Its antisymmetric [projector](projection-linear-algebra.md) is $A_{12}=(I-P_{12})/2$. For [orthonormal](orthonormal-set.md) [one-particle states](one-particle-state.md) $u,v$, the normalized [multiparticle quantum state](multiparticle-quantum-state.md) is

$$
|u\wedge v\rangle=\frac{|u\rangle\otimes|v\rangle-|v\rangle\otimes|u\rangle}{\sqrt2}.
$$

But attempting the same construction with $v=u$ gives the zero vector:

$$
A_{12}(|u\rangle\otimes|u\rangle)=\frac{|u\rangle\otimes|u\rangle-|u\rangle\otimes|u\rangle}{2}=0.
$$

The zero vector cannot be normalized to a [quantum state](quantum-state.md). This is exclusion as cancellation of [probability amplitudes](probability-amplitude.md), rather than a repulsive force. More generally, for normalized $u,v$ the squared [norm](norm.md) of the numerator divided by $\sqrt2$ is $1-|\langle u|v\rangle|^2$; the expression has unit [norm](norm.md) only when $u,v$ are [orthogonal](orthogonal-vectors.md). An overall [quantum phase](quantum-phase.md) difference between $u,v$ describes the same [one-particle state](one-particle-state.md) and also gives zero. Pauli explicitly connects exclusion with a vanishing antisymmetric [wavefunction](wave-function-split.md).[p. 31, antisymmetric functions with repeated states](exclusion-principle-and-quantum-mechanics-by-wolfgang-pauli.md)

<a id="image-antisymmetrization-removes-equal-state-pairs-and-pairs-the-twelve-remaining-ordered-products-into-six-fermionic-basis-states"></a>
![](pauli-antisymmetric-state-pairs.png)

**[Figure 3](#image-antisymmetrization-removes-equal-state-pairs-and-pairs-the-twelve-remaining-ordered-products-into-six-fermionic-basis-states). Antisymmetrization removes equal-state pairs and pairs the twelve remaining ordered products into six fermionic basis states**.

**Table of contents**

- [Slater determinant](slater-determinant.md)
  - [Slater-Condon rules](slater-condon-rules.md)

## ↑ Ancestors (10)

1. [Pauli exclusion principle](pauli-exclusion-principle.md)
2. [Fermion](fermion.md)
3. [Indistinguishable particles](indistinguishable-particles.md)
4. [Particle exchange operator](particle-exchange-operator.md)
5. [Multiparticle quantum state](multiparticle-quantum-state.md)
6. [Tensor product of quantum systems](tensor-product-of-quantum-systems-split.md)
7. [Quantum mechanics](quantum-mechanics-split.md)
8. [Branches of physics](branches-of-physics.md)
9. [Physics](physics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Counting spin orbitals in an electron shell](counting-spin-orbitals-in-an-electron-shell.md)
- [Slater determinant](slater-determinant.md)
- [Spectroscopic origin of the Pauli exclusion principle](spectroscopic-origin-of-the-pauli-exclusion-principle.md)
