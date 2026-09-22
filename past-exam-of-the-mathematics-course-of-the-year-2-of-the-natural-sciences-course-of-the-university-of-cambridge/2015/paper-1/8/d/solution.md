<h1 id="8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

If $N=|n|$ is an integer, the recurrence has zero numerator at $j=N$. Choosing the parity containing $a_N$ therefore makes all later coefficients vanish. Conversely, for a nonzero polynomial of degree $N$, the coefficient of $x^N$ in the differential equation is $(n^2-N^2)a_N$, so $n^2=N^2$ is necessary.

Normalizing the terminating series by $y(1)=1$ gives the first [Chebyshev polynomials](../../../../../chebyshev-polynomial.md):

$$
\boxed{T_0(x)=1,\qquad T_1(x)=x,\qquad T_2(x)=2x^2-1,\qquad T_3(x)=4x^3-3x.}
$$

Substitution verifies each differential equation and endpoint value. More generally, $T_N(x)=\cos(N\arccos x)$; its recurrence $T_{N+1}=2xT_N-T_{N-1}$ also establishes polynomiality and the normalization.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [8](../../8.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
