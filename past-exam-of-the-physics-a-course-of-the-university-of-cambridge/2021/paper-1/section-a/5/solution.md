<h1 id="section-a/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For a real signal with highest [frequency](../../../../../frequency.md) $f_{\max}=40\,\mathrm{MHz}$, the [Nyquist–Shannon sampling theorem](../../../../../nyquist-shannon-sampling-theorem.md) gives the nominal Nyquist [sampling rate](../../../../../sampling-rate.md)

$$
\boxed{f_{s,\mathrm{Nyquist}}=2f_{\max}=80\,\mathrm{MHz}
=80\times10^6\ \text{samples per second}.}
$$

To cover an arbitrary component exactly at the band edge, choose $f_s>80\,\mathrm{MHz}$: a $40\,\mathrm{MHz}$ sine sampled at exactly $80\,\mathrm{MHz}$ can have every sample equal to zero for an unfortunate phase. Practical [aliasing](../../../../../aliasing.md) suppression also calls for a margin above the nominal limiting rate.

With rounding to the nearest digitizer level, [quantization](../../../../../quantization-signal-processing.md) with step $q=0.1\,\mathrm{mV}$ has the [uniform-quantization error bound](../../../../../uniform-quantization-error-bound.md)

$$
\boxed{|V_{\mathrm{digitized}}-V_{\mathrm{sample}}|\leq q/2=0.05\,\mathrm{mV}.}
$$

Thus the stated digitizer meets the requested nominal amplitude precision per sample, assuming no clipping or other errors. The bandwidth sets the nominal minimum sampling rate; the level spacing sets the rounding precision. Strictly, the sampling theorem reconstructs exactly from exact samples. A uniform $0.05\,\mathrm{mV}$ error bound on the entire reconstructed continuous waveform is not guaranteed by the level spacing and sampling rate alone; that stronger requirement needs a specified reconstruction and noise model.

## ↑ Ancestors (14)

1. [5](../5.md)
2. [Section A](../../section-a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2021](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
