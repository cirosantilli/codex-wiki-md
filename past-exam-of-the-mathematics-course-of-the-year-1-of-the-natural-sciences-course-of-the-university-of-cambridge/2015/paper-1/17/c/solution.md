<h1 id="17/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First apply [integration by parts](../../../../../integration-by-parts.md) with $u=x^k$ and $dv=\sin x\,dx$:

$$
F(k)=\big[-x^k\cos x\big]_0^\pi
+k\int_0^\pi x^{k-1}\cos x\,dx
=\pi^k+k\int_0^\pi x^{k-1}\cos x\,dx.
$$

For $k>1$, integrate the remaining integral by parts once more. Its boundary term $[x^{k-1}\sin x]_0^\pi$ is zero, so

$$
\boxed{F(k)=\pi^k-k(k-1)F(k-2).}
$$

At $k=1$, direct [integration](../../../../../integral-split.md) gives $F(1)=\pi$, agreeing with the same formula; the coefficient of $F(-1)$ vanishes and that integral is finite. Now follow the odd chain:

$$
F(3)=\pi^3-6\pi,\qquad
\boxed{F(5)=\pi^5-20\pi^3+120\pi.}
$$

This is the [sine-weighted power integral recurrence](../../../../../sine-weighted-power-integral-recurrence.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [17](../../17.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
