# Accidental coincidence

↑ **Parent:** [Coincidence circuit](coincidence-circuit.md)

Suppose two independent background streams follow [Poisson processes](poisson-process-split.md) with rates $r_1$ and $r_2$. Define a coincidence by $|t_2-t_1|<w/2$: **$w$ is the full accepted time-difference width**. Around each first-counter signal, the expected number of second-counter signals is $r_2w$. The expected pair rate is therefore $r_1r_2w$. A circuit producing at most one output per first signal instead gives

$$
R_{\rm acc}=r_1(1-e^{-r_2w})\simeq r_1r_2w\qquad(r_2w\ll1).
$$

The distinction matters when multiple detections occur in one window. If a different convention accepts $|t_2-t_1|<\tau$, its full width is $w=2\tau$ and the dilute expression is $2r_1r_2\tau$.

For a chosen numerical model, take background rates $r_1=100\,\mathrm{s^{-1}}$, $r_2=80\,\mathrm{s^{-1}}$ and $w=20\,\mu\mathrm s$. The dilute pair rate is $0.16\,\mathrm{s^{-1}}$. These are stipulated teaching inputs, not measurements of the historical chamber.

Making $w$ smaller also rejects some genuine events. Suppose true pairs arrive at rate $S_0$ before the timing cut, and their time difference has a centered [normal distribution](normal-distribution.md) with [standard deviation](standard-deviation.md) $\sigma_t$. Its accepted fraction, using the [error function](error-function.md), is

$$
\epsilon_t(w)=\operatorname{erf}\!\left(\frac{w}{2\sqrt2\sigma_t}\right),\qquad
S(w)=S_0\epsilon_t(w).
$$

For chosen $S_0=2.0\,\mathrm{s^{-1}}$ and $\sigma_t=5\,\mu\mathrm s$, the $20\,\mu\mathrm s$ window retains about $95.45\%$ of true pairs. In the dilute background model the fraction of accepted events that are true is $S/(S+R_{\rm acc})\simeq92.27\%$. A narrow window trades [detection efficiency](detection-efficiency.md) against background; it does not make either quantity equal to one. Delaying one counter's signal far beyond genuine event correlations gives a proposed background check under stationarity, without assuming that the zero-delay excess itself is accidental.

## ↑ Ancestors (6)

1. [Coincidence circuit](coincidence-circuit.md)
2. [Trigger (particle physics)](trigger-particle-physics.md)
3. [Particle detector](particle-detector.md)
4. [Particle detection](particle-detection-split.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Bothe-Geiger coincidence experiment](bothe-geiger-coincidence-experiment.md)
- [Brookhaven J pair-spectrometer experiment](brookhaven-j-pair-spectrometer-experiment.md)
- [Chamberlain-Segrè antiproton identification](chamberlain-segre-antiproton-identification.md)
- [Coincidence circuit](coincidence-circuit.md)
- [Delayed neutron-capture coincidence window](delayed-neutron-capture-coincidence-window.md)
- [Detection loophole](detection-loophole.md)
- [Freedman-Clauser experiment](freedman-clauser-experiment.md)
- [Multiwire proportional chamber experiment](multiwire-proportional-chamber-experiment.md)
- [Photon-recoil lag correlation](photon-recoil-lag-correlation.md)
