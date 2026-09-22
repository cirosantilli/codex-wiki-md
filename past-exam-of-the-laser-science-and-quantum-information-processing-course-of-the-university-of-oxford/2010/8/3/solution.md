<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [optical success probability of a fourfold GHZ source](../../../../optical-success-probability-of-a-fourfold-ghz-source.md) depends on the photon-number statistics of the assumed two-pair input. Let $q$ be the probability that arm $a$ contains one $H$ and one $V$, given two pairs. The [beam splitter](../../../../beam-splitter.md) then puts one of the two $b$ photons into each output with probability $1/2$, and the final polarization-parity selection succeeds with probability $1/2$. With ideal [photodetectors](../../../../photodetector.md),

$$
\boxed{P(\text{fourfold}\mid\text{two pairs})=\frac q4.}
$$

For the normalized, fully overlapping [two-pair component of polarization-entangled down-conversion](../../../../two-pair-component-of-polarization-entangled-down-conversion.md) used above, $q=1/3$, so the squared norm of the accepted component gives **$P=1/12$**. Treating the two emissions instead as independently labelled [Bell pairs](../../../../bell-pair.md) gives the commonly used bookkeeping estimate $q=1/2$ and **$P=1/8$**. This is a different pair-statistics approximation; it must not be obtained by dropping labels from an input state without renormalizing it. Genuine [GHZ state](../../../../greenberger-horne-zeilinger-state.md) coherence additionally requires erasing information about the pair of origin.

Let $P_2$ be the two-pair probability per pulse and $f$ the pulse [repetition rate](../../../../pulse-repetition-frequency.md). The coincidence rate is **$R=fP_2q/4$**. With the usual order-of-magnitude estimate $P_2\simeq p^2$, the supplied $f=10^6\,\mathrm{s^{-1}}$ and $p=10^{-3}$ give $fP_2\simeq1\,\mathrm{s^{-1}}$. The fully overlapping model gives **$R\simeq0.083\,\mathrm{s^{-1}}$**, about one event per twelve seconds; independent-pair bookkeeping gives **$R\simeq0.125\,\mathrm{s^{-1}}$**, about one per eight seconds. Thus the estimate is of order **$10^{-1}\,\mathrm{s^{-1}}$** under these idealizations.

An exact prefactor cannot follow from the single-pair probability alone. For example, the [pair-number statistics of polarization-entangled down-conversion](../../../../pair-number-statistics-of-polarization-entangled-down-conversion.md) in a single collected mode pair give $P_2\simeq3p^2/4$ at weak gain, and hence **$R\simeq fp^2/16=0.0625\,\mathrm{s^{-1}}$** with $q=1/3$. Multiple temporal or spectral modes change those statistics. Real collection losses and detector efficiencies further reduce the rate; they are excluded by the ideal calculation.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [8](../../8-split.md)
3. [2010](../../split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
