<h1 id="section-d/d12/solution">Solution</h1>

↑ **Parent:** [D12](../d12.md)

An [ideal operational amplifier](../../../../../ideal-operational-amplifier.md) has infinite differential open-loop gain, infinite [input impedance](../../../../../input-impedance.md), zero [output impedance](../../../../../output-impedance.md) and unlimited [bandwidth](../../../../../bandwidth-signal-processing.md) and output capability, and zero [input offset voltage](../../../../../input-offset-voltage.md) and [input bias current](../../../../../input-bias-current.md). In a stable negative-feedback circuit operating linearly, its input currents vanish and $V_-=V_+$. This equality is a feedback consequence, not a rule for a saturated or open-loop amplifier. Here the grounded non-inverting input makes the inverting node a virtual earth.

The [inverting two-pole band-pass filter](../../../../../inverting-two-pole-band-pass-filter.md) has a series [resistor](../../../../../resistor.md) and [capacitor](../../../../../capacitor.md) input, while the feedback arm is a parallel [resistor](../../../../../resistor.md) and [capacitor](../../../../../capacitor.md). With Laplace variable $s$,

$$
Z_{\rm in}=R_1+\frac1{sC_1},\qquad
Z_f=\frac{R_2}{1+sR_2C_2},\qquad
\boxed{H(s)=-\frac{Z_f}{Z_{\rm in}}=-K\frac{s\tau_1}{(1+s\tau_1)(1+s\tau_2)}},\quad K=R_2/R_1.
$$

[Kirchhoff's current law](../../../../../kirchhoff-node-law.md) at virtual earth gives the minus sign. Substituting $s=i\omega$ yields

$$
|H|^2=K^2\frac{\omega^2\tau_1^2}{(1-\omega^2\tau_1\tau_2)^2+\omega^2(\tau_1+\tau_2)^2}.
$$

It vanishes at zero and infinite [frequency](../../../../../frequency.md), with low-frequency $|H|^2\simeq(\omega R_2C_1)^2$ and high-frequency $|H|^2\simeq1/(\omega R_1C_2)^2$. Differentiation gives the single maximum

$$
\boxed{\omega_0=\frac1{\sqrt{\tau_1\tau_2}},\quad
|H|_{\max}=K\frac{\tau_1}{\tau_1+\tau_2}}.
$$

For $\tau_1\gg\tau_2$, the broad interval $1/\tau_1\ll\omega\ll1/\tau_2$ has $|H|\simeq R_2/R_1$. For $\tau_2\gg\tau_1$, the interval $1/\tau_2\ll\omega\ll1/\tau_1$ instead has $|H|\simeq C_1/C_2$. The same rising and falling asymptotes apply outside either plateau.

<a id="section-d/d12/image-original-ideal-filter-power-gains-for-different-time-constant-ratios-showing-the-finite-selectivity-limit"></a>
![](../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2013/paper-1-band-pass.png)

**[Figure 3](#section-d/d12/image-original-ideal-filter-power-gains-for-different-time-constant-ratios-showing-the-finite-selectivity-limit). Original ideal filter power gains for different time-constant ratios, showing the finite selectivity limit**.

Writing $a=\tau_1+\tau_2$ and $b=\tau_1\tau_2$, the half-power [frequencies](../../../../../frequency.md) and [quality factor](../../../../../q-factor.md) are

$$
\omega_\pm=\frac{\sqrt{a^2+4b}\pm a}{2b},\quad
\Delta\omega=\omega_+-\omega_-=\frac ab,\quad
\boxed{Q=\frac{\omega_0}{\Delta\omega}=\frac{\sqrt{\tau_1\tau_2}}{\tau_1+\tau_2}\le\frac12}.
$$

Equal time constants give the narrowest fractional pass-band achievable here, with $\omega_\pm=(\sqrt2\pm1)\omega_0$ and

$$
\boxed{|H|_{\max}=\frac{R_2}{2R_1}=\frac{C_1}{2C_2}\quad(\tau_1=\tau_2)}.
$$

**This topology cannot make a genuinely sharp, high-$Q$ band-pass.** Its [poles](../../../../../pole.md) are real, and the [selectivity bound for a two-real-pole band-pass](../../../../../selectivity-bound-for-a-two-real-pole-band-pass.md) prevents arbitrarily narrow selection. A more selective resonant filter needs additional circuit structure. The gain above answers the component-ratio question for the sharpest available setting without assuming an impossible limit.

Real amplifiers have finite frequency-dependent gain and phase lag, so virtual earth becomes inaccurate, the response changes and stability must be checked. Gain-bandwidth limits, [slew rate](../../../../../slew-rate.md) for large [signals](../../../../../signal.md), output loading and [amplifier saturation](../../../../../amplifier-saturation.md) also matter. Component tolerances move the corners; [capacitor](../../../../../capacitor.md) parasitics, stray [capacitance](../../../../../capacitance.md), [resistor](../../../../../resistor.md) [noise](../../../../../noise-signal-processing.md) and input [noise](../../../../../noise-signal-processing.md) become significant. The ideal high-frequency tail should not be extrapolated beyond the amplifier and lumped-component operating ranges.

## ↑ Ancestors (14)

1. [D12](../d12.md)
2. [Section D](../../section-d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
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
