<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the same [Fourier transform](../../../../../fourier-transform-split.md) convention, now in the sense of [tempered distributions](../../../../../tempered-distribution.md), since the homogeneous oscillations are not integrable. Transforming gives

$$
\bigl[q^2-(\omega+r)^2\bigr]\widetilde\phi(\omega)=0.
$$

Since $q>0$, the two roots are distinct. A [distribution](../../../../../distribution-mathematical-analysis.md) annihilated by this polynomial is a linear combination of [Dirac delta distributions](../../../../../dirac-delta-function.md) at its roots:

$$
\widetilde\phi(\omega)=2\pi A\delta(\omega+r-q)+2\pi B\delta(\omega+r+q).
$$

[Fourier inversion](../../../../../fourier-inversion-theorem.md) therefore gives

$$
\boxed{\phi(t)=A e^{i(q-r)t}+B e^{-i(q+r)t}
=e^{-irt}\bigl(C\cos qt+D\sin qt\bigr).}
$$

The constants may be complex. Differentiating the factor $e^{-irt}$ also verifies that the original [ordinary differential equation](../../../../../ordinary-differential-equation.md) reduces to $\ddot\psi+q^2\psi=0$ for $\phi=e^{-irt}\psi$.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
