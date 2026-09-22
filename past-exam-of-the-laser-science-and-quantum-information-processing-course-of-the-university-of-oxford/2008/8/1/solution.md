<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A good atomic [qubit](../../../../qubit.md) needs two reproducible, [orthogonal](../../../../orthogonal-vectors.md) internal states whose populations and relative [quantum phase](../../../../quantum-phase.md) survive for many gate times. Both should be long lived, with weak [spontaneous emission](../../../../spontaneous-emission.md) and little [decoherence](../../../../quantum-decoherence.md) from fluctuating fields or atomic motion. Their transition must nevertheless permit fast, selective, coherent control with little leakage to other states. Reliable initialization and state-selective [quantum measurement](../../../../quantum-measurement-split.md) are also required; [optical pumping](../../../../optical-pumping.md) and fluorescence readout can supply these functions.

For [rubidium-87](../../../../rubidium-87.md), use the two [ground state](../../../../ground-state.md) [hyperfine levels](../../../../hyperfine-level.md) in the $5\,{}^2S_{1/2}$ electronic configuration. The electronic [angular momentum](../../../../angular-momentum.md) is $J=1/2$, and [addition of angular momentum](../../../../addition-of-angular-momentum.md) to the given [nuclear spin](../../../../nuclear-spin.md) $I=3/2$ gives $F=|I-J|,\ldots,I+J=1,2$. A suitable [Rubidium-87 clock qubit](../../../../rubidium-87-clock-qubit.md) is

$$
\boxed{|0\rangle=|5\,{}^2S_{1/2};F=1,m_F=0\rangle,\qquad
|1\rangle=|5\,{}^2S_{1/2};F=2,m_F=0\rangle.}
$$

These are coupled electron-nucleus [angular momentum eigenstates](../../../../angular-momentum-eigenstate.md), rather than two bare nuclear-spin projections. Their [hyperfine structure](../../../../hyperfine-structure.md) supplies a resolvable splitting $\nu_{01}\simeq6.835\,\mathrm{GHz}$. Both belong to the electronic [ground state](../../../../ground-state.md), avoiding a short optical excited-state lifetime. Since the weak-field [Zeeman shift](../../../../zeeman-shift.md) is proportional to $g_Fm_FB$, both have zero linear shift at $B=0$: their [rubidium-87 clock transition](../../../../rubidium-87-clock-transition.md) suppresses first-order magnetic-field [dephasing](../../../../dephasing-channel.md) near zero field. A [quadratic Zeeman shift of a clock transition](../../../../quadratic-zeeman-shift-of-a-clock-transition.md) and differential optical shifts remain. A small stable bias field can define the [quantization axis](../../../../quantization-axis.md) and help resolve unwanted transitions, at the cost of some residual magnetic sensitivity.[Section 3, ground-state hyperfine structure and clock-transition Zeeman shift](../../../../rubidium-87-d-line-data-by-daniel-a-steck.md)

Drive the [magnetic dipole transition](../../../../magnetic-dipole-transition.md) with a resonant [microwave](../../../../microwave.md) field of suitable polarization, here $\Delta m_F=0$, or use two phase-coherent optical fields for a far-detuned [stimulated Raman transition](../../../../stimulated-raman-transition.md) with their frequency difference resonant with $\nu_{01}$. The optical excited state is then only virtually populated, reducing [spontaneous emission](../../../../spontaneous-emission.md). In the rotating frame and [rotating-wave approximation](../../../../rotating-wave-approximation.md), define the drive phase $\phi$ by the effective [Hamiltonian](../../../../hamiltonian.md)

$$
H_{\mathrm{rot}}=\frac{\hbar\Omega}{2}(\cos\phi\,X+\sin\phi\,Y),\qquad
R_\phi(\theta)=e^{-i\theta(\cos\phi\,X+\sin\phi\,Y)/2},\quad\theta=\Omega t.
$$

Here $X,Y,Z$ are the [Pauli matrices](../../../../pauli-matrices.md) on the chosen [qubit](../../../../qubit.md), and $\Omega$ is the [Rabi angular frequency](../../../../rabi-angular-frequency.md). Pulse duration controls the [rotation gate](../../../../rotation-gate.md) angle, while phase selects the axis in the equatorial plane of the [Bloch sphere](../../../../bloch-sphere.md). A $\pi$ pulse exchanges the populations; a $\pi/2$ pulse makes an equal [quantum superposition](../../../../quantum-superposition.md) from either basis state. Controlled [Rabi detuning](../../../../rabi-detuning.md), a differential energy shift, or compositions of these pulses give $z$ rotations. For example, $R_z(\alpha)R_y(\beta)R_z(\gamma)$ realizes any one-[qubit](../../../../qubit.md) [unitary operator](../../../../unitary-operator.md) up to a [global phase](../../../../global-phase.md). Thus the atomic encoding admits arbitrary single-[qubit](../../../../qubit.md) [quantum gates](../../../../quantum-logic-gate.md).

## ↑ Ancestors (12)

1. [1](../1.md)
2. [8](../../8-split.md)
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
