# Velocity-averaged Ramsey line

↑ **Parent:** [Finite-pulse Ramsey transition probability](finite-pulse-ramsey-transition-probability.md)

Let each drive region have length $\ell$ and the drive-free gap have length $L$, measured edge to edge. A particle of constant [speed](speed.md) $v>0$ experiences $\tau(v)=\ell/v$ and $T(v)=L/v$. For a normalized detected-beam speed [probability density function](probability-density-function.md) $f(v)$, sum the transition [probabilities](probability.md), not the [probability amplitudes](probability-amplitude.md) of different particles:

$$
\overline P(\delta)=\int_0^\infty f(v)P_{g\to e}(\delta;\ell/v,L/v)\,dv,\qquad
f(v)=\frac{2v^3}{u^4}e^{-(v/u)^2},\quad v>0.
$$

The displayed $f$ is an ideal [effusion](effusion.md) flux distribution, with speed scale $u$, uniform transmission and speed-independent detection efficiency. It is not a claim about any particular clock's selected beam. The substitution $x=(v/u)^2$ gives $f(v)dv=xe^{-x}dx$, proving normalization. Actual apertures, state selection and readout can change the effective weights.

For an original example choose $\ell=0.10\,\mathrm m$, $L=1.00\,\mathrm m$, $u=v_*=200\,\mathrm{m\,s^{-1}}$ and $\Omega=2\pi\times500\,\mathrm{rad\,s^{-1}}$. The reference particle has $\tau_*=0.500\,\mathrm{ms}$, $T_*=5.00\,\mathrm{ms}$ and resonant $\pi/2$ pulses. The instantaneous-pulse width would be $100\,\mathrm{Hz}$. The exact finite-pulse width for that single [speed](speed.md) is about $88.7\,\mathrm{Hz}$; the chosen distribution also reduces the on-resonance average to approximately $0.738$ because not every particle receives a $\pi/2$ pulse.

<a id="image-finite-transit-times-shape-the-ramsey-line"></a>
![](ramsey-finite-pulse-velocity-average.png)

**[Figure 11](#image-finite-transit-times-shape-the-ramsey-line). Finite transit times shape the Ramsey line**. Original calculation of the [finite-pulse Ramsey transition probability](finite-pulse-ramsey-transition-probability.md) and [velocity-averaged Ramsey line](velocity-averaged-ramsey-line.md) for the chosen parameters above. The central panel also shows the instantaneous-pulse limit at $v_*$. All curves are model predictions; none reproduce experimental points.

Different [velocities](velocity.md) smear side fringes because $\delta L/v$ varies across the beam. Nevertheless every term is even in $\delta$, so this symmetric ideal-model average has no odd line asymmetry that could displace the central lock point. Reduced contrast or altered width alone is not evidence of a shifted line center. A speed-dependent transition shift or unequal drive [quantum phases](quantum-phase.md) changes that conclusion; [atomic clock frequency shifts](atomic-clock-frequency-shifts.md) explains why these distinctions matter experimentally.

## ↑ Ancestors (15)

1. [Finite-pulse Ramsey transition probability](finite-pulse-ramsey-transition-probability.md)
2. [Ramsey separated oscillatory fields experiment](ramsey-separated-oscillatory-fields-experiment.md)
3. [Ramsey interferometry](ramsey-interferometry.md)
4. [Qubit precession under a constant Hamiltonian](qubit-precession-under-a-constant-hamiltonian.md)
5. [Energy populations and evolving relative phases](energy-populations-and-evolving-relative-phases.md)
6. [Time-evolution operator](time-evolution-operator.md)
7. [Unitary time evolution](unitary-time-evolution.md)
8. [Hamiltonian (quantum mechanics)](hamiltonian-quantum-mechanics.md)
9. [Observable](observable.md)
10. [Quantum state](quantum-state.md)
11. [Quantum system](quantum-system-split.md)
12. [Quantum mechanics](quantum-mechanics-split.md)
13. [Branches of physics](branches-of-physics.md)
14. [Physics](physics-split.md)
15. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Cesium-beam clock procedure](cesium-beam-clock-procedure.md)
- [Ramsey fringe envelope](ramsey-fringe-envelope.md)
- [Velocity-averaged Ramsey line](velocity-averaged-ramsey-line.md)
