<h1 id="1/a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For the construction above, independence of the [normal random variables](../../../../../../../gaussian-random-variable.md) makes $S_N(h)$ normal with mean zero and variance $v_N=\sum_{j\le N}\langle h,e_j\rangle^2$. Its [characteristic function](../../../../../../../characteristic-function.md) is $\exp(-\theta^2v_N/2)$. The $L^2$ convergence gives $L^1$ convergence, and

$$
\left|\mathbb E e^{i\theta S_N(h)}-\mathbb E e^{i\theta X(h)}\right|\le |\theta|\,\mathbb E|S_N(h)-X(h)|\longrightarrow0.
$$

Since $v_N\to\|h\|^2$ by the [Parseval identity for a Hilbertian basis](../../../../../../../parseval-identity-for-a-hilbertian-basis.md), the limiting [characteristic function](../../../../../../../characteristic-function.md) identifies

$$
\boxed{X(h)\sim N(0,\|h\|^2).}
$$

This includes $h=0$, where the [normal distribution](../../../../../../../normal-distribution.md) is degenerate at zero.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 25](../../../../paper-25-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
