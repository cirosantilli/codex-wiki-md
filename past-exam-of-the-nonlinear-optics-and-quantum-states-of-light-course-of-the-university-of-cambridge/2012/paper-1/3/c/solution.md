<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[Frequency-resolved optical gating](../../../../../frequency-resolved-optical-gating.md) characterizes an ultrashort pulse using a nonlinear gate and a measured two-dimensional [spectrogram](../../../../../spectrogram.md). In [second-harmonic frequency-resolved optical gating](../../../../../second-harmonic-frequency-resolved-optical-gating.md), split the pulse into two replicas, vary their relative delay, overlap them noncollinearly in a thin second-harmonic crystal, and spectrally resolve the cross-generated beam. Its propagation direction separates it from the individual beams' self-generated harmonics. For complex pulse envelope $E(t)$, the ideal trace is

$$
\boxed{I_{\rm FROG}(\Omega,\tau)\propto\left|\int E(t)E(t-\tau)e^{-i\Omega t}\,dt\right|^2,}
$$

where $\Omega$ denotes the output [frequency](../../../../../frequency.md) offset in the envelope convention. An iterative [phase retrieval](../../../../../phase-retrieval.md) algorithm seeks a pulse consistent with both this measured Fourier magnitude and the nonlinear product relation. The delay axis provides timing structure, while the resolved spectrum adds information missing from a plain intensity [autocorrelation](../../../../../autocorrelation.md).[1993, nonlinear-gating spectrogram and pulse reconstruction](../../../../../characterization-of-arbitrary-femtosecond-pulses-using-frequency-resolved-optical-gating-by-daniel-j-kane-and-rick-trebino.md)

The measured trace does not fix absolute optical phase or absolute time origin. SHG FROG also has a conjugate time-reversal ambiguity: $E(t)$ and $E^*(-t)$ produce the same trace. Extra information, such as a known dispersion change and a second measurement, can resolve that direction-of-time ambiguity. Finite phase-matching bandwidth, [group-velocity mismatch](../../../../../group-velocity-mismatch.md), spatial chirp, [spectrometer](../../../../../spectrometer.md) calibration, delay error, noise and instability over the scan must be controlled. A thin gate helps avoid temporal blurring, but trades against signal. FROG therefore reconstructs a pulse under an explicit instrument model rather than reading optical phase directly from a single intensity image.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the nonlinear Optics and Quantum States of Light course of the University of Cambridge](../../../../split.md)
6. [Nonlinear Optics and Quantum States of Light course of the University of Cambridge](../../../../../nonlinear-optics-and-quantum-states-of-light-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
