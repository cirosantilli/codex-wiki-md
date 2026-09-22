<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The non-inverting input is grounded, so the finite [voltage gain](../../../../voltage-gain.md) gives $V_{\rm OUT}=-AV^-$, or $V^-=-V_{\rm OUT}/A$. Infinite [input impedance](../../../../input-impedance.md) makes [Kirchhoff's current law](../../../../kirchhoff-node-law.md) at the inverting input

$$
\frac{V_{\rm IN}-V^-}{R_1}+\frac{V_{\rm OUT}-V^-}{R_2}=0.
$$

Substitute $V^-=-V_{\rm OUT}/A$ and multiply by $R_1R_2$:

$$
R_2V_{\rm IN}+\left(R_1+\frac{R_1+R_2}{A}\right)V_{\rm OUT}=0.
$$

Hence the [inverting operational amplifier](../../../../inverting-operational-amplifier.md) has

$$
\boxed{\frac{V_{\rm OUT}}{V_{\rm IN}}=-\frac{R_2}{R_1+(R_1+R_2)/A},\qquad B=\frac{R_1+R_2}{A}.}
$$

As $A\to\infty$, the [voltage gain](../../../../voltage-gain.md) tends to $-R_2/R_1$. Setting $V^-=0$ before taking that limit would discard precisely the correction being calculated.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
