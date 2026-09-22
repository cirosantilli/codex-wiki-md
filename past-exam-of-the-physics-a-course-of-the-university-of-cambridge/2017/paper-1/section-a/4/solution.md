<h1 id="section-a/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use an [inverting operational amplifier](../../../../../inverting-operational-amplifier.md). Ground the non-inverting input, connect the source to the inverting input through $R_{\rm in}$, and connect $R_f$ from the output back to that same input.

<a id="section-a/4/image-an-ideal-inverting-amplifier-with-10-kilohm-input-resistance-and-100-kilohm-feedback-resistance"></a>
![](../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-1-q4-inverting-amplifier.png)

**[Figure 2](#section-a/4/image-an-ideal-inverting-amplifier-with-10-kilohm-input-resistance-and-100-kilohm-feedback-resistance). An ideal inverting amplifier with 10 kilohm input resistance and 100 kilohm feedback resistance**.

In linear operation the ideal [operational amplifier](../../../../../operational-amplifier.md) draws no input [electric current](../../../../../electric-current.md), and feedback holds the inverting input at the same [electric potential](../../../../../electric-potential.md) as the grounded non-inverting input. This node is a [virtual ground](../../../../../virtual-ground.md). [Kirchhoff's current law](../../../../../kirchhoff-node-law.md) there gives

$$
\frac{V_i}{R_{\rm in}}+\frac{V_o}{R_f}=0,
\qquad
\frac{V_o}{V_i}=-\frac{R_f}{R_{\rm in}}.
$$

The source supplies current $I_i=V_i/R_{\rm in}$, so its [input impedance](../../../../../input-impedance.md) is $R_{\rm in}$. The required design is therefore

$$
\boxed{R_{\rm in}=10\,\mathrm{k\Omega},\qquad R_f=100\,\mathrm{k\Omega},
\qquad V_o=-10V_i.}
$$

Only these two [resistors](../../../../../resistor.md) and the single ideal [operational amplifier](../../../../../operational-amplifier.md) are needed in the [signal](../../../../../signal.md) circuit; its power supplies are implicit. The result assumes an input small enough to keep the output within its linear operating range.

## ↑ Ancestors (14)

1. [4](../4.md)
2. [Section A](../../section-a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2017](../../../split.md)
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
