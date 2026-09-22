# Pure-state trace distance and fidelity identity

↑ **Parent:** [Fidelity of quantum states](fidelity-of-quantum-states.md)

For normalized [pure states](pure-state.md) $\rho=|\psi\rangle\langle\psi|$ and $\sigma=|\varphi\rangle\langle\varphi|$, the [trace distance](trace-distance.md) and [quantum fidelity](fidelity-of-quantum-states.md) satisfy

$$
D(\rho,\sigma)=\frac12\|\rho-\sigma\|_1=\sqrt{1-|\langle\psi|\varphi\rangle|^2}=\sqrt{1-F^2}=\sqrt{1-F_{\mathrm{sq}}}.
$$

The last two expressions distinguish the [unsquared quantum fidelity](fidelity-of-quantum-states.md) from the [squared quantum fidelity](squared-quantum-fidelity.md). Identical [pure states](pure-state.md) give $D=0$, and [orthogonal](orthogonal-vectors.md) [pure states](pure-state.md) give $D=1$. The equality need not hold for [mixed states](mixed-state.md); the [Fuchs-van de Graaf inequalities](fuchs-van-de-graaf-inequalities.md) give bounds in that case.

Brief proof: for two distinct [pure states](pure-state.md), their two-dimensional span contains the nonzero part of $\rho-\sigma$. This restriction has [trace](matrix-trace.md) zero and [determinant](determinant.md) $-(1-F^2)$, hence [eigenvalues](eigenvalue.md) $\pm\sqrt{1-F^2}$. Its [trace norm](trace-norm.md) is twice the positive [eigenvalue](eigenvalue.md), giving [trace distance](trace-distance.md) $D=\sqrt{1-F^2}$. For identical [pure states](pure-state.md), $\rho-\sigma=0$ directly.

**Table of contents**

- [Qubit fidelity along a Bloch meridian](qubit-fidelity-along-a-bloch-meridian.md)

## ↑ Ancestors (6)

1. [Fidelity of quantum states](fidelity-of-quantum-states.md)
2. [Quantum information theory](quantum-information-theory-split.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Cloning failure bound from trace-distance contraction](cloning-failure-bound-from-trace-distance-contraction.md)
- [Fidelity of commuting mixed states](fidelity-of-commuting-mixed-states.md)
- [Fidelity of quantum states](fidelity-of-quantum-states.md)
- [Fuchs-van de Graaf inequalities](fuchs-van-de-graaf-inequalities.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-54/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-58/4/ii/solution.md)
- [Qubit fidelity along a Bloch meridian](qubit-fidelity-along-a-bloch-meridian.md)
