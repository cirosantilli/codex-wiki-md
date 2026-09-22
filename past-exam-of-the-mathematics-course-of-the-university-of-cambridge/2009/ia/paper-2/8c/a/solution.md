<h1 id="8c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [chain rule](../../../../../../chain-rule.md) gives $\partial_x=\partial_u+\partial_v$ and $\partial_t=\partial_u-\partial_v$. Hence $\partial_x^2-\partial_t^2=4\partial_u\partial_v$, and the forced [wave equation](../../../../../../wave-equation-split.md) becomes $y_{uv}=1$. Integrating twice gives $y=uv+F(u)+G(v)$. At $t=0$ the initial conditions are

$$
x^2+F(x)+G(x)=\sin x,\qquad F'(x)-G'(x)=0.
$$

Thus $F-G$ is constant, which cancels from the final expression. Combining the remaining sum yields

$$
y=uv+\tfrac12(\sin u+\sin v-u^2-v^2)
=\boxed{\sin x\cos t-2t^2.}
$$

Differentiation checks the forcing and both initial conditions.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [8C](../../8c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
