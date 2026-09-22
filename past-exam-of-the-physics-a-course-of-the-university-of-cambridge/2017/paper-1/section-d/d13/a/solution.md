<h1 id="section-d/d13/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Electrical noise reduction](../../../../../../electrical-noise-reduction.md) starts by identifying what is unwanted in the measured [signal](../../../../../../signal.md) and where it enters. Increasing gain amplifies both [signal](../../../../../../signal.md) and input [noise](../../../../../../noise-signal-processing.md); it does not by itself improve the input [signal-to-noise ratio](../../../../../../signal-to-noise-ratio.md). Separate intrinsic component fluctuations, [amplifier](../../../../../../amplifier.md) [noise](../../../../../../noise-signal-processing.md) and external pickup before choosing a remedy.

**Physical sources.** A [resistor](../../../../../../resistor.md) at [temperature](../../../../../../temperature-split.md) $T$ has classical one-sided open-circuit [thermal electrical noise](../../../../../../thermal-electrical-noise.md) density $S_V=4k_BTR$ per hertz. In a flat measurement bandwidth $B$, its rms voltage is $\sqrt{4k_BTRB}$. Lowering an appropriate resistance, reducing [temperature](../../../../../../temperature-split.md) or narrowing the useful bandwidth can reduce this [noise](../../../../../../noise-signal-processing.md), with loading and signal-gain tradeoffs considered. These are [power spectral densities](../../../../../../power-spectral-density.md); an [amplitude spectral density](../../../../../../amplitude-spectral-density.md) is their square root.

Discrete independent charge transfers give [shot noise](../../../../../../shot-noise.md), with one-sided current density $S_I=2eI$ in the simple [Poisson process](../../../../../../poisson-process-split.md) model. Reducing leakage or unwanted bias current can help, but reducing a [photocurrent](../../../../../../photocurrent.md) may also reduce the desired [signal](../../../../../../signal.md). Charge correlations can change the simple shot-noise law. At low [frequency](../../../../../../frequency.md), [flicker noise](../../../../../../flicker-noise.md) and drift often dominate and are not described by a white spectrum.

**[Amplifier](../../../../../../amplifier.md) and impedance choice.** An [operational amplifier](../../../../../../operational-amplifier.md) has equivalent input voltage and current [noise](../../../../../../noise-signal-processing.md). In a simplified uncorrelated model, a resistive source contributes the input-referred voltage density

$$
S_{V,\rm eq}\simeq e_n^2+4k_BTR_s+i_n^2|Z_s|^2.
$$

Here $e_n,i_n$ are the voltage and current amplitude spectral densities and $Z_s$ is the source [electrical impedance](../../../../../../electrical-impedance.md); feedback components add further terms in a full circuit. Low current [noise](../../../../../../noise-signal-processing.md) matters particularly for a high-impedance source, while voltage [noise](../../../../../../noise-signal-processing.md) can dominate for a low-impedance source. Minimize needless source impedance, leakage and long sensitive connections without sacrificing the required transduction gain or bandwidth. Bias-current offsets and thermal drift also require calibration; they are not removed simply by quoting a random-noise density.

**Pickup and bandwidth.** Shield sensitive circuits against electric-field coupling, minimize loop area to reduce changing magnetic-flux pickup, and use twisted signal/return pairs or suitable coaxial connections. Differential readout rejects common-mode interference when impedances and [amplifier](../../../../../../amplifier.md) responses are adequately matched. Plan the [signal](../../../../../../signal.md) returns to avoid unwanted circulating ground currents, and decouple supply rails locally so supply fluctuations do not enter the [signal](../../../../../../signal.md) path. Mechanical vibration, cable motion and [temperature](../../../../../../temperature-split.md) changes may be converted into electrical [noise](../../../../../../noise-signal-processing.md) as well.

A [low-pass filter](../../../../../../low-pass-filter.md) removes out-of-band [noise](../../../../../../noise-signal-processing.md) before digitization; an [anti-aliasing filter](../../../../../../anti-aliasing-filter.md) is needed because digital filtering cannot undo already aliased content. Avoid a narrower passband than the physical [signal](../../../../../../signal.md) requires. For a known periodic [signal](../../../../../../signal.md), modulation and a [lock-in amplifier](../../../../../../lock-in-amplifier.md) select a narrow [frequency](../../../../../../frequency.md) interval, often moving the measurement above a strong [flicker noise](../../../../../../flicker-noise.md) region. A notch can reject a narrow interference line if that does not remove essential [signal](../../../../../../signal.md) information.

Independent [noise](../../../../../../noise-signal-processing.md) contributions add in [variance](../../../../../../variance-split.md), not directly in rms amplitude. Averaging $N$ independent equal-variance readings reduces the [standard error](../../../../../../standard-error.md) by $N^{-1/2}$, but slow correlated drift and [systematic errors](../../../../../../systematic-error.md) need separate controls. **Good [noise](../../../../../../noise-signal-processing.md) reduction preserves the information-bearing [signal](../../../../../../signal.md) while reducing unwanted coupling, intrinsic fluctuations or the admitted [noise](../../../../../../noise-signal-processing.md) bandwidth.**

## ↑ Ancestors (15)

1. [A](../a.md)
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
