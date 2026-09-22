<h1 id="b/5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

With $y=-c/\mu$, [differentiation](../../../../../differentiation.md) of the [quadratic penalty method](../../../../../quadratic-penalty-method.md) objective gives

$$
\boxed{\nabla P_\mu=g-A^Ty,\qquad \nabla^2P_\mu=H(x,y)+\mu^{-1}A^TA.}
$$

The primal [Newton system](../../../../../newton-system.md) is therefore

$$
\boxed{(H+\mu^{-1}A^TA)p=-g+A^Ty.}
$$

For bounded multipliers and regular derivatives, $H$ remains of ordinary size while $\mu^{-1}A^TA$ becomes large in directions normal to the constraints. If the feasible tangent space is nontrivial and retains ordinary-size curvature, this produces a large [condition number](../../../../../condition-number.md) as $\mu\downarrow0$.

Introduce $w=Ap/\mu$. The same step is obtained from the symmetric augmented system

$$
\boxed{\begin{pmatrix}H&A^T\\A&-\mu I\end{pmatrix}\begin{pmatrix}p\\w\end{pmatrix}=\begin{pmatrix}-g+A^Ty\\0\end{pmatrix}.}
$$

Eliminating $w$ recovers the primal system exactly. This matrix contains no explicit $\mu^{-1}$ entries and tends to a [saddle-point matrix](../../../../../saddle-point-matrix.md). Under full row rank of the limiting constraint [Jacobian matrix](../../../../../jacobian-matrix.md) and nonsingularity of the limiting [reduced Hessian](../../../../../reduced-hessian.md), that limiting matrix is nonsingular, so this formulation avoids the artificial penalty-induced separation of scales.

These conditioning statements require regularity beyond bounded $y$ alone. A rank-deficient constraint [Jacobian matrix](../../../../../jacobian-matrix.md) or singular [reduced Hessian](../../../../../reduced-hessian.md) can still make the augmented system ill-conditioned. If $m=n$ and $A$ is nonsingular, all directions may scale together in the primal system, so a large condition number is not automatic there either.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
