<h1 id="d/d3/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Apply the [monotone convergence theorem](../../../../../monotone-convergence-theorem.md) to $s_N=\sum_{k=1}^N|a_k|$. Its limit $s$ satisfies

$$
\int s=\sum_{k=1}^\infty\int|a_k|<\infty.
$$

Thus $s$ is finite almost everywhere, which proves [absolute convergence](../../../../../absolute-convergence.md) of $\sum_k a_k$ almost everywhere. Define its sum $a$ there, and set $a=0$ on the exceptional [null set](../../../../../null-set.md). Then $|a|\leq s$, so $a$ is integrable. The partial sums of $\sum_k a_k$ are also dominated by $s$; [dominated convergence](../../../../../dominated-convergence-theorem.md) gives

$$
\boxed{\int\sum_{k=1}^\infty a_k=\lim_{N\to\infty}\sum_{k=1}^N\int a_k
=\sum_{k=1}^\infty\int a_k.}
$$

The series of integrals converges absolutely, since $|\int a_k|\leq\int|a_k|$.

## ↑ Ancestors (13)

1. [1](../1.md)
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
