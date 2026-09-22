<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

[Quantum error correction](../../../../quantum-error-correction-split.md) encodes a [logical qubit](../../../../logical-qubit.md) redundantly, obtains an [error syndrome](../../../../error-syndrome.md) without measuring its unknown logical amplitudes, and applies a recovery that reverses the specified errors. A [decoherence-free subspace](../../../../decoherence-free-subspace.md) instead uses a symmetry of a specified noise model: each noise operator acts as a scalar on the entire encoded space, so no syndrome-dependent recovery is required. This is passive protection and can also be viewed as a special case of [quantum error correction](../../../../quantum-error-correction-split.md).

For the [two-spin decoherence-free encoding](../../../../two-spin-decoherence-free-encoding.md), choose

$$
|0_L\rangle=|01\rangle,\qquad |1_L\rangle=|10\rangle,\qquad
|\psi_L\rangle=\alpha|01\rangle+\beta|10\rangle,
\qquad |\alpha|^2+|\beta|^2=1.
$$

Simultaneous [Pauli Z gates](../../../../pauli-z-gate.md) give

$$
(Z\otimes Z)|01\rangle=-|01\rangle,\qquad
(Z\otimes Z)|10\rangle=-|10\rangle,
$$

so

$$
\boxed{(Z\otimes Z)|\psi_L\rangle=-|\psi_L\rangle.}
$$

Both logical components acquire the same [global phase](../../../../global-phase.md); their [relative phase](../../../../relative-quantum-phase.md) and amplitudes survive. The [density matrix](../../../../density-matrix-split.md) is exactly unchanged, so even an unknown random choice between applying $I$ and $Z\otimes Z$ causes no logical [dephasing](../../../../dephasing-channel.md).

More strongly, the encoding protects against arbitrary [collective dephasing](../../../../collective-dephasing.md):

$$
[R_z(\phi)\otimes R_z(\phi)]|\psi_L\rangle
=e^{-i\phi(Z\otimes I+I\otimes Z)/2}|\psi_L\rangle
=|\psi_L\rangle,
$$

because both basis states have total $Z$ [eigenvalue](../../../../eigenvalue.md) zero. At $\phi=\pi$, $R_z(\pi)\otimes R_z(\pi)=-Z\otimes Z$, consistent with the previous overall phase. The protection relies on correlated noise: independent $Z$ rotations generally change the logical relative phase, and this two-spin code does not protect a whole [logical qubit](../../../../logical-qubit.md) against arbitrary collective rotations about all three axes or against arbitrary single-spin errors.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [6](../../6-split.md)
3. [2008](../../split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
