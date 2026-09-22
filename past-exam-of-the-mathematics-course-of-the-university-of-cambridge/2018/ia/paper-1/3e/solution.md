<h1 id="3e/solution">Solution</h1>

↑ **Parent:** [3E](../3e.md)

Let $(u_n)$ be increasing and bounded above, and let $L=\sup\{u_n:n\in\mathbb N\}$. For every $\varepsilon>0$, the definition of the [supremum](../../../../../supremum.md) supplies $N$ with $L-\varepsilon<u_N\leq L$. Monotonicity gives $L-\varepsilon<u_n\leq L$ for every $n\geq N$, proving $u_n\to L$. This is the [monotone bounded sequence](../../../../../monotone-bounded-sequence.md) theorem.

For the recurrence, $f(x_n)>0$ makes $(x_n)$ increasing. If it were bounded above, it would converge to some $L$. Since $x_n\leq L$ and $f$ is decreasing, $f(x_n)\geq f(L)>0$, whence

$$
x_n=1+\sum_{j=1}^{n-1}f(x_j)\geq1+(n-1)f(L)\longrightarrow\infty,
$$

a contradiction. Therefore **$x_n\to\infty$**.

## ↑ Ancestors (10)

1. [3E](../3e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
