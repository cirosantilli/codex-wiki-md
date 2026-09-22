# Finite-pulse Ramsey transition probability

↑ **Parent:** [Ramsey separated oscillatory fields experiment](ramsey-separated-oscillatory-fields-experiment.md)

Use the [Driven two-level Rabi model](driven-two-level-rabi-model.md) in the ordered [basis](basis.md) $(|e\rangle,|g\rangle)$, with [Pauli matrices](pauli-matrices.md) satisfying $\sigma_z=\operatorname{diag}(1,-1)$. Let the [Rabi detuning](rabi-detuning.md) be $\delta=\omega_0-\omega=2\pi(\nu_0-\nu)$, in [angular frequency](angular-frequency.md), while $\nu_0$ and $\nu$ are ordinary [frequencies](frequency.md) in [hertz](hertz.md). Assume two identical square pulses, equal drive [oscillation phases](phase-waves.md), constant positive [Rabi angular frequency](rabi-angular-frequency.md) $\Omega$, constant $\delta$ during pulses and flight, and no [quantum decoherence](quantum-decoherence.md) or loss. The [rotating-wave approximation](rotating-wave-approximation.md) and isolation of the chosen [two-level system](two-level-system.md) are required, just as for the [Driven two-level Rabi model](driven-two-level-rabi-model.md). Free flight means no transverse drive; the reference [oscillator](oscillator.md) continues running.

The pulse and free-flight [Hamiltonian operators](hamiltonian-quantum-mechanics.md) in the [rotating frame](rotating-reference-frame.md) are

$$
H_p=\frac{\hbar}{2}(\delta\sigma_z+\Omega\sigma_x),\qquad
H_f=\frac{\hbar\delta}{2}\sigma_z,\qquad
q=\sqrt{\Omega^2+\delta^2},\quad c_p=\cos(q\tau/2),\quad s_p=\sin(q\tau/2).
$$

The [Pauli matrix multiplication law](pauli-matrix-multiplication-law.md) gives $(\delta\sigma_z+\Omega\sigma_x)^2=q^2I$. Thus the exact [special unitary group](special-unitary-group.md) $\mathrm{SU}(2)$ pulse [matrix](matrix.md) for this effective [Hamiltonian operator](hamiltonian-quantum-mechanics.md), and the flight [matrix](matrix.md), are

$$
U_p=\begin{pmatrix}
c_p-i(\delta/q)s_p&-i(\Omega/q)s_p\\
-i(\Omega/q)s_p&c_p+i(\delta/q)s_p
\end{pmatrix},\qquad
U_f=\begin{pmatrix}e^{-i\delta T/2}&0\\0&e^{i\delta T/2}\end{pmatrix}.
$$

The sequence is $U_pU_fU_p$. Starting in $|g\rangle$, [matrix multiplication](matrix-multiplication.md) and the [Born rule](born-rule.md) give

$$
\boxed{P_{g\to e}=4\frac{\Omega^2}{q^2}s_p^2
\left[c_p\cos\frac{\delta T}{2}-\frac{\delta}{q}s_p\sin\frac{\delta T}{2}\right]^2.}
$$

This retains the tilted rotation axis and [quantum phase](quantum-phase.md) accumulated during each finite pulse. At resonance it gives $P_{g\to e}(0)=\sin^2(\Omega\tau)$; with no flight it reduces to the single square-pulse response for duration $2\tau$. Both checks would fail if arbitrary ideal $\pi/2$ rotations were silently substituted at nonzero [Rabi detuning](rabi-detuning.md).

For resonant pulse area $\Omega\tau=\pi/2$, $|\delta|/\Omega\ll1$ and $\tau\ll T$, the central fringe approaches

$$
P_{g\to e}\simeq\cos^2(\delta T/2)=\cos^2[\pi(\nu-\nu_0)T].
$$

Its half-height points are $|\nu-\nu_0|=1/(4T)$, so the central peak's [full width at half maximum](full-width-at-half-maximum.md) is $1/(2T)$ in [hertz](hertz.md), or $\pi/T$ in [angular frequency](angular-frequency.md). This width assumes an effectively flat pulse envelope across that central peak, one flight time and unit contrast; it is neither a universal finite-pulse width nor a [frequency](frequency.md) uncertainty. Longer flight lets a smaller [frequency](frequency.md) difference accumulate the same observable [quantum phase](quantum-phase.md).

The two pulses here have the same sign and the plotted outcome is transfer to $|e\rangle$. The earlier [Ramsey interferometry](ramsey-interferometry.md) example uses an inverse analysis pulse and reports return to its initial label. Specifying the measured outcome and pulse [oscillation phases](phase-waves.md) reconciles the two conventions. In a beam the lengths and [speed](speed.md) determine $\tau$ and $T$; in the [Quantronium Ramsey interference experiment](quantronium-ramsey-interference-experiment.md) electronics set the pulse times for a stationary circuit.

**Table of contents**

- [Ramsey fringe envelope](ramsey-fringe-envelope.md)
- [Finite-pulse Ramsey phase response](finite-pulse-ramsey-phase-response.md)
- [Velocity-averaged Ramsey line](velocity-averaged-ramsey-line.md)

## ↑ Ancestors (14)

1. [Ramsey separated oscillatory fields experiment](ramsey-separated-oscillatory-fields-experiment.md)
2. [Ramsey interferometry](ramsey-interferometry.md)
3. [Qubit precession under a constant Hamiltonian](qubit-precession-under-a-constant-hamiltonian.md)
4. [Energy populations and evolving relative phases](energy-populations-and-evolving-relative-phases.md)
5. [Time-evolution operator](time-evolution-operator.md)
6. [Unitary time evolution](unitary-time-evolution.md)
7. [Hamiltonian (quantum mechanics)](hamiltonian-quantum-mechanics.md)
8. [Observable](observable.md)
9. [Quantum state](quantum-state.md)
10. [Quantum system](quantum-system-split.md)
11. [Quantum mechanics](quantum-mechanics-split.md)
12. [Branches of physics](branches-of-physics.md)
13. [Physics](physics-split.md)
14. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Atomic clock frequency shifts](atomic-clock-frequency-shifts.md)
- [Ramsey fringe envelope](ramsey-fringe-envelope.md)
- [Velocity-averaged Ramsey line](velocity-averaged-ramsey-line.md)
