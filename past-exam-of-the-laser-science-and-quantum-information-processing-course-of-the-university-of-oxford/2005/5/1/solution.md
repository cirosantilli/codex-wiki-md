<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Treat $|a\rangle=|0\rangle$ and $|b\rangle=|1\rangle$ as an isolated [ground-state hyperfine qubit](../../../../ground-state-hyperfine-qubit.md). Their transition angular frequency is $\omega_0=2\pi\times320.7\,\mathrm{MHz}$. The radiofrequency [magnetic field](../../../../magnetic-field-split.md) couples them through an allowed [magnetic dipole transition](../../../../magnetic-dipole-transition.md). After choosing its phase reference, take the two-level laboratory [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md) to be

$$
H(t)=-\frac{\hbar\omega_0}{2}Z+\hbar\Omega\cos(\omega t)X,
$$

where $X,Z$ are [Pauli operators](../../../../pauli-operator.md). Here $\Omega$ is defined by the on-resonance rotating-frame off-diagonal matrix element $\hbar\Omega/2$.

Use a [quantum rotating frame](../../../../quantum-rotating-frame.md) and the [rotating-wave approximation](../../../../rotating-wave-approximation.md), valid for $\Omega,|\delta|\ll\omega_0$, with [Rabi detuning](../../../../rabi-detuning.md) $\delta=\omega_0-\omega$. Ignoring off-resonant coupling to other levels gives

$$
H_R=\frac\hbar2(\Omega X-\delta Z).
$$

At resonance $\delta=0$, the [unitary time evolution](../../../../unitary-time-evolution.md) is

$$
U_R(t)=\cos\frac{\Omega t}{2}I-i\sin\frac{\Omega t}{2}X,
\qquad
|\psi_R(t)\rangle=\cos\frac{\Omega t}{2}|a\rangle-i\sin\frac{\Omega t}{2}|b\rangle.
$$

Thus the [Born rule](../../../../born-rule.md) gives coherent [Rabi oscillations](../../../../rabi-cycle.md),

$$
\boxed{P_a(t)=\cos^2\frac{\Omega t}{2},\qquad P_b(t)=\sin^2\frac{\Omega t}{2}.}
$$

The stated amplitudes are in the rotating frame; the laboratory carrier phases are tracked by the drive reference.

These logical states are orthogonal, individually resolvable [hyperfine levels](../../../../hyperfine-level.md) in the same electronic [ground state](../../../../ground-state.md). They avoid fast optical decay, can be coherently coupled by radiofrequency control, and have a state-selective optical readout through $|c\rangle$. The excited level $|c\rangle$ is useful for [fluorescence](../../../../fluorescence-split.md) detection rather than for the storage superposition in this model. Long lifetimes alone do not guarantee a useful qubit: control isolation and adequate [quantum coherence](../../../../quantum-coherence-in-a-specified-basis.md) are also required.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [5](../../5-split.md)
3. [2005](../../split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
