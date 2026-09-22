# Two-path attosecond phase reconstruction

↑ **Parent:** [Reconstruction of attosecond beating by interference of two-photon transitions](reconstruction-of-attosecond-beating-by-interference-of-two-photon-transitions.md)

An original two-amplitude model makes the timing inference explicit. Use the [spectral phase](spectral-phase.md) convention of the [coherent harmonic pulse-train model](coherent-harmonic-pulse-train-model.md), and define positive delay $\tau$ to retard the reference [electric field](electric-field-split.md). Let the amplitudes leading to the same final [photoelectron](photoelectron.md) state be

$$
M_-(\tau)=b_-e^{i(\phi_{q-1}+\omega\tau+\eta_-)},\qquad
M_+(\tau)=b_+e^{i(\phi_{q+1}-\omega\tau+\eta_+)},
$$

with real $b_\pm\geq0$. Squaring their sum gives

$$
S_q(\tau)=b_-^2+b_+^2+2b_-b_+\cos(2\omega\tau-\Delta\phi_q+\delta_q),
\qquad \Delta\phi_q=\phi_{q+1}-\phi_{q-1},\quad\delta_q=\eta_--\eta_+.
$$

The $2\omega$ oscillation comes from opposite signs of the reference [photon](photon.md)'s [phase](phase-waves.md). For $\Delta\phi_q=2\omega t_0$ and $\delta_q=0$, the signal peaks at $\tau=t_0$ modulo $T/2$. A fitted phase contains the target contribution $\delta_q$; setting it to zero is an assumption, not an observation. In an experiment, unobserved final channels can add as probabilities, so the displayed formula is one effective-channel idealization.

For a chosen example, impose $\Delta\phi_q=0.80$ radians and $\delta_q=0.15$ radians at $800\,\mathrm{nm}$. The observed oscillation has argument $2\omega\tau-0.65$. Its peak shift is $0.1380\,\mathrm{fs}$, while the corrected finite-difference [group delay](group-delay.md) is $\Delta\phi_q/(2\omega)=0.1699\,\mathrm{fs}$. Ignoring the target contribution would bias the inferred delay by $-31.9$ attoseconds. These stipulated phases demonstrate a reconstruction error; they are not atomic calculations or measured delays.

Recovering all neighboring phase differences determines the component [spectral phases](spectral-phase.md) up to an overall [phase](phase-waves.md) and the chosen timing origin, provided the oscillation phases are consistently unwrapped. Known component amplitudes then give a temporal field by a finite inverse [Fourier transform](fourier-transform-split.md). This is why measuring the [optical spectrum](optical-spectrum.md) alone is insufficient: it omits the very information that decides when constructive [wave interference](interference-wave-propagation.md) occurs.

## ↑ Ancestors (7)

1. [Reconstruction of attosecond beating by interference of two-photon transitions](reconstruction-of-attosecond-beating-by-interference-of-two-photon-transitions.md)
2. [Attosecond physics](attosecond-physics.md)
3. [Laser](laser-split.md)
4. [Optics](optics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [2001 attosecond pulse-train experiment](2001-attosecond-pulse-train-experiment.md)
- [Reconstruction of attosecond beating by interference of two-photon transitions](reconstruction-of-attosecond-beating-by-interference-of-two-photon-transitions.md)
