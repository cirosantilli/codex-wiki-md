# Detector dead time

↑ **Parent:** [Particle detector](particle-detector.md)

The interval during which a detector or readout cannot register another event while recovering from a response. A [detector trigger](trigger-particle-physics.md) may be fast while the camera, chamber or data acquisition is still busy.

In a simple nonextending model, every accepted event starts a fixed busy interval $\tau_d$; arrivals during it are lost and do not extend it. With [Poisson process](poisson-process-split.md) input rate $R$, the average cycle lasts $\tau_d+1/R$, giving observed rate

$$
R_{\rm obs}=\frac{R}{1+R\tau_d}.
$$

This is a specified mathematical model, not a universal correction. An instrument whose busy interval is extended by further arrivals behaves differently. Correcting the total rate also does not remove the [multiplicity bias from a detector trigger](multiplicity-bias-from-a-detector-trigger.md).

**Table of contents**

- [Energy-biased detection probability](energy-biased-detection-probability.md)

## ↑ Ancestors (4)

1. [Particle detector](particle-detector.md)
2. [Particle detection](particle-detection-split.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Finite-bin photon correlations](finite-bin-photon-correlations.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2014/paper-1/section-a/4/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2015/paper-1/section-d/d13/c/solution.md)
- [Photon-recoil lag correlation](photon-recoil-lag-correlation.md)
- [Photon statistics](photon-statistics.md)
