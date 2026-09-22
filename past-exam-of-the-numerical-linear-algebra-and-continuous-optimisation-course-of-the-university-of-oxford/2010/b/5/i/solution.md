<h1 id="b/5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [optimization Lagrangian](../../../../../optimization-lagrangian.md) $\mathcal L(x,y)=f(x)-y^Tc(x)$, with $A(x)=Dc(x)$ and $H(x,y)=\nabla_{xx}^2\mathcal L(x,y)$. Under the usual [linear independence constraint qualification](../../../../../linear-independence-constraint-qualification.md), a local minimizer has multipliers $y_*$ satisfying the equality-constrained [Karush-Kuhn-Tucker conditions](../../../../../karush-kuhn-tucker-conditions.md)

$$
\boxed{c(x_*)=0,\qquad g(x_*)-A(x_*)^Ty_*=0.}
$$

The second-order necessary condition is

$$
\boxed{d^TH(x_*,y_*)d\geq0\quad\text{for every }d\in\ker A(x_*).}
$$

Only feasible tangent directions enter this last test; the [Hessian matrix](../../../../../hessian-matrix.md) need not be positive semidefinite on the entire ambient space.

## ↑ Ancestors (13)

1. [I](../i.md)
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
