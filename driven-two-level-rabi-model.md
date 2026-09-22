# Driven two-level Rabi model

↑ **Parent:** [Rabi cycle](rabi-cycle.md)

Choose an isolated pair of [energy levels](energy-level.md), with [ground state](ground-state.md) $|g\rangle=(0,1)^T$ and [excited state](excited-state.md) $|e\rangle=(1,0)^T$. Use the [Pauli matrices](pauli-matrices.md) in the ordered [basis](basis.md) $(|e\rangle,|g\rangle)$, so $\sigma_z=\operatorname{diag}(1,-1)$. After subtracting the mean [energy](energy-split.md), prescribe the laboratory [Hamiltonian operator](hamiltonian-quantum-mechanics.md)

$$
H_{\mathrm{lab}}(t)=\frac{\hbar\omega_0}{2}\sigma_z
+\hbar\Omega\cos(\omega t+\phi)\sigma_x,
\qquad \delta=\omega_0-\omega,\qquad \Omega\geq0.
$$

The unperturbed [energy](energy-split.md) gap is $\hbar\omega_0$, the drive has [angular frequency](angular-frequency.md) $\omega$, and $\phi$ fixes its [oscillation phase](phase-waves.md) at the chosen time origin. All of $\omega_0$, $\omega$, the [Rabi angular frequency](rabi-angular-frequency.md) $\Omega$ and the [Rabi detuning](rabi-detuning.md) $\delta$ are in radians per second; ordinary [frequency](frequency.md) is angular frequency divided by $2\pi$. In particular, $\Omega$ here is the coefficient multiplying the cosine in $H_{\mathrm{lab}}/\hbar$, not twice that coefficient.

Write $|\psi_{\mathrm{lab}}\rangle=R(t)|\psi_{\mathrm{rot}}\rangle$ with $R(t)=\exp(-i\omega t\sigma_z/2)$. Transforming the [Schrödinger equation](schrodinger-equation.md) gives $H_{\mathrm{rot}}=R^\dagger H_{\mathrm{lab}}R-i\hbar R^\dagger\dot R$. The [rotating-wave approximation](rotating-wave-approximation.md) drops terms at angular frequency $2\omega$, leaving

$$
H_{\mathrm{rot}}=\frac{\hbar}{2}K,\qquad
K=\begin{pmatrix}\delta&\Omega e^{-i\phi}\\\Omega e^{i\phi}&-\delta\end{pmatrix},\qquad
\Omega_{\mathrm{eff}}=\sqrt{\Omega^2+\delta^2}.
$$

This approximation requires $\Omega,|\delta|\ll\omega_0,\omega$, and an interaction duration over which omitted corrections remain small. It also assumes that other [energy levels](energy-level.md) can be neglected. Resonance alone does not justify either assumption. An exactly co-rotating drive has no discarded counter-rotating component; the linearly oscillating laboratory drive above does.

The [Pauli matrix multiplication law](pauli-matrix-multiplication-law.md) gives $K^2=\Omega_{\mathrm{eff}}^2I$. Separating even and odd terms of the [matrix exponential](matrix-exponential.md) therefore proves

$$
U_{\mathrm{rot}}(t)=I\cos\frac{\Omega_{\mathrm{eff}}t}{2}
-i\frac{K}{\Omega_{\mathrm{eff}}}\sin\frac{\Omega_{\mathrm{eff}}t}{2},
$$

with the continuous limit $U=I$ when $\Omega=\delta=0$. Starting from $|g\rangle$, the upper [probability amplitude](probability-amplitude.md) is $-ie^{-i\phi}(\Omega/\Omega_{\mathrm{eff}})\sin(\Omega_{\mathrm{eff}}t/2)$. The [Born rule](born-rule.md) gives

$$
P_{g\to e}(t)=\frac{\Omega^2}{\Omega^2+\delta^2}
\sin^2\!\left(\frac{\sqrt{\Omega^2+\delta^2}\,t}{2}\right).
$$

The rotating transformation only changes the [quantum phases](quantum-phase.md) of these [basis](basis.md) states, so their laboratory populations are the same. [Rabi detuning](rabi-detuning.md) tilts the rotation axis of the [Bloch vector](bloch-vector.md): it increases the oscillation rate to $\Omega_{\mathrm{eff}}$ but caps the transferred population at $\Omega^2/(\Omega^2+\delta^2)$. A fixed drive [oscillation phase](phase-waves.md) cancels from this single-pulse population when the initial state is $|g\rangle$. It still fixes the relative [quantum phase](quantum-phase.md) of a resulting [quantum superposition](quantum-superposition.md) and matters when another pulse supplies a phase reference.

**Table of contents**

- [Rabi vector](rabi-vector.md)
- [Equatorial reachability of a detuned spin pulse](equatorial-reachability-of-a-detuned-spin-pulse.md)
- [Laboratory phase of a resonant spin pulse](laboratory-phase-of-a-resonant-spin-pulse.md)
- [Rabi angular frequency](rabi-angular-frequency.md)
- [Rabi detuning](rabi-detuning.md)
- [Rabi pi pulse](rabi-pi-pulse.md)

## ↑ Ancestors (10)

1. [Rabi cycle](rabi-cycle.md)
2. [Unitary time evolution](unitary-time-evolution.md)
3. [Hamiltonian (quantum mechanics)](hamiltonian-quantum-mechanics.md)
4. [Observable](observable.md)
5. [Quantum state](quantum-state.md)
6. [Quantum system](quantum-system-split.md)
7. [Quantum mechanics](quantum-mechanics-split.md)
8. [Branches of physics](branches-of-physics.md)
9. [Physics](physics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Finite-pulse Ramsey phase response](finite-pulse-ramsey-phase-response.md)
- [Finite-pulse Ramsey transition probability](finite-pulse-ramsey-transition-probability.md)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2021/section-b/4/b/solution.md)
- [Rabi angular frequency](rabi-angular-frequency.md)
- [Rabi pi pulse](rabi-pi-pulse.md)
- [Resonance envelope of a Rabi transition](resonance-envelope-of-a-rabi-transition.md)
