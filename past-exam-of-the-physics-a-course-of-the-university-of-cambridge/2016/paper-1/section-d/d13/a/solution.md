<h1 id="section-d/d13/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The ideal voltage-feedback [Operational amplifier](../../../../../../operational-amplifier.md) has **zero input currents** and, while stable [negative feedback](../../../../../../negative-feedback.md) holds it in its linear operating range, **equal input voltages**: $i_+=i_-=0$ and $v_+=v_-$. The first rule follows from infinite [input impedance](../../../../../../input-impedance.md); the second is the large-open-loop-gain limit of $v_o=A(v_+-v_-)$. Equal input [electric potential](../../../../../../electric-potential.md) is a [virtual short](../../../../../../virtual-short.md), not an electrically conducting connection.

For an [inverting amplifier](../../../../../../inverting-amplifier.md) with the noninverting input grounded, $v_-=0$ and node-current balance gives $v_i/R_i=-v_o/R_f$, hence **$v_o=-R_fv_i/R_i$**. For a [noninverting amplifier](../../../../../../noninverting-amplifier.md), the feedback divider gives $v_-=v_oR_g/(R_f+R_g)=v_i$, hence **$v_o=(1+R_f/R_g)v_i$**.

<a id="section-d/d13/a/image-ideal-inverting-and-noninverting-negative-feedback-configurations"></a>
![](../../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2016/paper-1-op-amp-feedback.png)

**[Figure 6](#section-d/d13/a/image-ideal-inverting-and-noninverting-negative-feedback-configurations). Ideal inverting and noninverting negative-feedback configurations**. [Source](paper-1-op-amp-feedback.py).

One should check output swing, input common-mode range, [slew rate](../../../../../../slew-rate.md), [Gain-bandwidth product](../../../../../../gain-bandwidth-product.md) and stability before using these limits in a real circuit. Saturation, positive feedback or operation beyond [bandwidth](../../../../../../bandwidth-signal-processing.md) invalidates the equal-voltage rule; finite input bias currents and offset voltage can also matter.[University electronics course, Chapter 3: high-gain feedback assumptions and practical limits](../../../../../../operational-amplifier-negative-feedback-by-analog-devices.md)

## ↑ Ancestors (15)

1. [A](../a.md)
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
