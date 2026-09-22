<h1 id="section-d/d13/solution">Solution</h1>

↑ **Parent:** [D13](../d13.md)

An [ideal operational amplifier](../../../../../ideal-operational-amplifier.md) draws no current at either input. With stable [operational-amplifier negative feedback](../../../../../operational-amplifier-negative-feedback.md) in its unsaturated linear range, infinite [open-loop gain](../../../../../open-loop-gain.md) also gives a [virtual short](../../../../../virtual-short.md), $V_+=V_-$. The amplifier adjusts its output to enforce that equality; it is not a conducting connection between the inputs. Here $V_+=0$, so the ideal summing node is a [virtual ground](../../../../../virtual-ground.md). [Kirchhoff's current law](../../../../../kirchhoff-node-law.md) gives $V_{\rm in}/R_1=-V_{\rm out}/R_2$, hence **the ideal gain is $-R_2/R_1$**.

For the [finite-input-resistance inverting amplifier](../../../../../finite-input-resistance-inverting-amplifier.md) let the inverting-node [voltage](../../../../../voltage.md) be $v$, and continue to neglect [output impedance](../../../../../output-impedance.md). The controlled output and node-current balance are

$$
V_{\rm out}=-Av,\qquad
\frac{v-V_{\rm in}}{R_1}+\frac{v-V_{\rm out}}{R_2}+\frac{v}{R_{\rm in}}=0.
$$

Eliminating $v$ gives

$$
\boxed{\frac{V_{\rm out}}{V_{\rm in}}
=-\frac{R_2/R_1}{1+\dfrac1A\left(1+\dfrac{R_2}{R_1}+\dfrac{R_2}{R_{\rm in}}\right)}}.
$$

Dividing the denominator by $R_2$ gives the requested resistance-sum form. The ideal result follows whenever $|A|\gg 1+R_2/R_1+R_2/R_{\rm in}$; taking $R_{\rm in}\to\infty$ alone is insufficient if $A$ is small. At finite [frequency](../../../../../frequency.md) $A$ and the gain are [phasor](../../../../../phasor.md) ratios, subject to feedback stability.

With equal [resistors](../../../../../resistor.md) and sufficiently large loop gain, **$V_{\rm out}\simeq -V_{\rm in}$**. This gives a controlled sign reversal or 180-degree [phase](../../../../../phase-waves.md) inversion, useful for subtraction and opposite-phase signal paths, with amplitude set by a [resistor](../../../../../resistor.md) ratio rather than uncertain [open-loop gain](../../../../../open-loop-gain.md). The source still sees approximately $R_1$, so this is not a high-input-impedance [voltage](../../../../../voltage.md) follower. For the ideal-input, single-pole model, the [noise gain of an operational amplifier](../../../../../noise-gain-of-an-operational-amplifier.md) is two and the closed-loop [bandwidth](../../../../../bandwidth-signal-processing.md) is approximately half the [gain-bandwidth product](../../../../../gain-bandwidth-product.md). Output swing, [slew rate](../../../../../slew-rate.md) and load constraints must also permit linear operation.

## ↑ Ancestors (14)

1. [D13](../d13.md)
2. [Section D](../../section-d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2011](../../../split.md)
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
