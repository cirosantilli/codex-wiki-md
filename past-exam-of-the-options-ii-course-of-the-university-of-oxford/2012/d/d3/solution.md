<h1 id="d/d3/solution">Solution</h1>

↑ **Parent:** [D3](../d3.md)

The [monotone convergence theorem](../../../../monotone-convergence-theorem.md) states that if [measurable functions](../../../../measurable-function.md) $0\leq f_n\uparrow f$ pointwise on a [measure space](../../../../measure-space.md), then $\int f_n\uparrow\int f$, allowing the limit to be infinite.

Extend each restriction to $I_n$ by zero on $I\setminus I_n$. The functions $f\mathbf1_{I_n}$ are nonnegative and increase pointwise to $f$ because the [intervals](../../../../interval-mathematics.md) are increasing and exhaust $I$. Hence

$$
\int_I f=\lim_{n\to\infty}\int_{I_n}f=\sup_n\int_{I_n}f.
$$

For nonnegative $f$, [integrability](../../../../integrability.md) means finiteness of this [integral](../../../../integral-split.md), so

$$
\boxed{f\in L^1(I)\iff\sup_n\int_{I_n}f<\infty.}
$$

No [boundedness](../../../../boundedness.md) or [closedness](../../../../closedness.md) of the [intervals](../../../../interval-mathematics.md) is required.

## ↑ Ancestors (12)

1. [D3](../d3.md)
2. [D](../../d.md)
3. [2012](../../../2012-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
