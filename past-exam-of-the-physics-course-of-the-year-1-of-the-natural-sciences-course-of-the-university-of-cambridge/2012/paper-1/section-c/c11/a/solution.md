<h1 id="section-c/c11/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In sinusoidal [steady state](../../../../../../steady-state.md), [complex impedance](../../../../../../electrical-impedance.md) is the [voltage](../../../../../../voltage.md) [phasor](../../../../../../phasor.md) divided by the current [phasor](../../../../../../phasor.md). Its [modulus](../../../../../../modulus.md) is the [amplitude](../../../../../../wave-amplitude.md) ratio and its [argument](../../../../../../argument-complex-analysis.md) is the [voltage](../../../../../../voltage.md) lead. With the $e^{i\omega t}$ convention, $I=dq/dt=i\omega CV$, so **$Z_C=1/(i\omega C)$**.

The PDF labels $V_1$ across $R_1$, not across the complete driven network. If $I$ is the current through $R_1$, then $V_1=IR_1$ and $I=Y_pV_2$, where

$$
Y_p=\frac1R+i\left(\omega C-\frac1{\omega L}\right).
$$

The [resistor-referenced parallel-resonator response](../../../../../../resistor-referenced-parallel-resonator-response.md) is

$$
\boxed{H(\omega)=\frac{V_2}{V_1}=\frac{R/R_1}{1+iR(\omega C-1/(\omega L))}.}
$$

Writing $b(\omega)=\omega C-1/(\omega L)$,

$$
|H|=\frac{R/R_1}{\sqrt{1+R^2b^2}},\qquad
\arg H=-\tan^{-1}(Rb).
$$

The maximum occurs at $\omega_0=1/\sqrt{LC}$, where **$|H|=R/R_1$ and the [phase](../../../../../../phase-waves.md) is zero**. Below [resonance](../../../../../../resonance.md) the [phase](../../../../../../phase-waves.md) is positive, tending to $+\pi/2$; above it the [phase](../../../../../../phase-waves.md) is negative, tending to $-\pi/2$. The [amplitude](../../../../../../wave-amplitude.md) tends to zero at both extremes: the [inductor](../../../../../../inductor.md) shorts the parallel network at low [frequency](../../../../../../frequency.md), and the [capacitor](../../../../../../capacitor.md) does so at high [frequency](../../../../../../frequency.md). At [resonance](../../../../../../resonance.md) their reactive currents cancel, leaving only the [resistor](../../../../../../resistor.md) current.

<a id="section-c/c11/a/image-resistor-referenced-parallel-resonator-amplitude-and-phase-normalized-without-choosing-circuit-component-values"></a>
![](../../../../../../past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1-ia2012-parallel-response.png)

**[Figure 2](#section-c/c11/a/image-resistor-referenced-parallel-resonator-amplitude-and-phase-normalized-without-choosing-circuit-component-values). Resistor-referenced parallel-resonator amplitude and phase, normalized without choosing circuit component values**.

If instead $V_{\rm in}$ denotes the [voltage](../../../../../../voltage.md) across the complete circuit, its different transfer ratio is $V_2/V_{\rm in}=1/[1+R_1/R+iR_1b]$, with peak $R/(R+R_1)$. This distinction follows directly from the printed [voltage](../../../../../../voltage.md) endpoints.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [C11](../../c11.md)
3. [Section C](../../../section-c.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2012](../../../../split.md)
6. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
