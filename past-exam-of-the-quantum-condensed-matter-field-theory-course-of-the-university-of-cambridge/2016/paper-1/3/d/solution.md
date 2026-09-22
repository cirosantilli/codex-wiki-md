<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Continue the [free-particle propagator](../../../../../free-particle-propagator.md) to $t=-i\mathcal T$ and replace its coordinate mass by the angular inertia $I$. The [Euclidean free-particle bridge amplitude](../../../../../euclidean-free-particle-bridge-amplitude.md) at coincident endpoints is

$$
\boxed{Z_0=\sqrt{\frac I{2\pi\hbar\mathcal T}}=\sqrt{\frac I{2\pi\hbar^2\beta}}.}
$$

This normalization includes the time-sliced [Gaussian measure](../../../../../gaussian-measure.md), not just a formal [determinant](../../../../../determinant.md) with an unspecified multiplicative constant. Set $A=2\pi^2I/(\hbar^2\beta)>0$. The correct [Poisson summation formula](../../../../../poisson-summation-formula.md) is $\sum_mF(m)=\sum_n\int_{-\infty}^{\infty}dx\,F(x)e^{-2\pi inx}$; the source PDF omits the integral sign before its $d\theta$. For $F(x)=e^{-Ax^2+i2\pi fx}$ the Gaussian Fourier integral gives

$$
\int_{-\infty}^{\infty}dx\,e^{-Ax^2+i2\pi(f-n)x}=\sqrt{\frac\pi A}\,e^{-\pi^2(n-f)^2/A}.
$$

The overall prefactor cancels exactly: $2\pi Z_0\sqrt{\pi/A}=1$, and $\pi^2/A=\beta\hbar^2/(2I)$. Hence

$$
\boxed{Z=\sum_n e^{-\beta\hbar^2(n-f)^2/(2I)},}
$$

in agreement with the angular-momentum [trace](../../../../../matrix-trace.md). Pairing $m$ and $-m$ makes the winding expression real, and the [momentum](../../../../../momentum-split.md) expression shows positivity. Both are periodic in flux and invariant under $f\mapsto-f$. At high [temperature](../../../../../temperature-split.md) the zero-winding term gives $Z\simeq\sqrt{2\pi I/(\beta\hbar^2)}$, with exponentially small flux dependence; at low [temperature](../../../../../temperature-split.md) the nearest integer angular-momentum state dominates, with two equal lowest terms at half-integer flux. These independent limits also check the normalization and the flux phase.

## ↑ Ancestors (14)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
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
