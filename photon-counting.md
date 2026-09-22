# Photon counting

↑ **Parent:** [Quantum optics](quantum-optics-split.md)

[Photon counting](photon-counting.md) registers discrete detector events and their times. A [beam splitter](beam-splitter.md) sends the selected [light](light.md) to two [photodetectors](photodetector.md); a [coincidence circuit](coincidence-circuit.md) or time-recording system compares the outputs. With a vacuum input at the unused [optical port](optical-port.md), splitter fractions $R,T$ and independent [quantum efficiencies](quantum-efficiency.md) $\eta_1,\eta_2$, a selected input [photon](photon.md) reaches the two recorded channels with probabilities $p_1=R\eta_1$ and $p_2=T\eta_2$. Conditional on input occupation $N$, each pair of distinct [photons](photon.md) contributes $p_1p_2$ to the cross-channel pair moment. Therefore

$$
\langle K_1\rangle=p_1\mu,\qquad
\langle K_2\rangle=p_2\mu,\qquad
\langle K_1K_2\rangle=p_1p_2\langle N(N-1)\rangle.
$$

Their normalized ratio recovers $g^{(2)}(0)$. This assumes number-resolving counts, or sufficiently dilute gates for threshold detectors to approximate them. One [photon](photon.md) cannot create both channel counts in this ideal model.

<a id="image-functional-two-detector-photon-correlation-measurement-and-its-normalization"></a>
![](photon-coincidence-readout.png)

**[Figure 2](#image-functional-two-detector-photon-correlation-measurement-and-its-normalization). Functional two-detector photon-correlation measurement and its normalization**. Original schematic: optical selection and a beam splitter feed independent detectors; all cross-channel time differences populate a histogram. A single photon produces at most one ideal detection. The empty splitter input is vacuum.

**Table of contents**

- [Coincidence counting](coincidence-counting.md)
- [Finite-bin photon correlations](finite-bin-photon-correlations.md)
- [Photon correlation loss and background model](photon-correlation-loss-and-background-model.md)

## ↑ Ancestors (5)

1. [Quantum optics](quantum-optics-split.md)
2. [Quantum theory](quantum-theory-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Number squeezing](number-squeezing.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1/section-b/b2/solution.md)
- [Photon counting](photon-counting.md)
- [Quantum optics](quantum-optics-split.md)
- [Resonance fluorescence antibunching experiment](resonance-fluorescence-antibunching-experiment.md)
