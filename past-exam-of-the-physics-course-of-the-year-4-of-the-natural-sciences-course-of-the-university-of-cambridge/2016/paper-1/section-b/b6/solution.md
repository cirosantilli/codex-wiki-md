<h1 id="section-b/b6/solution">Solution</h1>

↑ **Parent:** [B6](../b6.md)

Two applications of [optical interferometry](../../../../../optical-interferometry.md) are precision displacement or strain measurement, and [Fourier transform spectroscopy](../../../../../fourier-transform-spectroscopy.md), which recovers a spectrum from an interferogram.

For the [round-trip phase in a Michelson interferometer](../../../../../round-trip-phase-in-a-michelson-interferometer.md), take a lossless 50:50 [beam splitter](../../../../../beam-splitter.md) with $t=1/\sqrt2$ and $r=i/\sqrt2$, and mirror reflection amplitude $-1$. At the depicted detector, each returning path has one beam-splitter transmission and one reflection. Their amplitudes are $-iA_0e^{2ikD}/2$ and $-iA_0e^{2ik(D+\delta)}/2$. Consequently,

$$
\boxed{I(\delta)=\frac{|A_0|^2}{2}[1+\cos(2k\delta)]=|A_0|^2\cos^2(k\delta).}
$$

The factor 2 in the phase is the return journey: the labelled $\delta$ is a one-way arm-length difference. The other output port has the complementary [intensity](../../../../../intensity-physics.md). **The printed $|A_0|^2(1+2\cos k\delta)$ cannot be an [intensity](../../../../../intensity-physics.md):** it becomes negative, and does not match the depicted path difference. No choice of normalization fixes that negative minimum. The expression above is the physically consistent result for the drawn output port.

For mutually incoherent spectral components with incident power [density](../../../../../density.md) $S(k)$,

$$
I(\delta)=\frac12\int S(k)[1+\cos(2k\delta)]\,dk.
$$

The plot labels are $\lambda_1=589.59\,\mathrm{nm}$ and $\lambda_2=590.00\,\mathrm{nm}$; these printed centres are used here. In the narrow-line, equal-power limit, each line has incident [intensity](../../../../../intensity-physics.md) $J$ and

$$
\boxed{I=J[1+\cos((k_1+k_2)\delta)\cos((k_1-k_2)\delta)].}
$$

There are rapid carrier fringes with approximately $0.2949\,\mathrm{\mu m}$ mirror-displacement spacing and a slowly varying [Interferometric visibility](../../../../../interferometric-visibility.md) envelope. The first visibility zero is at $0.2121\,\mathrm{mm}$, and successive visibility revivals are separated by

$$
\boxed{\Delta\delta_{\rm vis}=\frac\pi{|k_1-k_2|}=\frac{\lambda_1\lambda_2}{2|\lambda_2-\lambda_1|}=0.4242\,\mathrm{mm}.}
$$

For the [unequal-line visibility in a spectral doublet](../../../../../unequal-line-visibility-in-a-spectral-doublet.md), with incident line powers $J_1,J_2$, replace the [intensity](../../../../../intensity-physics.md) by $[J_1+J_2+J_1\cos(2k_1\delta)+J_2\cos(2k_2\delta)]/2$. The visibility becomes

$$
\mathcal V(\delta)=\frac{\sqrt{J_1^2+J_2^2+2J_1J_2\cos(2(k_1-k_2)\delta)}}{J_1+J_2}.
$$

The visibility minima rise from zero to $|J_1-J_2|/(J_1+J_2)$. The finite widths drawn in the spectrum also make coherence decay with path difference. For example, Gaussian lines of common wave-number [standard deviation](../../../../../standard-deviation.md) $\sigma_k$ multiply the oscillatory term by $e^{-2\sigma_k^2\delta^2}$; the actual linewidth is not specified numerically. Thus the narrow-line plot gives the beat positions, while the true long-delay oscillations die away.[Temporal coherence and interference of incoherent spectral components](../../../../../interference-and-coherence-by-sander-konijnenberg-aurele-j-l-adam-and-h-paul-urbach.md)

<a id="section-b/b6/image-doublet-interferograms-unequal-line-powers-prevent-complete-loss-of-visibility-finite-linewidth-damps-the-revival-envelope"></a>
![](../../../../../past-exam-of-the-physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1-doublet-interferogram.png)

**[Figure 5](#section-b/b6/image-doublet-interferograms-unequal-line-powers-prevent-complete-loss-of-visibility-finite-linewidth-damps-the-revival-envelope). Doublet interferograms: unequal line powers prevent complete loss of visibility; finite linewidth damps the revival envelope**. [Source](paper-1-doublet-interferogram.py).

The [common-arm phase cancellation in a balanced interferometer](../../../../../common-arm-phase-cancellation-in-a-balanced-interferometer.md) means **there is no smallest positive common mirror distance $D$ in a balanced interferometer.** With $\delta=0$ the common factor $e^{2ikD}$ cancels from every [intensity](../../../../../intensity-physics.md), and both paths interfere constructively at this detector for every $D>0$. Their infimum is zero. The $0.4242\,\mathrm{mm}$ beat length describes changes of arm difference, not of the common arm length. It therefore cannot answer the final request as printed.

## ↑ Ancestors (13)

1. [B6](../b6.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
