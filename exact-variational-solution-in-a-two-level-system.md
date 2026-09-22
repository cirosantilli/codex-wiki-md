# Exact variational solution in a two-level system

↑ **Parent:** [Variational method](variational-method.md)

In a [two-level system](two-level-system.md), let the [Hamiltonian operator](hamiltonian-quantum-mechanics.md) have [matrix](matrix.md) $H=\operatorname{diag}(0,2)$ in the [orthonormal basis](orthonormal-basis.md) $|0\rangle,|1\rangle$. The normalized real trial [quantum states](quantum-state.md) and their [Rayleigh quotient](rayleigh-quotient.md) are

$$
|\psi_\theta\rangle=\cos\theta\,|0\rangle+\sin\theta\,|1\rangle,\qquad E(\theta)=\langle\psi_\theta|H|\psi_\theta\rangle=2\sin^2\theta.
$$

The excited-state [probability amplitude](probability-amplitude.md) is $\sin\theta$, so its [probability](probability.md) is $\sin^2\theta$. Thus $E(\theta)\geq0=E_0$, with equality if and only if the excited-state [probability amplitude](probability-amplitude.md) vanishes: $\theta\in\pi\mathbb Z$. The remaining [quantum state](quantum-state.md) is $|0\rangle$ up to a [global phase](global-phase.md). At $\theta=\pi/4$ the trial [energy](energy-split.md) is $1$; at $\theta=\pi/2$ it is $2$. These are upper bounds on the [ground-state energy](ground-state-energy.md), even though neither is a minimizing trial.

<a id="image-two-level-variational-energy-is-twice-the-excited-level-probability-and-reaches-zero-only-when-the-excited-amplitude-vanishes"></a>
![](two-level-variational-energy.png)

**[Figure 9](#image-two-level-variational-energy-is-twice-the-excited-level-probability-and-reaches-zero-only-when-the-excited-amplitude-vanishes). Two-level variational energy is twice the excited-level probability and reaches zero only when the excited amplitude vanishes**.

The real trial family contains the [ground state](ground-state.md), so it attains the exact minimum despite not covering every complex [quantum state](quantum-state.md). More generally, a family covering all normalized [vectors](vector.md) in a two-dimensional [Hilbert space](hilbert-space-split.md) gives the exact lowest [eigenvalue](eigenvalue.md) of any [Hermitian matrix](hermitian-operator.md) by minimizing its [Rayleigh quotient](rayleigh-quotient.md). For a complex trial $c_0|0\rangle+c_1|1\rangle$ with $|c_0|^2+|c_1|^2=1$, the same calculation gives $E=2|c_1|^2$: a relative [quantum phase](quantum-phase.md) cannot change this diagonal [Hamiltonian](hamiltonian.md) energy. This finite example is the [weighted mean](weighted-arithmetic-mean.md) proof of the [variational method](variational-method.md) with just two [energy eigenstates](energy-eigenstate.md).

**Table of contents**

- [Level repulsion in a two-level Hamiltonian](level-repulsion-in-a-two-level-hamiltonian.md)

## ↑ Ancestors (5)

1. [Variational method](variational-method.md)
2. [Quantum theory](quantum-theory-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Variational method](variational-method.md)
