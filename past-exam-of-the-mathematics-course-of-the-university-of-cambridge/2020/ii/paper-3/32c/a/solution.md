<h1 id="32c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $\xi=V_1$, $\eta=\phi$, and $u_j=d^ju/dx^j$. On the [jet space of a scalar ordinary differential equation](../../../../../../jet-space-of-a-scalar-ordinary-differential-equation.md), define

$$
\eta^{(0)}=\eta,
\qquad
\eta^{(j)}=D_x\eta^{(j-1)}-u_jD_x\xi,
$$

where the [total derivative operator](../../../../../../total-derivative-operator.md) is

$$
D_x=\partial_x+u_1\partial_u+u_2\partial_{u_1}+\cdots.
$$

The order-$N$ [prolongation of a vector field](../../../../../../prolongation-of-a-vector-field.md) is

$$
\boxed{
\operatorname{pr}^{(N)}V
=\xi\partial_x+\eta\partial_u
+\sum_{j=1}^N\eta^{(j)}\partial_{u_j}}.
$$

In the coordinates $(x,u)$, the given action of the [special orthogonal group](../../../../../../special-orthogonal-group.md) is

$$
\widetilde x=x\cos s+u\sin s,
\qquad
\widetilde u=u\cos s-x\sin s.
$$

Differentiating at $s=0$ gives the [infinitesimal generator of a Lie point symmetry](../../../../../../infinitesimal-generator-of-a-lie-point-symmetry.md)

$$
V=u\partial_x-x\partial_u,
$$

so $\xi=u$ and $\eta=-x$. The recursive formula gives

$$
\eta^{(1)}=D_x(-x)-u_xD_xu=-1-u_x^2
$$

and

$$
\eta^{(2)}=D_x(-1-u_x^2)-u_{xx}D_xu
=-3u_xu_{xx}.
$$

Therefore the [second prolongation of the rotation generator for plane graphs](../../../../../../second-prolongation-of-the-rotation-generator-for-plane-graphs.md) is

$$
\boxed{
\operatorname{pr}^{(2)}V
=u\partial_x-x\partial_u
-(1+u_x^2)\partial_{u_x}
-3u_xu_{xx}\partial_{u_{xx}}}.
$$

For $\Delta_0=u_{xx}$,

$$
\operatorname{pr}^{(2)}V(\Delta_0)=-3u_xu_{xx},
$$

which vanishes when $\Delta_0=0$. For

$$
\Delta_1=u_{xx}-(1+u_x^2)^{3/2},
$$

we obtain

$$
\begin{aligned}
\operatorname{pr}^{(2)}V(\Delta_1)
&=-3u_xu_{xx}
-3u_x(1+u_x^2)^{1/2}[-(1+u_x^2)]\\
&=-3u_x\Delta_1,
\end{aligned}
$$

which likewise vanishes on the equation. This is the infinitesimal invariance criterion for both equations.

Geometrically, $u_{xx}=0$ describes straight lines. The [signed curvature of a plane graph](../../../../../../signed-curvature-of-a-plane-graph.md) is

$$
\kappa=\frac{u_{xx}}{(1+u_x^2)^{3/2}},
$$

so the second equation says $\kappa=1$ and describes consistently oriented arcs of unit circles. [Rotation](../../../../../../rotation-matrix.md) preserves straight lines, circles, and signed curvature, explaining both invariances.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [32C](../../32c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
