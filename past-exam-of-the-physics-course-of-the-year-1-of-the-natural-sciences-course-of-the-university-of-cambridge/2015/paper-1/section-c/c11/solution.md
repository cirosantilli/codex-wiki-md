<h1 id="section-c/c11/solution">Solution</h1>

↑ **Parent:** [C11](../c11.md)

Use $e^{i\omega t}$ [phasors](../../../../../phasor.md). The relation $V=L\dot I$ gives $Z_L=i\omega L$. The three branches form a [parallel RLC circuit](../../../../../parallel-rlc-circuit.md) and share the source [voltage](../../../../../voltage.md). The source-current [phasor](../../../../../phasor.md) and its real time dependence are

$$
\widetilde I_{\rm total}=V_0\left[\frac1R+i\left(\omega C-\frac1{\omega L}\right)\right],
$$



$$
I_{\rm total}(t)=V_0\left[\frac{\cos\omega t}{R}-\left(\omega C-\frac1{\omega L}\right)\sin\omega t\right].
$$

Consequently its [amplitude](../../../../../wave-amplitude.md) is $V_0\sqrt{R^{-2}+(\omega C-1/(\omega L))^2}$ and its [phase](../../../../../phase-waves.md) relative to the [voltage](../../../../../voltage.md) is $\tan^{-1}[R(\omega C-1/(\omega L))]$. At low [frequency](../../../../../frequency.md) it is inductive and lags toward $-\pi/2$; at high [frequency](../../../../../frequency.md) it is capacitive and leads toward $+\pi/2$. The ideal [amplitude](../../../../../wave-amplitude.md) diverges at either extreme and has a finite minimum between them; real component losses and source [electrical impedance](../../../../../electrical-impedance.md) limit those asymptotes.

<a id="section-c/c11/image-original-normalized-source-current-amplitude-phase-and-resistor-to-source-current-ratio-for-an-illustrative-ideal-parallel-rlc-circuit"></a>
![](../../../../../past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1-parallel-resonance.png)

**[Figure 3](#section-c/c11/image-original-normalized-source-current-amplitude-phase-and-resistor-to-source-current-ratio-for-an-illustrative-ideal-parallel-rlc-circuit). Original normalized source-current amplitude, phase and resistor-to-source-current ratio for an illustrative ideal parallel RLC circuit**.

Zero [phase](../../../../../phase-waves.md) requires cancellation of [electrical susceptances](../../../../../electrical-susceptance.md):

$$
\boxed{\omega_{\rm res}=\frac1{\sqrt{LC}},\qquad|I_{\rm total}|_{\rm res}=\frac{V_0}{R}\quad\text{(minimum)}.}
$$

The [inductor](../../../../../inductor.md) and [capacitor](../../../../../capacitor.md) currents are nonzero, equal in magnitude and opposite in [phase](../../../../../phase-waves.md), while the [resistor](../../../../../resistor.md) supplies the in-phase source current. [energy](../../../../../energy-split.md) oscillates between the reactive elements; dissipation occurs in the shunt [resistor](../../../../../resistor.md). A source-current maximum would describe a different, series-resonant circuit.

The specified ratio is

$$
\frac{|I_R|}{|I_{\rm total}|}=\frac1{\sqrt{1+R^2(\omega C-1/(\omega L))^2}}.
$$

It exceeds $1/\sqrt2$ when $|\omega C-1/(\omega L)|<1/R$. Define $b=1/(RC)$ and $\omega_0=1/\sqrt{LC}$. The two positive endpoints are $\omega_\pm=[\sqrt{b^2+4\omega_0^2}\pm b]/2$, so

$$
\boxed{\delta\omega=\omega_+-\omega_-=\frac1{RC},\qquad Q=\frac{\omega_0}{\delta\omega}=R\sqrt{\frac CL}.}
$$

The endpoints have geometric mean $\omega_0$. Increasing the parallel resistance reduces dissipative loading and narrows this band, in contrast with increasing the resistance of a [series RLC circuit](../../../../../series-rlc-circuit.md). Equivalently, $Q=\omega_0U_{\max}/P_{\rm loss}$, with $U_{\max}=CV_0^2/2$ and $P_{\rm loss}=V_0^2/(2R)$. The [parallel RLC bandwidth](../../../../../parallel-rlc-bandwidth.md) here belongs to the explicitly defined current ratio, not a half-maximum rule applied to a source-current peak that does not exist.

## ↑ Ancestors (13)

1. [C11](../c11.md)
2. [Section C](../../section-c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
