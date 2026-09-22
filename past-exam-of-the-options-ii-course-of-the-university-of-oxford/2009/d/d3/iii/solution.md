<h1 id="d/d3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [function](../../../../../function-split.md) is [continuous](../../../../../continuous-function.md) and nonnegative, bounded above by $x$ on $(0,1)$ and by $xe^{-x}$ on $(1,\infty)$, so it is integrable. For $x>0$ the [geometric series](../../../../../geometric-series.md) gives

$$
\frac{x}{e^x+1}=\sum_{n=1}^\infty(-1)^{n-1}xe^{-nx}.
$$

The series is absolutely summable in integral because

$$
\sum_{n=1}^\infty\int_0^\infty xe^{-nx}\,dx
=\sum_{n=1}^\infty\frac1{n^2}<\infty.
$$

Each integral follows by substituting $t=nx$ and integrating $te^{-t}$ by parts. [Tonelli's theorem](../../../../../tonelli-theorem.md) applied to the absolute terms, followed by [Fubini's theorem](../../../../../fubini-s-theorem.md), therefore justifies termwise integration and gives

$$
\boxed{\int_0^\infty\frac{x}{e^x+1}\,dx=\sum_{n=1}^\infty\frac{(-1)^{n-1}}{n^2}}.
$$

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [D3](../../d3.md)
3. [D](../../../d.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
