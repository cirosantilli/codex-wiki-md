<h1 id="30k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $V(n,x)$ be the minimum expected remaining cost after time $n$, given $X_n=x$. The terminal condition is $V(N,x)=x^2$, and the [Bellman equation](../../../../../../bellman-equation.md) is

$$
\boxed{V(n-1,x)=\inf_{u\in\mathbb R}
\left\{u^2+\mathbb E[V(n,x+u+\xi_n)]\right\}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [30K](../../30k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
