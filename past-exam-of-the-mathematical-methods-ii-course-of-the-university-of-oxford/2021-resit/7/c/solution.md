<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [expectation](../../../../expected-value-split.md) follows by [integration by parts](../../../../integration-by-parts.md), with $u=t$ and $dv=e^{-t/25}\,dt/25$:

$$
\mathbb E[T]=\int_0^\infty t\,\frac1{25}e^{-t/25}\,dt
=\left[-te^{-t/25}\right]_0^\infty+\int_0^\infty e^{-t/25}\,dt.
$$

The endpoint term vanishes because the [exponential function](../../../../exponential-function.md) decays faster than $t$ grows. Hence the mean lifetime is

$$
\boxed{\mathbb E[T]=25\ \text{months}.}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [7](../../7.md)
3. [2021 resit](../../../2021-resit-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
