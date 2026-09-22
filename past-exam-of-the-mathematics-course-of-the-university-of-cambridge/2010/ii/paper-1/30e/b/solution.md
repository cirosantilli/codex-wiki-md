<h1 id="30e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Inside the fan $u=x/t$, one has $u_t=-x/t^2$ and $u\,u_x=x/t^2$, while the constant regions also satisfy the equation. Across $x=0$ and $x=t$, the two traces of both $u$ and its flux $u^2/2$ agree. Integrating by parts separately in the three regions therefore cancels all interface terms and gives

$$
\int_0^\infty\int_{\mathbb R}\left(u\phi_t+\frac{u^2}{2}\phi_x\right)dx\,dt
+\int_{\mathbb R}u_0(x)\phi(x,0)\,dx=0
$$

for every smooth compactly supported [test function](../../../../../../test-function.md). The initial term is correct because $u(\cdot,t)\to\mathbf1_{\{x>0\}}$ in local $L^1$: the difference is supported in $(0,t)$ and its integral is at most $t$. Thus **the fan is a [weak solution](../../../../../../weak-solution.md) of the Burgers equation with the required initial data**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [30E](../../30e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
