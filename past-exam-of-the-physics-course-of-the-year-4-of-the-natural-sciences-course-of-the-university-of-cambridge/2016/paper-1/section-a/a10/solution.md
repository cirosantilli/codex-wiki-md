<h1 id="section-a/a10/solution">Solution</h1>

↑ **Parent:** [A10](../a10.md)

The fastest clearly resolved late oscillations occupy roughly $0.004$–$0.005\,\mathrm s$ per cycle when compared with the $0.05\,\mathrm s$ major-tick spacing. Thus $f_{\max}$ is of order $200$–$250\,\mathrm{Hz}$ and the [Nyquist–Shannon sampling theorem](../../../../../nyquist-shannon-sampling-theorem.md) requires

$$
\boxed{f_s>2f_{\max}\sim400\text{–}500\,\mathrm{samples\,s^{-1}}.}
$$

A [sampling rate](../../../../../sampling-rate.md) of order $500\,\mathrm{samples\,s^{-1}}$ is the estimated lower boundary for the plotted signal bandwidth; practical acquisition needs anti-alias filtering and margin. This is not a determination of LIGO's actual acquisition rate.[MT-002: bandwidth-limited sampling and anti-alias filtering](../../../../../what-the-nyquist-criterion-means-to-your-sampled-data-system-design-by-walt-kester.md)

The [bit-depth requirements for waveform digitization](../../../../../bit-depth-requirements-for-waveform-digitization.md) need a specified precision. **The numerical bit depth is underdetermined by the figure.** If the digitizer covers a full-scale range $V_{\rm FS}$ and the required quantization step is at most $\Delta$, then

$$
\boxed{b\geq\left\lceil\log_2\frac{V_{\rm FS}}{\Delta}\right\rceil.}
$$

For a uniform quantizer its ideal quantization-noise rms is approximately $\Delta/\sqrt{12}$. No permitted quantization error, noise criterion or calibrated digitizer range is specified. The plotted reconstruction band does not itself define one. Therefore no unique finite bit count, or exact lossless digitization of an arbitrary real-valued waveform, follows from the supplied data.

## ↑ Ancestors (13)

1. [A10](../a10.md)
2. [Section A](../../section-a.md)
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
