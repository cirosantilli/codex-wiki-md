<h1 id="d/d3/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For $0<x<1$, expand $(1-x)^{-2}=\sum_{k\ge1}kx^{k-1}$. All terms after multiplication by $(\log x)^2$ are nonnegative, so [monotone convergence](../../../../../monotone-convergence-theorem.md) permits integration term by term. Substituting $x=e^{-t}$ and integrating by parts twice gives

$$
\int_0^1x^{k-1}(\log x)^2dx=\int_0^\infty e^{-kt}t^2dt=\frac2{k^3}.
$$

Consequently the integral is $\sum_{k\ge1}2/k^2$, and the supplied sum gives $\boxed{\pi^2/3}$.

## ↑ Ancestors (13)

1. [2](../2.md)
2. [D3](../../d3.md)
3. [D](../../../d.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
