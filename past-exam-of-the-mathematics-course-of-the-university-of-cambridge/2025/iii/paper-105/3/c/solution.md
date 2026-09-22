<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With $g=0$, pull the bounded measurable initial value back along the [characteristic flow map](../../../../../../characteristic-flow-map.md):

$$
u(t,x)=u_0(X(0;t,x)).
$$

The flow is measurable and invertible, so $u$ is measurable and $\|u\|_\infty\leq\|u_0\|_\infty$. Choose smooth $u_0^{(k)}$ converging to $u_0$ in $L^1_{\mathrm{loc}}$ with uniformly bounded essential suprema, and define

$$
u^{(k)}(t,x)=u_0^{(k)}(X(0;t,x)).
$$

Part a makes each $u^{(k)}$ a classical, hence weak, solution. On every compact subset of spacetime, the $C^1$ change-of-variables formula for the flow and its locally bounded [Jacobian determinant](../../../../../../jacobian-determinant.md) give $u^{(k)}\to u$ in $L^1$. Passing to the limit in the weak identity by [dominated convergence](../../../../../../dominated-convergence-theorem.md) proves that $u$ is a bounded weak solution with initial datum $u_0$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
