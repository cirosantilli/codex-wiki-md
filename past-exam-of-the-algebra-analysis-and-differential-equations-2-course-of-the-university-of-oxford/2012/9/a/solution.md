<h1 id="9/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a [quasilinear partial differential equation](../../../../quasilinear-partial-differential-equation.md), the [characteristic equations for a quasilinear equation](../../../../characteristic-equations-for-a-first-order-quasilinear-equation.md) are the ordinary [differential equations](../../../../differential-equation-split.md)

$$
\boxed{\frac{dx}{ds}=P(x,y,z),\qquad\frac{dy}{ds}=Q(x,y,z),\qquad\frac{dz}{ds}=R(x,y,z).}
$$

A [solution surface](../../../../solution-surface.md) is locally a differentiable graph $z=u(x,y)$ whose tangent plane contains the [vector](../../../../vector.md) $(P,Q,R)$ at every point. Its normal is $(-u_x,-u_y,1)$, so the tangency condition is precisely $Pu_x+Qu_y=R$. Thus every characteristic lying on that graph follows the [vector](../../../../vector.md) field without leaving the graph.

Parameterize the given initial curve by $\gamma(t)=(x_0(t),y_0(t),z_0(t))$. For each $t$, solve the [characteristic equations for a quasilinear equation](../../../../characteristic-equations-for-a-first-order-quasilinear-equation.md) with initial value $\gamma(t)$ at $s=0$. The resulting map $(s,t)\mapsto(x(s,t),y(s,t),z(s,t))$ sweeps out a candidate solution surface. If the [coefficients](../../../../coefficient.md) and initial data are continuously differentiable, the [Picard-Lindelöf theorem](../../../../picard-lindelof-theorem.md) supplies this local family. To make it a graph we also need the projection $(s,t)\mapsto(x,y)$ to be locally invertible. At $s=0$ its [Jacobian determinant](../../../../jacobian-determinant.md) is

$$
J(0,t)=P(\gamma(t))y_0'(t)-Q(\gamma(t))x_0'(t).
$$

The [Noncharacteristic Cauchy data](../../../../noncharacteristic-cauchy-data.md) condition is $J(0,t)\ne0$. The [inverse function theorem](../../../../inverse-function-theorem.md) then gives $s=s(x,y)$ and $t=t(x,y)$, and hence $u(x,y)=z(s(x,y),t(x,y))$. Its [derivatives](../../../../derivative.md) obey the PDE by the [chain rule](../../../../chain-rule.md). The same characteristic initial-value uniqueness gives local uniqueness of this solution wherever the projection remains invertible and the relevant characteristic meets the prescribed data.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [9](../../9.md)
3. [2012](../../../2012-split.md)
4. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
