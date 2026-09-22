<h1 id="7/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For [teleportation with an ambiguous Bell-state phase label](../../../../../teleportation-with-an-ambiguous-bell-state-phase-label.md), write $\rho=|\psi\rangle\langle\psi|$. The [Bell-basis measurement](../../../../../bell-basis-measurement.md) outcomes $\phi^+$ and $\phi^-$ each occur with [probability](../../../../../probability.md) $1/4$. In either case a correct guess gives Bob $\rho$, while the wrong guess differs by the [Pauli Z gate](../../../../../pauli-z-gate.md) and gives $Z\rho Z$. The other two [Bell states](../../../../../bell-state-split.md) are identified correctly. Since Alice guesses each ambiguous label with [probability](../../../../../probability.md) $1/2$, the overall wrong-correction [probability](../../../../../probability.md) is $(1/2)(1/2)=1/4$. Averaging over the actual [quantum measurement](../../../../../quantum-measurement-split.md) outcome and her guess gives the [phase-flip channel](../../../../../phase-flip-channel.md)

$$
\boxed{\rho_{\rm out}=\mathcal E(\rho)=\frac34\rho+\frac14Z\rho Z
=\begin{pmatrix}|\alpha|^2&\alpha\beta^*/2\\\alpha^*\beta/2&|\beta|^2\end{pmatrix}.}
$$

Conditional only on an ambiguous analyzer result, the output is $(\rho+Z\rho Z)/2$; that conditional channel has weight $1/2$ in the displayed unconditional result. There is no rejection of those rounds.

Use the [teleportation fidelity](../../../../../teleportation-fidelity.md) for a [pure state](../../../../../pure-state.md) target, namely the [squared quantum fidelity](../../../../../squared-quantum-fidelity.md)

$$
F_\psi=\langle\psi|\rho_{\rm out}|\psi\rangle.
$$

This compares the input with the resulting [mixed state](../../../../../mixed-state.md); averaging state vectors before forming a [density matrix](../../../../../density-matrix-split.md) would give a different, incorrect answer. Direct substitution gives

$$
\boxed{F_\psi=\frac34+\frac14|\langle\psi|Z|\psi\rangle|^2
=\frac34+\frac14(|\alpha|^2-|\beta|^2)^2
=1-|\alpha|^2|\beta|^2.}
$$

Thus **the maximum is $1$**, attained by $|0\rangle$ and $|1\rangle$ up to a [global phase](../../../../../global-phase.md), because these are [eigenstates](../../../../../eigenstate.md) of the [Pauli Z gate](../../../../../pauli-z-gate.md). **The minimum is $3/4$**, attained by every equal-weight [quantum superposition](../../../../../quantum-superposition.md)

$$
|\psi\rangle=\frac{|0\rangle+e^{i\theta}|1\rangle}{\sqrt2},\qquad \theta\in\mathbb R,
$$

on the equator of the [Bloch sphere](../../../../../bloch-sphere.md). The [unsquared quantum fidelity](../../../../../fidelity-of-quantum-states.md) is $\sqrt{F_\psi}$ if that alternative convention is used. No average over different input [quantum states](../../../../../quantum-state.md) is needed for the requested state-dependent answer.

## ↑ Ancestors (13)

1. [2](../2.md)
2. [7](../../7.md)
3. [7 and 8](../../../7-and-8-split.md)
4. [2005](../../../split.md)
5. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../../split.md)
6. [Laser science and quantum information processing course of the University of Oxford](../../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
7. [Year 4 of the physics course of the University of Oxford](../../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
