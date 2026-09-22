<h1 id="section-d/d13/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Thermal agitation in a [resistor](../../../../../../resistor.md) produces **[Johnson-Nyquist noise](../../../../../../thermal-electrical-noise.md)**, even without an applied mean current. In the classical low-frequency regime, its one-sided open-circuit voltage spectrum is $S_V=4k_BTR$ and its equivalent short-circuit current spectrum is $S_I=4k_BT/R$. In an [Effective noise bandwidth](../../../../../../effective-noise-bandwidth.md) $B$,

$$
\boxed{v_{\rm rms}=\sqrt{4k_BTRB},\qquad i_{\rm rms}=\sqrt{4k_BTB/R}.}
$$

For a matched load, available thermal noise power is $k_BTB$. A [resistor](../../../../../../resistor.md) and load at the same [temperature](../../../../../../temperature-split.md) exchange noise power without a net heat flow.

Cooling reduces the rms amplitude as $\sqrt T$ if [Electrical resistance](../../../../../../electrical-resistance.md) and [bandwidth](../../../../../../bandwidth-signal-processing.md) remain fixed. A cryogenic bath or refrigerator, [thermal anchoring](../../../../../../thermal-anchoring.md) and controlled heat input can maintain a steady low [temperature](../../../../../../temperature-split.md). Radiation shields, an insulating [vacuum](../../../../../../vacuum.md), thermally anchored leads and limited measurement dissipation reduce heat leaks and self-heating. [Temperature](../../../../../../temperature-split.md) sensing and stable [feedback control](../../../../../../closed-loop-control.md) reduce slow temperature-induced drift; keeping [temperature](../../../../../../temperature-split.md) constant does not remove microscopic [thermal fluctuations](../../../../../../thermal-fluctuation.md).

<a id="section-d/d13/b/image-at-fixed-resistance-and-bandwidth-thermal-noise-power-scales-with-temperature-and-rms-amplitude-with-its-square-root"></a>
![](../../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2016/paper-1-thermal-noise.png)

**[Figure 7](#section-d/d13/b/image-at-fixed-resistance-and-bandwidth-thermal-noise-power-scales-with-temperature-and-rms-amplitude-with-its-square-root). At fixed resistance and bandwidth, thermal-noise power scales with temperature and rms amplitude with its square root**. [Source](paper-1-thermal-noise.py).

[Bandwidth](../../../../../../bandwidth-signal-processing.md) restriction, suitable impedance and a low-noise amplifier complement cooling. Warm leads, contacts and the amplifier can otherwise dominate the observed noise. At fixed mean current, [shot noise](../../../../../../shot-noise.md) is not generally reduced merely by cooling, and low-frequency excess noise need not follow the Johnson law. At frequencies with $hf\gtrsim k_BT$, quantum noise expressions replace the classical approximation.[Distinction between resistor thermal noise, amplifier noise and current-noise contributions](../../../../../../op-amp-noise-by-analog-devices.md)

## ↑ Ancestors (15)

1. [B](../b.md)
2. [D13](../../d13.md)
3. [Section D](../../../section-d.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2016](../../../../split.md)
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
