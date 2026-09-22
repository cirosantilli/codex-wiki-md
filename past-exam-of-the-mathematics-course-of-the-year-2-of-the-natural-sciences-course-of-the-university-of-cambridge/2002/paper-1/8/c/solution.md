<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

By [superposition](../../../../../superposition-principle.md), $y(x)=\int_1^eG(x,\xi)f(\xi)\,d\xi$. Split the [integral](../../../../../integral-split.md) at $\xi=x$: the portion $\xi>x$ uses the first branch of the [Green's function](../../../../../green-s-function-split.md), and the portion $\xi<x$ uses the second. This yields

$$
\boxed{y(x)=x\ln x\int_x^e(\ln\xi-1)f(\xi)\,d\xi+x(\ln x-1)\int_1^x\ln\xi f(\xi)\,d\xi.}
$$

For $f(\xi)=1/\xi$, put $t=\ln x$. The two [integrals](../../../../../integral-split.md) are

$$
\int_x^e\frac{\ln\xi-1}{\xi}\,d\xi=-\frac12-\frac{t^2}2+t,\qquad\int_1^x\frac{\ln\xi}{\xi}\,d\xi=\frac{t^2}2.
$$

Substitution and cancellation give

$$
\boxed{y(x)=\frac x2\bigl[(\ln x)^2-\ln x\bigr].}
$$

Indeed $y(1)=y(e)=0$. For a direct differential check,

$$
y'=\frac12(t^2+t-1),\qquad y''=\frac{2t+1}{2x},
$$

and therefore

$$
y''-\frac{y'}x+\frac y{x^2}=\frac{(2t+1)-(t^2+t-1)+(t^2-t)}{2x}=\frac1x.
$$

The homogeneous uniqueness shown in part (a) makes this the unique solution.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [8](../../8.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
