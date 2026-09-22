<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Restrict $\varphi$ to an arbitrary [line segment](../../../../../../../line-segment.md) by defining $q(t)=\varphi((1-t)x+ty)$ for $0\leq t\leq1$. The [chain rule](../../../../../../../chain-rule.md) and the assumed [positive semidefinite matrix](../../../../../../../positive-semidefinite-matrix.md) condition on the [Hessian matrix](../../../../../../../hessian-matrix.md) give

$$
q''(t)=(y-x)^\top D^2\varphi((1-t)x+ty)(y-x)\geq0.
$$

Thus $q'$ is non-decreasing. For $0<t<1$, integrating $q'$ on the two subintervals gives

$$
\frac{q(t)-q(0)}t\leq\frac{q(1)-q(t)}{1-t}.
$$

Rearranging, and including the immediate endpoint cases, yields

$$
\boxed{\varphi((1-t)x+ty)\leq(1-t)\varphi(x)+t\varphi(y)\quad(0\leq t\leq1).}
$$

This is precisely the definition of a [convex function](../../../../../../../convex-function.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 348](../../../../paper-348-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
