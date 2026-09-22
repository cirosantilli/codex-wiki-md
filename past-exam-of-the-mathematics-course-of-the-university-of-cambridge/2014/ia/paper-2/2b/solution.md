<h1 id="2b/solution">Solution</h1>

↑ **Parent:** [2B](../2b.md)

For continuously differentiable coefficients on a simply connected domain, the exactness condition is **$P_y=Q_x$**. Locally the same condition suffices without a global topological assumption. An [exact first-order ordinary differential equation](../../../../../exact-first-order-ordinary-differential-equation.md) has a potential $F$ with $F_x=P$ and $F_y=Q$, so $dF/dx=P+Qy'=0$ along a solution. Thus its [implicit solution](../../../../../implicit-solution.md) is $F(x,y)=C$. One local construction, on a rectangle about $(x_0,y_0)$, is

$$
F(x,y)=\int_{x_0}^xP(s,y_0)\,ds+\int_{y_0}^yQ(x,t)\,dt.
$$

The equality of cross derivatives verifies both required derivatives; on a simply connected domain one may use the corresponding path-independent integral of the [exact differential form](../../../../../exact-differential-form.md).

Here $P=4x+3y$, $Q=3x+3y^2$ and $P_y=Q_x=3$. Integrating $P$ with respect to $x$ gives $F=2x^2+3xy+K(y)$. Matching $F_y=Q$ gives $K'=3y^2$, so take $K=y^3$. The initial value sets $C=F(1,2)=16$. Therefore

$$
\boxed{2x^2+3xy+y^3=16.}
$$

This is the requested explicit relation between the coordinates. Since $F_y(1,2)=15\ne0$, the [implicit function theorem](../../../../../implicit-function-theorem.md) gives a unique local graph through the initial point, with slope $-10/15=-2/3$.

## ↑ Ancestors (10)

1. [2B](../2b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
