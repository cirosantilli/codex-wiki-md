<h1 id="section-d/d13/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In an [operational-amplifier negative feedback](../../../../../../operational-amplifier-negative-feedback.md) loop, an [operational amplifier](../../../../../../operational-amplifier.md) has large [open-loop gain](../../../../../../open-loop-gain.md) $A$, with $V_o=A(V_+-V_-)$. Feeding a fraction $\beta V_o$ back to the inverting input opposes an output increase. For a non-inverting [signal](../../../../../../signal.md) input,

$$
\boxed{\frac{V_o}{V_i}=\frac A{1+A\beta}\simeq\frac1\beta\quad\text{when }|A\beta|\gg1.}
$$

Its sensitivity to [open-loop gain](../../../../../../open-loop-gain.md) changes is reduced by $d\ln A_{\rm cl}/d\ln A=1/(1+A\beta)$. Thus [resistor](../../../../../../resistor.md) ratios can set a reproducible gain despite device variation; feedback also suppresses internal distortion and reduces [output impedance](../../../../../../output-impedance.md). Gain is traded for usable [bandwidth](../../../../../../bandwidth-signal-processing.md), subject to the amplifier's [frequency](../../../../../../frequency.md) response.

For the non-inverting connection, place $R_f$ between output and inverting input and $R_g$ between that input and ground. Then $\beta=R_g/(R_f+R_g)$, giving gain $1+R_f/R_g$. For an inverting connection, ground the non-inverting input, inject the [signal](../../../../../../signal.md) through $R_{\rm in}$ and return $R_f$ from output to the inverting [node](../../../../../../node-dynamical-systems.md). Small differential input and negligible input current then give gain $-R_f/R_{\rm in}$. The near-zero [node](../../../../../../node-dynamical-systems.md) is a [virtual ground](../../../../../../virtual-ground.md), not a physical ground connection.

The feedback must remain stable at the [frequencies](../../../../../../frequency.md) where [loop gain](../../../../../../loop-gain.md) matters. Extra phase lag can turn the intended opposition into oscillation; adequate [phase margin](../../../../../../phase-margin.md), supply headroom, input common-mode range, output-current capability and [slew rate](../../../../../../slew-rate.md) are required. Feedback neither prevents clipping nor removes all input [noise](../../../../../../noise-signal-processing.md).[Chapter 3, §§3.2.2–3.2.4, gain stability, loop gain and frequency dependence](../../../../../../operational-amplifier-negative-feedback-by-analog-devices.md)

## ↑ Ancestors (15)

1. [A](../a.md)
2. [D13](../../d13.md)
3. [Section D](../../../section-d.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2014](../../../../split.md)
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
