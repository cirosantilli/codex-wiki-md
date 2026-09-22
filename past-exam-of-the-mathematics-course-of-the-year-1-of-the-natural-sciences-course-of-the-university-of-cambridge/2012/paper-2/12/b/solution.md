<h1 id="12/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $s=\sin u$, so $ds=\cos u\,du$, and write $J_n=I_{n,1}(\pi/2,0)$. The [integration by substitution](../../../../../integration-by-substitution.md) gives $J_n=\int_0^1(1-s^3)^n\,ds$. For $n>0$, [integration by parts](../../../../../integration-by-parts.md) yields

$$
J_n=[s(1-s^3)^n]_0^1+3n\int_0^1s^3(1-s^3)^{n-1}\,ds.
$$

Both endpoint terms vanish. Use $s^3=1-(1-s^3)$ inside the remaining [integral](../../../../../integral-split.md):

$$
J_n=3n(J_{n-1}-J_n).
$$

Consequently

$$
\boxed{I_{n,1}(\pi/2,0)=\frac{3n}{3n+1}I_{n-1,1}(\pi/2,0),\qquad
f(n)=\frac{3n}{3n+1}}.
$$

This is the $p=3$ instance of the [power-complement integral recurrence](../../../../../power-complement-integral-recurrence.md), with initial value $J_0=1$.

## ↑ Ancestors (13)

1. [B](../b.md)
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
