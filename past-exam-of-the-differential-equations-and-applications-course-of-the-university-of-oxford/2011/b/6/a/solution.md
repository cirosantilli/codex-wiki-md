<h1 id="b/6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $F_p,F_q$ evaluated at the fixed pair $(p(s),q(s))$. Differentiating in $\tau$ gives $x_\tau=F_p$, $y_\tau=F_q$, and $u_\tau=pF_p+qF_q$, proving $u_\tau=px_\tau+qy_\tau$.

Differentiate the other parameter. The difference of the required sides is

$$
u_s-px_s-qy_s=(u_0'-px_0'-qy_0')+\tau(p'F_p+q'F_q).
$$

The first bracket is zero by the prescribed initial compatibility condition, and the second is zero by differentiating $F(p(s),q(s))=0$. Thus $u_s=px_s+qy_s$ as well. These calculations use the differentiability of the supplied parametric functions.

If the coordinate [Jacobian determinant](../../../../../jacobian-determinant.md) $J=x_sy_\tau-y_sx_\tau$ is nonzero, the [inverse function theorem](../../../../../inverse-function-theorem.md) gives local coordinates $(x,y)$. The [chain rule](../../../../../chain-rule.md) then makes $(u_x-p,u_y-q)$ solve a homogeneous two-by-two [linear system](../../../../../system-of-linear-equations.md) with determinant $J$. Therefore

$$
\boxed{u_x=p,\qquad u_y=q.}
$$

This is the [method of characteristics](../../../../../method-of-characteristics.md) for a first-order equation depending only on the gradient.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the differential equations and applications course of the University of Oxford](../../../../split.md)
6. [Differential equations and applications course of the University of Oxford](../../../../../differential-equations-and-applications-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
