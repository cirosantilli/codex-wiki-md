<h1 id="d/d3/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For $0<x<1$, expand $(1-x)^{-2}=\sum_{k\geq1}kx^{k-1}$. Multiplying by $(\log x)^2$ gives nonnegative terms, so the [monotone convergence theorem](../../../../../monotone-convergence-theorem.md) permits termwise integration. Put $x=e^{-t}$ to obtain

$$
\int_0^1x^{k-1}(\log x)^2\,dx
=\int_0^\infty t^2e^{-kt}\,dt=\frac2{k^3},
$$

where scaling followed by two integrations by parts evaluates the last integral. Hence

$$
\boxed{\int_0^1\left(\frac{\log x}{1-x}\right)^2dx
=2\sum_{k=1}^\infty\frac1{k^2}=\frac{\pi^2}{3}.}
$$

The finite value also establishes integrability at both endpoints.

## ↑ Ancestors (13)

1. [2](../2.md)
2. [D3](../../d3.md)
3. [D](../../../d.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
