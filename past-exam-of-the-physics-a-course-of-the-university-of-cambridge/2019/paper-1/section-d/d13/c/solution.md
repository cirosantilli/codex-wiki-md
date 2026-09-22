<h1 id="section-d/d13/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Digital acquisition converts a continuous [voltage](../../../../../../voltage.md) signal into timed numerical samples. A practical chain is a suitably buffered and amplified sensor signal, an analogue [anti-aliasing filter](../../../../../../anti-aliasing-filter.md), a sampling or sample-and-hold stage, an [analog-to-digital converter](../../../../../../analog-to-digital-converter.md), and a clocked data-storage system. Choose the gain so that the interesting variation uses the available input range without clipping. Finite [input impedance](../../../../../../input-impedance.md) can load a sensor, so an appropriate buffer or [operational amplifier](../../../../../../operational-amplifier.md) may be needed.

Sampling makes time discrete. If the conditioned signal is confined below [frequency](../../../../../../frequency.md) $f_{\max}$, choose a [sampling rate](../../../../../../sampling-rate.md) $f_s>2f_{\max}$, allowing a transition band for the physical filter. The [Nyquist–Shannon sampling theorem](../../../../../../nyquist-shannon-sampling-theorem.md) permits ideal reconstruction of a suitably [bandlimited function](../../../../../../bandlimited-function.md) from exact samples. Without filtering, components separated by integer multiples of $f_s$ have identical samples; in particular real sinusoids at $f$ and $f_s-f$ can be indistinguishable. This [aliasing](../../../../../../aliasing.md) cannot generally be undone by later digital filtering. Oversampling can ease filter design, but does not replace the requirement to suppress unwanted high-frequency content before sampling.

[Amplitude](../../../../../../wave-amplitude.md) [quantization](../../../../../../quantization-signal-processing.md) is separate from sampling. A uniform $b$-[bit](../../../../../../bit.md) converter covering [voltage](../../../../../../voltage.md) span $V_{\mathrm{span}}$ has step $q\simeq V_{\mathrm{span}}/2^b$. Rounding an in-range input gives the [uniform-quantization error bound](../../../../../../uniform-quantization-error-bound.md) $|\epsilon|\leq q/2$. If the rounding errors can additionally be modeled as uniform and uncorrelated, their [standard deviation](../../../../../../standard-deviation.md) is $q/\sqrt{12}$. This statistical estimate is not a guarantee for a constant input or a coherent periodic signal. More bits increase resolution, but accuracy also depends on voltage-reference calibration, offset, gain error, nonlinearity and electronic [noise](../../../../../../noise-signal-processing.md). Out-of-range signals clip and invalidate the rounding bound.

Clock quality matters too. Timing jitter $\delta t$ gives a [voltage](../../../../../../voltage.md) error approximately $(dV/dt)\delta t$; for a sinusoid its scale grows with $2\pi fV_p\sigma_t$. A clock calibration error biases measured frequencies and time intervals. Simultaneous multichannel signals need known relative timing, and the sampling and analogue settling times must be appropriate to the signal [bandwidth](../../../../../../bandwidth-signal-processing.md).

For $n_c$ channels the raw recording rate is approximately $n_cf_sb$ bits per second, before overhead, so storage and sustained transfer speed must prevent missing data. Store units, channel identities, timestamps, [sampling rate](../../../../../../sampling-rate.md), input ranges and calibration information along with the readings. Preserve the original samples when applying digital filters or other processing. Averaging can improve precision for independent fluctuating errors, but cannot restore aliased frequencies, clipped peaks or a fixed rounding bias. Digital recording makes reproducible analysis and transmission possible when its sampling, [amplitude](../../../../../../wave-amplitude.md) and timing limitations are all controlled.

## ↑ Ancestors (15)

1. [C](../c.md)
2. [D13](../../d13.md)
3. [Section D](../../../section-d.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
