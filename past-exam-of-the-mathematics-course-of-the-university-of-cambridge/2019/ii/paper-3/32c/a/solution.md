<h1 id="32c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $u_j=u^{(j)}$. The transformation $\psi_s:(x,u)\mapsto(\widetilde x,\widetilde u)$ induces a transformation of the $n$th [jet space of a scalar ordinary differential equation](../../../../../../jet-space-of-a-scalar-ordinary-differential-equation.md) by differentiating $\widetilde u$ with respect to $\widetilde x$ through order $n$. The infinitesimal generator of this induced action is the [prolongation of a vector field](../../../../../../prolongation-of-a-vector-field.md)

$$
\boxed{
\operatorname{pr}^{(n)}V
=V+\sum_{j=1}^n\eta_j\frac{\partial}{\partial u_j}.}
$$

To determine its coefficients, put $\eta_0=\eta$ and use the [total derivative operator](../../../../../../total-derivative-operator.md)

$$
D_x=\frac{\partial}{\partial x}
+u_1\frac{\partial}{\partial u}
+\sum_{j\geq1}u_{j+1}\frac{\partial}{\partial u_j}.
$$

Differentiating transformed derivatives by

$$
\widetilde u_j
=\frac{D_x\widetilde u_{j-1}}{D_x\widetilde x}
$$

and then differentiating with respect to the group parameter at $s=0$ gives the recursion

$$
\boxed{
\eta_j=D_x\eta_{j-1}-u_jD_x\xi,
\qquad j=1,\ldots,n.}
$$

This also proves the displayed form of the prolongation by mathematical induction on the derivative order.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [32C](../../32c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
