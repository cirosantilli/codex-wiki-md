<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the same protocol: distribute one resource photon through $\mathcal C$, and send Alice's two classical bits error-free in the $D,A$ alphabet from part a. At $p=1/2$ the distributed resource is

$$
\rho_{23}=\tfrac12|\Phi^+\rangle\langle\Phi^+|
+\tfrac12|\Psi^+\rangle\langle\Psi^+|,
\qquad |\Psi^+\rangle=(I\otimes X)|\Phi^+\rangle.
$$

For the second component Bob has an extra $X$ before his conditional correction. Conjugation by that correction changes $X$ at most by a sign, which cancels in the [density operator](../../../../density-matrix-split.md). This [bit-flipped Bell resource teleportation](../../../../bit-flipped-bell-resource-teleportation.md) therefore induces the bit-flip map,

$$
\rho_{\rm tel}=\tfrac12|\psi\rangle\langle\psi|+
\tfrac12X|\psi\rangle\langle\psi|X.
$$

Using the squared pure-target [quantum fidelity](../../../../fidelity-of-quantum-states.md) convention,

$$
\boxed{F_\psi=\langle\psi|\rho_{\rm tel}|\psi\rangle
=\frac12\left(1+|\langle\psi|X|\psi\rangle|^2\right)
=\frac12\left(1+4[\operatorname{Re}(\alpha^*\beta)]^2\right).}
$$

The maximum is $1$ precisely for the [Pauli X eigenstates](../../../../pauli-x-eigenstate.md) $D,A$. The minimum is $1/2$ whenever $\operatorname{Re}(\alpha^*\beta)=0$, the great circle with zero $x$ component of the [Bloch vector](../../../../bloch-vector.md), including $H,V$ and both circular [polarizations](../../../../polarization-waves.md). Uniform averaging over pure [qubits](../../../../qubit.md) gives $\overline F=2/3$.

The resource-distribution and classical-encoding assumptions are essential. If a perfect shared pair had already been supplied independently and this channel were used only for the robustly encoded classical bits, teleportation would remain perfect even at $p=1/2$. Conversely, unprotected $H,V$ transmission of Alice's correction bits would add classical errors. The stated expression applies to the resource sent through the given channel and the error-free classical encoding explicitly available in part a.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [7](../../7.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
