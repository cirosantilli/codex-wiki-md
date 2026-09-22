<h1 id="d/4/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For fixed $n>0$, Tonelli gives

$$
\int_0^n\int_0^\infty |\sin x|e^{-tx}\,dt\,dx=\int_0^n\frac{|\sin x|}{x}\,dx<\infty,
$$

because the quotient is [bounded](../../../../../../boundedness.md) near zero. Fubini therefore permits reversing the order for this finite $x$ [interval](../../../../../../interval-mathematics.md). Direct integration in $x$ yields

$$
\int_0^n e^{-tx}\sin x\,dx=\frac{1-e^{-nt}(t\sin n+\cos n)}{1+t^2}.
$$

Thus the desired integral equals $\pi/2$ minus the integral of the exponential remainder. Its absolute value is at most

$$
\int_0^\infty e^{-nt}(t+1)\,dt=\frac1{n^2}+\frac1n\longrightarrow0.
$$

Consequently $\boxed{\lim_{n\to\infty}\int_0^n\sin x/x\,dx=\pi/2}$. The truncation is essential: Fubini is not being applied to an absolutely [integrable function](../../../../../../lebesgue-integrable-function.md) over the whole infinite rectangle.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [D](../../../../d.md)
5. [2008](../../../../../2008-split.md)
6. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../../split.md)
7. [Probability, statistics and options II course of the University of Oxford](../../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Mathematics and statistics course of the University of Oxford](../../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
