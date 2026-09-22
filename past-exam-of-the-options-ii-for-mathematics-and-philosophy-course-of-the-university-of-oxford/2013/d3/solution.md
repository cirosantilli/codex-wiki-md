<h1 id="d3/solution">Solution</h1>

↑ **Parent:** [D3](../d3.md)

The [monotone convergence theorem](../../../monotone-convergence-theorem.md) states that if $0\leq h_n\uparrow h$ pointwise for measurable [functions](../../../function-split.md), then $h$ is measurable and $\int h=\lim_n\int h_n$, allowing infinity.

Apply it to the partial sums $S_N=\sum_{n=0}^Nf_n$. They are nonnegative, measurable, and increase pointwise to $f$. Finite additivity of the [integral](../../../integral-split.md) and monotone convergence yield

$$
\boxed{\int_{\mathbb R}f=\lim_{N\to\infty}\sum_{n=0}^N\int_{\mathbb R}f_n
=\sum_{n=0}^{\infty}\int_{\mathbb R}f_n.}
$$

The assumed finite sum of [integrals](../../../integral-split.md) makes $f$ integrable. This proves the series-integration rule needed below directly from the stated theorem, without assuming an additional interchange theorem.

## ↑ Ancestors (11)

1. [D3](../d3.md)
2. [2013](../../2013-split.md)
3. [Past exam of the options II for mathematics and philosophy course of the University of Oxford](../../split.md)
4. [Options II for mathematics and philosophy course of the University of Oxford](../../../options-ii-for-mathematics-and-philosophy-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics and philosophy course of the University of Oxford](../../../year-2-of-the-mathematics-and-philosophy-course-of-the-university-of-oxford.md)
6. [Mathematics and philosophy course of the University of Oxford](../../../mathematics-and-philosophy-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
