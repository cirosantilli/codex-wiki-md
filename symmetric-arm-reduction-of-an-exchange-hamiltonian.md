# Symmetric-arm reduction of an exchange Hamiltonian

↑ **Parent:** [XY exchange interaction](xy-exchange-interaction.md)

Consider $q$ identical length-$n$ arms joined to one hub, with [XY exchange interactions](xy-exchange-interaction.md) of strength $J_0/\sqrt q$ from the hub to each first site and strength $J_k$ between sites $k,k+1$ on each arm. Let $|s_0\rangle$ be the hub excitation and $|s_k\rangle=q^{-1/2}\sum_{a=1}^q|a,k\rangle$. This [orthonormal](orthonormal-set.md) symmetric [single-excitation subspace](single-excitation-subspace.md) is invariant, and its restricted [Hamiltonian operator](hamiltonian-quantum-mechanics.md) is

$$
H|s_0\rangle=J_0|s_1\rangle,\qquad H|s_k\rangle=J_{k-1}|s_{k-1}\rangle+J_k|s_{k+1}\rangle,
$$

with endpoint terms omitted. At the first link the $q$ hub contributions add to $J_0$; all other links act identically on the arms. Thus the [linear isometry](linear-isometry-of-hilbert-spaces.md) $F|k\rangle=|s_k\rangle$ intertwines $H$ with the path [Hamiltonian operator](hamiltonian-quantum-mechanics.md) $H_T=\sum_{k=0}^{n-1}J_k(|k\rangle\langle k+1|+|k+1\rangle\langle k|)$: $HF=FH_T$. Expanding the [matrix exponential](matrix-exponential.md) gives $e^{-iHt}F=Fe^{-iH_Tt}$. [Perfect quantum state transfer](perfect-quantum-state-transfer.md) from zero to $n$ on the path therefore produces an equal excitation superposition at the $q$ arm tips. Since all other [qubits](qubit.md) are zero, the tip state is a pure [W state](w-state.md), up to the transfer's common phase.

## ↑ Ancestors (9)

1. [XY exchange interaction](xy-exchange-interaction.md)
2. [Single-excitation subspace](single-excitation-subspace.md)
3. [Heisenberg model](heisenberg-model.md)
4. [Spin](spin.md)
5. [Angular momentum operator](angular-momentum-operator.md)
6. [Quantum mechanics](quantum-mechanics-split.md)
7. [Branches of physics](branches-of-physics.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-57/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-57/3/d/solution.md)
- [W state](w-state.md)
