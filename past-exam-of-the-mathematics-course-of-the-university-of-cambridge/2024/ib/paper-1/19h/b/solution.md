<h1 id="19h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

There are no visits when the initial excursion returns to $i$ before hitting $j$, so

$$
\boxed{\mathbb P_i(N=0)=1-\alpha}.
$$

For $k\geq1$, the chain must first hit $j$, return to $j$ before $i$ exactly $k-1$ times, and then hit $i$ before another return to $j$. The [Strong Markov property](../../../../../../strong-markov-property.md) gives

$$
\boxed{
\mathbb P_i(N=k)=\alpha^2(1-\alpha)^{k-1},
\qquad k\geq1}.
$$

The formula also covers the boundary cases $\alpha=0$ and $\alpha=1$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [19H](../../19h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
