<h1 id="d/d4/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For fixed $n>0$, Tonelli and the allowed exponential integral give

$$
\int_0^n\int_0^\infty|\sin x|e^{-tx}\,dt\,dx=\int_0^n\frac{|\sin x|}x\,dx\leq n<\infty.
$$

The point $x=0$ is irrelevant to the integral. Fubini therefore permits reversing the signed integrals. Evaluating the elementary inner integral yields

$$
\int_0^n\frac{\sin x}x\,dx
=\int_0^\infty\frac{1-e^{-nt}(t\sin n+\cos n)}{1+t^2}\,dt.
$$

The first term has integral $\pi/2$. The absolute value of the remainder is at most

$$
\int_0^\infty e^{-nt}(t+1)\,dt=\frac1{n^2}+\frac1n\to0.
$$

Consequently **the improper integral tends to $\pi/2$**. The interchange was justified on each finite strip, without asserting absolute integrability on the infinite quadrant.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [D4](../../../d4.md)
4. [D](../../../../d.md)
5. [2008 printed variant](../../../../../2008-printed-variant-split.md)
6. [Past exam of the options II course of the University of Oxford](../../../../../split.md)
7. [Options II course of the University of Oxford](../../../../../../options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
