<h1 id="19/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume $\alpha<\beta$ and abbreviate

$$
A=\int_\alpha^\beta f^2\,dx,\qquad B=\int_\alpha^\beta fg\,dx,\qquad C=\int_\alpha^\beta g^2\,dx.
$$

The [integral](../../../../../integral-split.md) of the nonnegative square expands to $A+2\lambda B+\lambda^2C\geq0$ for every real $\lambda$. If $C>0$, completing the square, or choosing $\lambda=-B/C$, gives $A-B^2/C\geq0$. Hence the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) is

$$
\boxed{\left(\int_\alpha^\beta fg\,dx\right)^2
\leq\left(\int_\alpha^\beta f^2\,dx\right)
\left(\int_\alpha^\beta g^2\,dx\right)}.
$$

If $C=0$, [continuity](../../../../../continuous-function.md) and nonnegativity imply $g=0$ throughout the interval, so the same inequality is immediate.

When $C>0$, equality holds exactly when $\int(f-(B/C)g)^2dx=0$. The [integrand](../../../../../integrand.md) is continuous and nonnegative, so it must vanish everywhere, giving $f=(B/C)g$. Including the case of a zero [function](../../../../../function-split.md), equality is equivalent to [linear dependence](../../../../../linear-dependence.md) of $f$ and $g$ as elements of the real [vector space](../../../../../vector-space-split.md) of continuous [functions](../../../../../function-split.md) on the interval.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [19](../../19.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
