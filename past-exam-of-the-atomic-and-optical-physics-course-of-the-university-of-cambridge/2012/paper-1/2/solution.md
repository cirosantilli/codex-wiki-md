<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Fix the [qubit polarization](../../../../qubit-polarization.md) convention by $\rho=(I+\vec P\cdot\vec\sigma)/2$, where the [Pauli matrices](../../../../pauli-matrices.md) are ordered in the basis $(|1\rangle,|2\rangle)$ and $\sigma_z=|1\rangle\langle1|-|2\rangle\langle2|$. Thus the [ground state](../../../../ground-state.md) is the north pole of the [Bloch sphere](../../../../bloch-sphere.md). In a [rotating frame](../../../../rotating-reference-frame.md) and within the [rotating-wave approximation](../../../../rotating-wave-approximation.md), choose the drive phase and detuning sign so that

$$
H_R=\frac\hbar2(\Omega\sigma_x+\Delta\sigma_z),\qquad
\dot{\vec P}=(\Omega,0,\Delta)\times\vec P.
$$

For example, with this ground-state convention one may take $\Delta=\omega_L-\omega_0$ and choose the transverse coupling positive. The [Bloch vector](../../../../bloch-vector.md) precesses around the effective field $(\Omega,0,\Delta)$ at [angular frequency](../../../../angular-frequency.md) $\Omega_R=\sqrt{\Omega^2+\Delta^2}$, tracing a circle at fixed projection on that axis. Its length is conserved under coherent [unitary time evolution](../../../../unitary-time-evolution.md). On resonance the axis is transverse and the [Rabi oscillation](../../../../rabi-cycle.md) can fully invert an initially ground-state atom. Away from resonance the axis tilts, and

$$
P_{1\to2}(t)=\frac{\Omega^2}{\Omega^2+\Delta^2}\sin^2\!\left(\frac{\Omega_Rt}{2}\right).
$$

There is no relaxation towards an equilibrium [Bloch vector](../../../../bloch-vector.md) in this ideal model. An inhomogeneous ensemble can nevertheless lose its _averaged_ [qubit polarization](../../../../qubit-polarization.md) through [dephasing](../../../../dephasing-channel.md) even without [spontaneous emission](../../../../spontaneous-emission.md); the circle description assumes a common drive and detuning.

For $|a|^2+|b|^2=1$, the stated [quantum state](../../../../quantum-state.md) gives

$$
\rho=|\Psi\rangle\langle\Psi|=
\begin{pmatrix}|a|^2&ab^*\\a^*b&|b|^2\end{pmatrix},\qquad
\vec P=(2\operatorname{Re}(a^*b),\,2\operatorname{Im}(a^*b),\,|a|^2-|b|^2).
$$

The diagonal elements are the two state populations. The off-diagonal elements are [quantum coherences](../../../../quantum-coherence-in-a-specified-basis.md): they retain the [relative quantum phase](../../../../relative-quantum-phase.md) and determine [interference](../../../../interference-wave-propagation.md) under a subsequent pulse. **This is a [pure state](../../../../pure-state.md)**, even if both populations are nonzero: $\rho^2=\rho$, $\operatorname{Tr}\rho^2=1$, and $|\vec P|=1$. A [mixed state](../../../../mixed-state.md) averages projectors over preparation [probabilities](../../../../probability.md) and generally has $\operatorname{Tr}\rho^2<1$. Equal populations alone do not distinguish an equal coherent [superposition](../../../../superposition-principle.md) from an unpolarized mixture.

For use in all three cases, multiplication of the gates gives the [Hadamard-phase-Hadamard qubit rotation](../../../../hadamard-phase-hadamard-qubit-rotation.md)

$$
U=HP_\alpha H=\frac12\begin{pmatrix}1+e^{i\alpha}&1-e^{i\alpha}\\1-e^{i\alpha}&1+e^{i\alpha}\end{pmatrix}
=e^{i\alpha/2}\exp(-i\alpha\sigma_x/2).
$$

The [global phase](../../../../global-phase.md) cancels in $\rho'=U\rho U^\dagger$. Thus the [Bloch vector](../../../../bloch-vector.md) map is

$$
\boxed{(P_x,P_y,P_z)\longmapsto(P_x,\,P_y\cos\alpha-P_z\sin\alpha,\,P_y\sin\alpha+P_z\cos\alpha).}
$$

The final unlabelled [Ramsey spectroscopy](../../../../ramsey-spectroscopy.md) comparison applies to the three cases as follows. In an [atomic clock](../../../../atomic-clock.md), an initial coherent pulse prepares a [superposition](../../../../superposition-principle.md), a free interval $T$ accumulates a [relative quantum phase](../../../../relative-quantum-phase.md) proportional to detuning times $T$, and a final coherent pulse converts that phase to a population. Here $\alpha$ plays the role of that accumulated phase, with sign and fringe offset set by pulse conventions. In (a), the first [Hadamard gate](../../../../hadamard-gate.md) creates the needed [superposition](../../../../superposition-principle.md) and the final gate reveals full-contrast [Ramsey interferometry](../../../../ramsey-interferometry.md). In (b), the first [Hadamard gate](../../../../hadamard-gate.md) instead puts the state in $|1\rangle$, so the intervening [phase gate](../../../../phase-gate.md) has no [relative quantum phase](../../../../relative-quantum-phase.md) to imprint: the output is independent of $\alpha$. In (c), the unpolarized [density matrix](../../../../density-matrix-split.md) remains unchanged under every gate, so the ensemble has no [Ramsey interferometry](../../../../ramsey-interferometry.md) contrast. A coherent [unitary gate](../../../../quantum-logic-gate.md) alone cannot initialize a maximally mixed ensemble into a pure clock state.

The [Ramsey interferometry](../../../../ramsey-interferometry.md) analogy concerns preparation, phase accumulation, and readout; **a [Hadamard gate](../../../../hadamard-gate.md) is not literally a transverse $\pi/2$ [rotation](../../../../rotation-mathematics.md) on every input**. In this basis $H=R_y(\pi/2)\sigma_z$, and its [Bloch sphere](../../../../bloch-sphere.md) action is a $\pi$ [rotation](../../../../rotation-mathematics.md) about $(\hat x+\hat z)/\sqrt2$, up to a [global phase](../../../../global-phase.md). The phase conventions of physical [Ramsey spectroscopy](../../../../ramsey-spectroscopy.md) pulses must be specified to compare their outputs for arbitrary initial states.

## ↑ Ancestors (13)

1. [2](../2.md)
2. [Paper 1](../../paper-1-split.md)
3. [2012](../../split.md)
4. [Past exam of the atomic and Optical Physics course of the University of Cambridge](../../../split.md)
5. [Atomic and Optical Physics course of the University of Cambridge](../../../../atomic-and-optical-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
