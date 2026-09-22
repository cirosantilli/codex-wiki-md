# Fluorescence instrument response

↑ **Parent:** [Time-correlated single-photon counting](time-correlated-single-photon-counting.md)

A [fluorescence instrument response](fluorescence-instrument-response.md) is the distribution of recorded delays for an effectively prompt optical signal. Finite excitation-pulse width and timing variation in the [photodetector](photodetector.md) and electronics contribute. With a normalized response $R$, intrinsic fluorescent [photon](photon.md) rate $I$, and background rate $B$, the expected trace is

$$
M(t)=\int_{-\infty}^{\infty}R(u)I(t-u)\,du+B(t),\qquad
\int_{-\infty}^{\infty}R(u)\,du=1.
$$

Fit a candidate decay after this [convolution](convolution.md) with the measured response; treating the broadened leading edge as the intrinsic decay can bias [fluorescence lifetime](fluorescence-lifetime.md). The accessible technical note describes measuring prompt scattered excitation with a nonfluorescent scattering sample.[Michael Wahl, Time-Correlated Single Photon Counting, v. 2.1, p. 3: scattering-medium response measurement and iterative reconvolution](time-correlated-single-photon-counting-technical-note-v-2-1-by-michael-wahl.md)

<a id="fluorescence-decay-instrument-convolution"></a>
![](fluorescence-decay-instrument-convolution.png)

**[Figure 32](#fluorescence-decay-instrument-convolution). Synthetic fluorescence lifetime decay broadened by an instrument response**. Original stipulated model, not measurements: $I(t)=e^{-t/(4\,\mathrm{ns})}$ for $t\geq0$ and zero otherwise; $R$ is a normalized [Gaussian function](gaussian-function.md) of [standard deviation](standard-deviation.md) $0.6\,\mathrm{ns}$ centred at zero; the background is $B=0.025$ in the common signal units. The left panel compares intrinsic and convolved traces; the right shows how an unremoved background flattens the tail on a logarithmic scale. Negative delays come from the stipulated timing response about the pulse reference, not emission before excitation. Only the instrument-response curve is rescaled to unit peak for display.

## ↑ Ancestors (8)

1. [Time-correlated single-photon counting](time-correlated-single-photon-counting.md)
2. [Fluorescence lifetime](fluorescence-lifetime.md)
3. [Fluorescence](fluorescence.md)
4. [Physical optics](physical-optics.md)
5. [Optics](optics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Fluorescence instrument response](fluorescence-instrument-response.md)
- [Fluorescence lifetime measurement with pulsed excitation](fluorescence-lifetime-measurement-with-pulsed-excitation.md)
- [Time-correlated single-photon counting](time-correlated-single-photon-counting.md)
