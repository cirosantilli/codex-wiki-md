<h1 id="section-d/d13/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In this digital-sampling context, Nyquist's theorem means the [Nyquist–Shannon sampling theorem](../../../../../../nyquist-shannon-sampling-theorem.md). A continuous [signal](../../../../../../signal.md) with no Fourier content outside $|f|\le B$ can be reconstructed from uniformly spaced samples taken sufficiently fast. The familiar practical condition is

$$
\boxed{f_s>2B,\qquad T_s=\frac1{f_s},\qquad f_N=\frac{f_s}{2}.}
$$

Here $f_N$ is the Nyquist [frequency](../../../../../../frequency.md), while $2B$ is the Nyquist rate required by that [signal](../../../../../../signal.md) bandwidth. A finite-energy bandlimited formulation allows equality; a rule intended to include arbitrary pure sinusoids at the boundary must be strict, because $\sin(\pi f_st)$ vanishes at every sampling time $t=n/f_s$.

The mechanism is visible in the [Fourier transform](../../../../../../fourier-transform-split.md). Sampling by a time comb creates shifted copies of the original spectrum, separated by $f_s$:

$$
x_s(t)=\sum_nx(nT_s)\delta(t-nT_s),\qquad
X_s(f)=f_s\sum_kX(f-kf_s).
$$

If those copies do not overlap, an ideal reconstruction filter selects one copy and recovers the original waveform. Equivalently, ideal interpolation uses the normalized [sinc function](../../../../../../sinc-function.md):

$$
\boxed{x(t)=\sum_{n=-\infty}^{\infty}x(nT_s)
\operatorname{sinc}\!\left(\frac{t-nT_s}{T_s}\right),\qquad
\operatorname{sinc}u=\frac{\sin\pi u}{\pi u}.}
$$

Each interpolation function is one at its own sample and zero at all other sample times. Exact reconstruction presumes the bandwidth condition, an ideal sampling clock and the full sample sequence.

If the spectrum extends beyond half the [sampling rate](../../../../../../sampling-rate.md), different continuous frequencies become indistinguishable: this is [aliasing](../../../../../../aliasing.md). A sinusoid at [frequency](../../../../../../frequency.md) $f$ is indistinguishable on the sampling grid from frequencies differing by integer multiples of $f_s$, with the usual sign reflection for real [signals](../../../../../../signal.md). For example, $10\,\mathrm{kHz}$ sampled at $8\,\mathrm{kS\,s^{-1}}$ aliases to $2\,\mathrm{kHz}$; a later digital filter cannot tell which [signal](../../../../../../signal.md) generated those samples.

Use an analogue [anti-aliasing filter](../../../../../../anti-aliasing-filter.md) before the [analogue-to-digital converter](../../../../../../analog-to-digital-converter.md) and choose a [sampling rate](../../../../../../sampling-rate.md) leaving room for its finite transition band. Faster sampling can relax that analogue filtering problem, but simply increasing the number of samples in a fixed-duration record does not improve the independent Fourier-bin spacing beyond approximately $1/T$. A long recording is needed for low-frequency resolution, while a small sampling interval is needed for high-frequency coverage. Finite records also introduce windowing and [spectral leakage](../../../../../../spectral-leakage.md).

Digitization adds amplitude quantization as well as time sampling. An ideal $N$-bit converter spanning voltage range $V_{\rm span}$ has step $\Delta=V_{\rm span}/2^N$. When quantization error may be modeled as independent and uniform across one step, its rms size is $\Delta/\sqrt{12}$; small coherent [signals](../../../../../../signal.md) need not obey that white-noise approximation. **[Sampling rate](../../../../../../sampling-rate.md) controls temporal ambiguity, recording duration controls [frequency](../../../../../../frequency.md) resolution, and converter resolution controls amplitude discretization.**

## ↑ Ancestors (15)

1. [B](../b.md)
2. [D13](../../d13.md)
3. [Section D](../../../section-d.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2017](../../../../split.md)
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
