<h1 id="17/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Two applications of [integration by parts](../../../../../integration-by-parts.md) lower the exponent by two. First, the sine boundary term vanishes:

$$
I_n=[x^{2n}\sin x]_0^\pi-2n\int_0^\pi x^{2n-1}\sin x\,dx
=-2n\int_0^\pi x^{2n-1}\sin x\,dx.
$$

For $n\ge1$, integrate the last expression once more:

$$
\int_0^\pi x^{2n-1}\sin x\,dx=[-x^{2n-1}\cos x]_0^\pi
+(2n-1)\int_0^\pi x^{2n-2}\cos x\,dx
=\pi^{2n-1}+(2n-1)I_{n-1}.
$$

Thus the [recurrence relation](../../../../../recurrence-relation.md) is

$$
\boxed{I_n=-2n\pi^{2n-1}-2n(2n-1)I_{n-1},\qquad n\ge1.}
$$

The starting value is $I_0=\int_0^\pi\cos x\,dx=0$. Successive applications give $I_1=-2\pi$ and $I_2=-4\pi^3+24\pi$, followed by

$$
\boxed{I_3=-6\pi^5+120\pi^3-720\pi.}
$$

## ↑ Ancestors (13)

1. [C](../c.md)
2. [17](../../17.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
