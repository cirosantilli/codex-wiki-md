<h1 id="8c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose $X=x-2y$ and $T=x$, so $(\alpha,\beta,\gamma,\delta)=(1,-2,1,0)$. The [Jacobian determinant](../../../../../../jacobian-determinant.md) of the coordinate change is two, so it is an [invertible linear map](../../../../../../invertible-linear-map.md). By the [chain rule](../../../../../../chain-rule.md), $\partial_x=\partial_X+\partial_T$ and $\partial_y=-2\partial_X$. Consequently

$$
\partial_x^2+\partial_x\partial_y
=(\partial_X+\partial_T)(\partial_T-\partial_X)
=\partial_T^2-\partial_X^2.
$$

This is the [wave equation](../../../../../../wave-equation-split.md) with $c=1$. The [D'Alembert formula](../../../../../../d-alembert-s-formula.md) is $F(X,T)=U(X+T)+V(X-T)$, with arbitrary twice [differentiable functions](../../../../../../differentiable-function.md) $U,V$. Returning to the old coordinates and absorbing factors of two into the arbitrary functions gives

$$
\boxed{f(x,y)=G(x-y)+H(y).}
$$

Direct differentiation checks the cancellation. Equivalently, first integrating $\partial_x(f_x+f_y)=0$ produces the same two-function family.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [8C](../../8c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
