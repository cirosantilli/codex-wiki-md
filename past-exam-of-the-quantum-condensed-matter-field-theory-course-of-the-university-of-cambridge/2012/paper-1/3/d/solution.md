<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Analytically continue the supplied free propagator using $M=I$ and $t=-i\hbar\beta$. This gives $Z_0=\sqrt{I/(2\pi\hbar^2\beta)}$ without an arbitrary measure constant.

Apply the [Poisson summation formula](../../../../../poisson-summation-formula.md) to $h(x)=e^{-Ax^2}$, with $A=2\pi^2I/(\hbar^2\beta)$. Its [Gaussian integral](../../../../../gaussian-integral.md) is

$$
\int_{-\infty}^\infty dx\,e^{-Ax^2+2\pi inx}=\sqrt{\frac\pi A}\,e^{-\pi^2n^2/A}.
$$

The prefactors cancel exactly because $2\pi Z_0\sqrt{\pi/A}=1$. Therefore the [momentum-winding duality of the quantum rotor](../../../../../momentum-winding-duality-of-the-quantum-rotor.md) gives

$$
\boxed{2\pi Z_0\sum_me^{-Am^2}=\sum_ne^{-\beta\hbar^2n^2/(2I)},}
$$

in agreement with the spectrum. The [thermal winding dominance of a free rotor](../../../../../thermal-winding-dominance-of-a-free-rotor.md) interchanges between the two representations. At low temperature the momentum sum is dominated by n=0 and $Z\to1$. At high temperature the winding sum is dominated by m=0 and $Z\sim\sqrt{2\pi I/(\beta\hbar^2)}$, the classical angular phase-space integral. Winding and momentum labels are dual descriptions; keeping only m=0 at low temperature would be incorrect.

## ↑ Ancestors (14)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the quantum Condensed Matter Field Theory course of the University of Cambridge](../../../../split.md)
6. [Quantum Condensed Matter Field Theory course of the University of Cambridge](../../../../../quantum-condensed-matter-field-theory-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
