<h1 id="23g/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the usual hypothesis that the ground field has characteristic different from two, and work over its algebraic closure for the geometric points. This hypothesis is necessary for the smooth elliptic-curve calculation: in characteristic two, the displayed cubic model can be singular even when its three roots are distinct.

Homogenization gives

$$
Y^2Z=(X-\lambda_1Z)(X-\lambda_2Z)(X-\lambda_3Z).
$$

At $Z=0$ this says $X^3=0$, so

$$
\boxed{P_\infty=[0:1:0].}
$$

To compute the [pole orders on a smooth cubic in Weierstrass form](../../../../../../pole-orders-on-a-smooth-cubic-in-weierstrass-form.md), work in the chart $Y=1$, writing $u=X/Y$ and $v=Z/Y$. The equation is $v=\prod_j(u-\lambda_jv)$. Its derivative in $v$ at $(0,0)$ is one on the left after bringing the right side across, so $u$ is a [local parameter](../../../../../../local-parameter-on-a-smooth-algebraic-curve.md). The equation gives $v=u^3+O(u^5)$. Consequently $x=u/v$ and $y=1/v$ have poles of orders two and three at $P_\infty$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [23G](../../23g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
