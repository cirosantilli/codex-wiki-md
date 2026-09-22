<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For every compactly supported $C^1$ [test function](../../../../../../test-function.md) $\varphi$ on $[0,\infty)\times\mathbb R$, define a [weak solution](../../../../../../weak-solution.md) by the identity

$$
\int_0^\infty\!\int_{\mathbb R}
u(\varphi_t+x\varphi_x+\varphi)\,dx\,dt
+\int_{\mathbb R}u_0(x)\varphi(0,x)\,dx=0.
$$

The extra $\varphi$ appears because $\partial_x(x\varphi)=x\varphi_x+\varphi$. This identity is obtained from the [linear transport equation](../../../../../../linear-transport-equation.md) by [integration by parts](../../../../../../integration-by-parts.md) in time and space.

Conversely, if $u$ and $u_0$ have the stated $C^1$ regularity, choosing test functions supported away from $t=0$ shows in the [distributional sense](../../../../../../distributional-identity.md) that $u_t+xu_x=0$. Continuity makes the equation pointwise. Integrating that pointwise equation by parts in the displayed identity leaves

$$
\int_{\mathbb R}\bigl(u(0,x)-u_0(x)\bigr)\varphi(0,x)\,dx=0
$$

for all boundary test functions. The [fundamental lemma of the calculus of variations](../../../../../../fundamental-lemma-of-the-calculus-of-variations.md) gives $u(0,x)=u_0(x)$, so $u$ is a [classical solution](../../../../../../classical-solution.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
