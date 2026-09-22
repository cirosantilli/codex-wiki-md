<h1 id="section-a/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

[negative feedback](../../../../../negative-feedback.md) and the ideal [operational amplifier](../../../../../operational-amplifier.md)'s [virtual short](../../../../../virtual-short.md) hold the inverting node at zero potential, with no current entering either input. The parallel feedback [resistor](../../../../../resistor.md) and [capacitor](../../../../../capacitor.md) have [electrical impedance](../../../../../electrical-impedance.md)

$$
Z_f=\left(R_f^{-1}+i\omega C\right)^{-1}
=\frac{R_f}{1+i\omega R_fC}.
$$

[Kirchhoff's current law](../../../../../kirchhoff-node-law.md) at the inverting node gives $V_{\rm in}/R_i=-V_{\rm out}/Z_f$. For the component values read from the circuit,

$$
G(f)=\frac{V_{\rm out}}{V_{\rm in}}
=-\frac{1000}{1+i\,2\pi f(1\,\mathrm s)},\qquad
\boxed{|G(f)|=\frac{1000}{\sqrt{1+(f/0.15915\,\mathrm{Hz})^2}}}.
$$

This [inverting low-pass amplifier](../../../../../inverting-low-pass-amplifier.md) has a DC gain magnitude of 1000 and [cutoff frequency](../../../../../cutoff-frequency.md) $f_c=(2\pi R_fC)^{-1}=0.15915$ Hz. At the corner, $|G|=707.1$. Above it the gain approaches $1/(2\pi fR_iC)=159.15/f$, with $f$ in Hz: a slope of $-1$ on logarithmic axes, or $-20$ dB per decade on a [Bode plot](../../../../../bode-plot.md). At $0.01,1,10,100$ Hz the magnitudes are approximately $998,157.2,15.91,1.592$. These are voltage ratios, not [decibels](../../../../../decibel.md).

<a id="section-a/5/image-calculated-magnitude-response-of-the-inverting-low-pass-amplifier"></a>
![](../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2015/paper-1-amplifier-gain.png)

**[Figure 2](#section-a/5/image-calculated-magnitude-response-of-the-inverting-low-pass-amplifier). Calculated magnitude response of the inverting low-pass amplifier**.

## ↑ Ancestors (14)

1. [5](../5.md)
2. [Section A](../../section-a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
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
