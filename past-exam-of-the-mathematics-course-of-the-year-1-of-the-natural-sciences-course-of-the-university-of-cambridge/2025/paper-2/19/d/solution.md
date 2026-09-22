<h1 id="19/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For positive integers $n$, the summand is $a_n=\sin(\pi\sin(1/n))/n$. Since $0<\sin(1/n)<1$, these terms are positive. Apply the [limit comparison test](../../../../../limit-comparison-test.md) with the convergent [p-series](../../../../../p-series.md) $\sum n^{-2}$:

$$
\frac{a_n}{n^{-2}}
=n\sin(\pi\sin(1/n))
=\frac{\sin(\pi\sin(1/n))}{\pi\sin(1/n)}\,
\pi\frac{\sin(1/n)}{1/n}
\longrightarrow\pi.
$$

Each sine ratio tends to one. The [limit comparison test](../../../../../limit-comparison-test.md) says that two positive-term [series](../../../../../series-mathematics.md) whose term ratio tends to a finite positive number are either both [convergent](../../../../../convergent-series.md) or both [divergent](../../../../../divergent-series.md). Therefore

$$
\boxed{\sum_{n=1}^\infty f_{-1}(n)\text{ converges absolutely}}.
$$

There is also a direct [comparison test for series](../../../../../comparison-test-for-series.md): $0\leq\sin(\pi\sin(1/n))\leq\pi\sin(1/n)\leq\pi/n$, giving $0\leq a_n\leq\pi/n^2$.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [19](../../19.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
