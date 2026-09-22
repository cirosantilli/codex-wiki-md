# Rabi pi pulse

↑ **Parent:** [Driven two-level Rabi model](driven-two-level-rabi-model.md)

For a constant-amplitude square pulse on resonance, a [Rabi pi pulse](rabi-pi-pulse.md) lasts $\tau_\pi=\pi/\Omega$ and gives $|g\rangle\mapsto-ie^{-i\phi}|e\rangle$ in the rotating frame. A half-duration pulse prepares $(|g\rangle-ie^{-i\phi}|e\rangle)/\sqrt2$. The [quantum pulse area](quantum-pulse-area.md) $\Omega t$ determines these rotations only under the stated resonant, constant-axis assumptions; a detuned drive rotates about a different axis.

As an original numerical illustration, choose $\Omega=2\pi\times1000\ \mathrm{rad\,s^{-1}}$ and hence $\tau_\pi=0.500\ \mathrm{ms}$. These are chosen model parameters, not historical apparatus settings. Holding that duration fixed gives

$$
x=\frac{\delta}{\Omega},\qquad
P_\pi(x)=\frac{\sin^2[(\pi/2)\sqrt{1+x^2}]}{1+x^2}.
$$

Thus $P_\pi(0)=1$, $P_\pi(1)=\tfrac12\sin^2(\pi/\sqrt2)\simeq0.3166$, and $P_\pi(\sqrt3)=0$. The last zero comes from completing a full rotation about the tilted axis, rather than switching the drive off. At zero [Rabi detuning](rabi-detuning.md), doubling the pulse duration restores the ground-state population; continuous driving does not keep transferring population irreversibly.

<a id="image-ideal-rabi-oscillations-and-the-detuning-response-of-a-fixed-pi-pulse"></a>
![](rabi-square-pulse-detuning.png)

**[Figure 12](#image-ideal-rabi-oscillations-and-the-detuning-response-of-a-fixed-pi-pulse). Ideal Rabi oscillations and the detuning response of a fixed pi pulse**. Original [Driven two-level Rabi model](driven-two-level-rabi-model.md), with no measured points. The left panel varies pulse duration; the right fixes $\Omega\tau_\pi=\pi$ and varies [Rabi detuning](rabi-detuning.md). The dotted curve is the population-transfer upper bound, not a fitted spectral line.

## ↑ Ancestors (11)

1. [Driven two-level Rabi model](driven-two-level-rabi-model.md)
2. [Rabi cycle](rabi-cycle.md)
3. [Unitary time evolution](unitary-time-evolution.md)
4. [Hamiltonian (quantum mechanics)](hamiltonian-quantum-mechanics.md)
5. [Observable](observable.md)
6. [Quantum state](quantum-state.md)
7. [Quantum system](quantum-system-split.md)
8. [Quantum mechanics](quantum-mechanics-split.md)
9. [Branches of physics](branches-of-physics.md)
10. [Physics](physics-split.md)
11. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2015/paper-1/4/iii/solution.md)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2017/1/a/solution.md)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2021/section-b/4/c/solution.md)
- [Rabi cycle](rabi-cycle.md)
- [Rabi pi pulse](rabi-pi-pulse.md)
- [Rabi transit-time and field averaging](rabi-transit-time-and-field-averaging.md)
- [Ramsey fringe envelope](ramsey-fringe-envelope.md)
- [Ramsey spectroscopy](ramsey-spectroscopy.md)
- [Trapped-ion sideband pulse model](trapped-ion-sideband-pulse-model.md)
