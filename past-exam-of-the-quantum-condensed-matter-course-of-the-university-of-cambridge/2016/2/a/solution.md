<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [junction field-effect transistor](../../../../junction-field-effect-transistor.md) has a conducting channel between source and drain, with gate regions forming reverse-biased [p-n junctions](../../../../p-n-junction.md) to that channel. In an n-channel device, a more negative gate-source [electric potential difference](../../../../electric-potential-difference.md) increases the [reverse bias](../../../../reverse-bias.md) and widens the [depletion region](../../../../depletion-region.md). The conducting cross-section shrinks, reducing the drain [electric current](../../../../electric-current.md). The gate ideally draws only a small leakage [electric current](../../../../electric-current.md), giving a high input resistance; the source-drain supply provides the controlled output [power](../../../../power.md). Carrier motion in a p-channel device reverses the relevant polarities.

At small positive $V_{DS}$, the channel conducts approximately as a resistor. As the potential rises from source to drain, the local gate-channel [reverse bias](../../../../reverse-bias.md) increases toward the drain. The depletion layers are therefore thicker there. For a symmetric n channel of half-thickness $a$, uniformly doped at density $N_D$, the one-sided [depletion approximation](../../../../depletion-approximation.md) gives

$$
w(y)\simeq\sqrt{\frac{2\varepsilon_s}{eN_D}\left[V_{\rm bi}+V(y)-V_{GS}\right]},
$$

where $w$ is the depletion width from each side and $V_{\rm bi}$ the built-in junction potential. The neutral channel closes locally when $w=a$. Define the positive geometrical depletion [electric potential difference](../../../../electric-potential-difference.md) $U_P=eN_Da^2/(2\varepsilon_s)$. The approximate drain-end pinch-off condition is

$$
\boxed{V_{DS,\rm sat}\simeq U_P-V_{\rm bi}+V_{GS}.}
$$

More negative gate bias makes this saturation occur at a smaller drain [electric potential difference](../../../../electric-potential-difference.md).

<a id="2/a/image-gate-depletion-drain-end-pinch-off-and-approximate-current-saturation-in-an-n-channel-jfet"></a>
![](../../../../past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2016-jfet-pinch-off.png)

**[Figure 2](#2/a/image-gate-depletion-drain-end-pinch-off-and-approximate-current-saturation-in-an-n-channel-jfet). Gate depletion, drain-end pinch-off and approximate current saturation in an n-channel JFET**.

[Pinch-off in a junction field-effect transistor](../../../../pinch-off-in-a-junction-field-effect-transistor.md) does **not** mean that the drain [electric current](../../../../electric-current.md) vanishes. [Electrons](../../../../electron.md) arriving through the remaining neutral channel are swept across the high-field depleted region into the drain. Further increases in $V_{DS}$ mostly fall across that region, so the [electric current](../../../../electric-current.md) changes only weakly: this is the saturation regime used for amplification. Channel shortening gives a finite output slope in real devices. Excessive reverse [electric potential difference](../../../../electric-potential-difference.md) eventually causes breakdown, beyond the normal saturation model.

A sufficiently negative gate [electric potential difference](../../../../electric-potential-difference.md) can instead deplete the entire channel from the source end and produce **cutoff**. In the simplified geometry its threshold is $V_{GS,\rm off}\simeq V_{\rm bi}-U_P<0$. A commonly used approximate transfer law in saturation is

$$
I_D\simeq I_{DSS}\left(1-\frac{V_{GS}}{V_{GS,\rm off}}\right)^2,\qquad V_{GS,\rm off}\leq V_{GS}\leq0.
$$

Here $I_{DSS}$ is the saturated drain [electric current](../../../../electric-current.md) at zero gate-source bias. The square law is a useful device approximation, not an exact result for arbitrary channel profiles. It connects field control of depletion to a measurable transfer characteristic while keeping drain-end pinch-off distinct from complete gate cutoff.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the quantum condensed matter course of the University of Cambridge](../../../split.md)
5. [Quantum Condensed Matter course of the University of Cambridge](../../../../quantum-condensed-matter-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
