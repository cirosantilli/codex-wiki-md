<h1 id="12/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Subtract the integrands first, using $\cos u-\cos^3u=\cos u\sin^2u$. Then set $s=\sin u$:

$$
I_{n,1}(\pi/2,0)-I_{n,3}(\pi/2,0)
=\int_0^1s^2(1-s^3)^n\,ds.
$$

The further [integration by substitution](../../../../../integration-by-substitution.md) $w=s^3$ makes $dw=3s^2ds$, so

$$
\boxed{I_{n,1}(\pi/2,0)-I_{n,3}(\pi/2,0)
=\frac13\int_0^1(1-w)^n\,dw=\frac1{3(n+1)}}.
$$

This also holds at $n=0$.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [12](../../12.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
