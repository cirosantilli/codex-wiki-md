# Rabi transit-time and field averaging

↑ **Parent:** [Rabi molecular beam magnetic resonance experiment](rabi-molecular-beam-magnetic-resonance-experiment.md)

For an ideal single transit, let the oscillatory [magnetic field](magnetic-field-split.md) occupy a region of length $L$, take the longitudinal [speed](speed.md) $v$ constant, and neglect edge fields. Each molecule then experiences one square pulse of duration $\tau=L/v$. This is one contiguous interaction region, distinct from the two separated pulses of [Ramsey interferometry](ramsey-interferometry.md). The static [magnetic field](magnetic-field-split.md) sets the selected transition gap; the transverse drive sets [Rabi angular frequency](rabi-angular-frequency.md). A change of RF [frequency](frequency.md) or static [magnetic field](magnetic-field-split.md) changes [Rabi detuning](rabi-detuning.md).

For an original ideal detector model, suppose every successful transition removes an otherwise accepted molecule and the incident beam occupies the lower state of the selected pair. With accepted no-transition signal $S_0$, constant background $S_{\mathrm{bg}}$, and effective loss contrast $0\leq\eta\leq1$, write

$$
S(\delta)=S_{\mathrm{bg}}+S_0[1-\eta\,\overline P(\delta)].
$$

For identical trajectories $\overline P=P_{g\to e}(L/v)$, giving an intensity dip where transfer is largest. For real trajectory variation, a normalized joint [probability density](probability-density.md) $w(v,\epsilon,\Omega')$ gives the static-offset model

$$
\overline P(\delta)=\int_0^\infty\!dv\int_{-\infty}^\infty\!d\epsilon\int_0^\infty\!d\Omega'\,
 w(v,\epsilon,\Omega')
 \frac{\Omega'^2}{\Omega'^2+(\delta+\epsilon)^2}
 \sin^2\!\left[\frac{L}{2v}\sqrt{\Omega'^2+(\delta+\epsilon)^2}\right],
\qquad \int w\,dv\,d\epsilon\,d\Omega'=1.
$$

Here $\epsilon$ is the trajectory's transition-frequency offset and $\Omega'$ its drive strength, each in angular-frequency units. The weighting is for molecules accepted by the apparatus, rather than an assumed unfiltered oven distribution. In particular, designing $\Omega L/v_0=\pi$ does not produce a [Rabi pi pulse](rabi-pi-pulse.md) for every speed: at $0.8v_0$ and $1.2v_0$ the resonant transfer probabilities are respectively $\sin^2(5\pi/8)\simeq0.8536$ and $\sin^2(5\pi/12)\simeq0.9330$.

Spread in transit times, static [magnetic fields](magnetic-field-split.md) and drive amplitudes can reduce or smear oscillations without [quantum decoherence](quantum-decoherence.md) on any individual trajectory. Even the single-transit square pulse has finite spectral width of order $1/\tau$ in [angular frequency](angular-frequency.md). If the [magnetic field](magnetic-field-split.md) varies substantially along one path, its [Hamiltonian operator](hamiltonian-quantum-mechanics.md) changes during the passage and the constant-offset average above must be replaced by a [time-ordered exponential](time-ordered-exponential.md). Actual molecules may also have several coupled [energy levels](energy-level.md); the isolated pair and perfect loss discriminator are explicit idealizations of this model.

## ↑ Ancestors (11)

1. [Rabi molecular beam magnetic resonance experiment](rabi-molecular-beam-magnetic-resonance-experiment.md)
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
