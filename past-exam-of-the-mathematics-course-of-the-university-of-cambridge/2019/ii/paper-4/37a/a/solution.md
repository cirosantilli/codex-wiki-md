<h1 id="37a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\mathbf u$ be the [Stokes flow](../../../../../../stokes-flow-split.md) and let $\mathbf v$ be any other admissible incompressible flow with the same [no-slip boundary condition](../../../../../../no-slip-boundary-condition.md) on the sphere and the same decay at infinity. Put

$$
\mathbf w=\mathbf v-\mathbf u,
\qquad
\mathbf e(\mathbf q)
=\frac12\left(\nabla\mathbf q+\nabla\mathbf q^T\right).
$$

Then $\nabla\mathbin{\cdot}\mathbf w=0$ and $\mathbf w=0$ on the sphere. The [viscous dissipation](../../../../../../viscous-dissipation.md) satisfies

$$
\begin{aligned}
\mathcal D[\mathbf v]
&=2\mu\int_{\mathcal D}
\mathbf e(\mathbf u+\mathbf w):
\mathbf e(\mathbf u+\mathbf w)\,dV\\
&=\mathcal D[\mathbf u]
+4\mu\int_{\mathcal D}\mathbf e(\mathbf u):\mathbf e(\mathbf w)\,dV
+2\mu\int_{\mathcal D}\mathbf e(\mathbf w):\mathbf e(\mathbf w)\,dV.
\end{aligned}
$$

For the Stokes stress

$$
\boldsymbol\sigma=-p\mathbf I+2\mu\mathbf e(\mathbf u),
$$

incompressibility of $\mathbf w$ gives

$$
2\mu\mathbf e(\mathbf u):\mathbf e(\mathbf w)
=\boldsymbol\sigma:\nabla\mathbf w.
$$

The [divergence theorem](../../../../../../divergence-theorem.md), the homogeneous boundary data, decay at infinity, and $\nabla\mathbin{\cdot}\boldsymbol\sigma=0$ give

$$
\int_{\mathcal D}\boldsymbol\sigma:\nabla\mathbf w\,dV
=\int_{\partial\mathcal D}\mathbf w\mathbin{\cdot}
\boldsymbol\sigma\mathbf n\,dS
-\int_{\mathcal D}\mathbf w\mathbin{\cdot}
(\nabla\mathbin{\cdot}\boldsymbol\sigma)\,dV
=0.
$$

Therefore

$$
\boxed{
\mathcal D[\mathbf v]-\mathcal D[\mathbf u]
=2\mu\int_{\mathcal D}
\mathbf e(\mathbf w):\mathbf e(\mathbf w)\,dV\geq0.}
$$

This proves the [Minimum-dissipation theorem for Stokes flow](../../../../../../minimum-dissipation-theorem-for-stokes-flow.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [37A](../../37a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
