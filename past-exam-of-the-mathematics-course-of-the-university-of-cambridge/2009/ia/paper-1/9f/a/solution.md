<h1 id="9f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $s=\sin x$, so $-1\le s\le1$. The printed summand is $(3s^n+s^{2n})/n$. If $|s|<1$, its absolute value is at most $3|s|^n+|s|^{2n}$, and the two [geometric series](../../../../../../geometric-series.md) converge. Thus there is [absolute convergence](../../../../../../absolute-convergence.md).

For $s=1$ the [series](../../../../../../series-mathematics.md) becomes $\sum4/n$, a divergent multiple of the [harmonic series](../../../../../../harmonic-series.md). For $s=-1$ it becomes

$$
3\sum_{n\ge1}\frac{(-1)^n}{n}+\sum_{n\ge1}\frac1n.
$$

The first [series](../../../../../../series-mathematics.md) converges by the [alternating series test](../../../../../../alternating-series-test.md), while the second diverges to $+\infty$, so their partial sums tend to $+\infty$. In particular, alternation of some terms does not imply convergence here. The complete classification is

$$
\boxed{\begin{array}{ll}x\notin\{\pi/2+k\pi:k\in\mathbb Z\}:&\text{absolute convergence},\\x\in\{\pi/2+k\pi:k\in\mathbb Z\}:&\text{divergence to }+\infty.\end{array}}
$$

**There are no conditionally convergent cases.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [9F](../../9f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
