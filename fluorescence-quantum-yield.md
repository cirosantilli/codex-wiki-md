# Fluorescence quantum yield

↑ **Parent:** [Fluorescence](fluorescence-split.md)

[Fluorescence quantum yield](fluorescence-quantum-yield.md) counts emitted fluorescent [photons](photon.md) per absorbed excitation [photon](photon.md). It differs from [quantum efficiency](quantum-efficiency.md), which describes the [photodetector](photodetector.md).[§1.1.2, Quantum yield, equation 2 and the quantum-efficiency distinction](advanced-fluorescence-microscopy-techniques-frap-flip-flap-fret-and-flim-by-hellen-c-ishikawa-ankerhold-and-others.md)

For an original constant-rate model, let $k_{\rm r}$ be the radiative decay rate and $k_{\rm nr}$ the sum of competing rates without fluorescent [photon emission](photon-emission.md). An initial population $N_0$ in the emitting [excited state](excited-state.md) obeys the [rate equation](rate-equation.md)

$$
\frac{dN}{dt}=-(k_{\rm r}+k_{\rm nr})N,\qquad
N(t)=N_0e^{-t/\tau},\qquad
\tau=\frac{1}{k_{\rm r}+k_{\rm nr}}.
$$

Integrating $k_{\rm r}N(t)$ over all [time](time-in-physics.md) gives

$$
\Phi=\frac{1}{N_0}\int_0^\infty k_{\rm r}N(t)\,dt
=\frac{k_{\rm r}}{k_{\rm r}+k_{\rm nr}}=k_{\rm r}\tau.
$$

Here every absorbed excitation is assumed to reach this emitting population; additional losses before that stage require another factor. Under steady weak excitation, absorbed [photon](photon.md) rate $R_{\rm abs}$ and total detection fraction $\eta$ give $C=\eta\Phi R_{\rm abs}$. The count rate therefore mixes excitation, yield, and detection, whereas $\tau$ specifies a decay timescale.

## ↑ Ancestors (6)

1. [Fluorescence](fluorescence-split.md)
2. [Physical optics](physical-optics-split.md)
3. [Optics](optics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Dynamic fluorescence quenching](dynamic-fluorescence-quenching.md)
- [Fluorescence excitation spectrum](fluorescence-excitation-spectrum.md)
- [Fluorescence lifetime](fluorescence-lifetime.md)
- [Fluorescence quantum yield](fluorescence-quantum-yield.md)
- [Fluorophore](fluorophore.md)
- [Light-emitting diode efficiency](light-emitting-diode-efficiency.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/paper-2a/section-b/22/a/i/solution.md)
- [Phosphor-converted white light-emitting diode](phosphor-converted-white-light-emitting-diode.md)
