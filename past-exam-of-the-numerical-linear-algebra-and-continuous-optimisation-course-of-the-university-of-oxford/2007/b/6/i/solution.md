<h1 id="b/6/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [optimization Lagrangian](../../../../../optimization-lagrangian.md) $L(x,y)=f(x)-y^Tc(x)$ and let $A=Dc$ be the $m\times n$ constraint [Jacobian matrix](../../../../../jacobian-matrix.md). Under the standard regularity hypothesis $\operatorname{rank}A(x_*)=m$, a local constrained minimizer satisfies, for some multiplier $y_*$,

$$
\boxed{c(x_*)=0,\qquad\nabla f(x_*)-A(x_*)^Ty_*=0.}
$$

The second-order necessary condition is

$$
\boxed{d^T\nabla_{xx}^2L(x_*,y_*)d\geq0\quad\text{whenever }A(x_*)d=0.}
$$

Regularity makes each such tangent vector the velocity of a feasible smooth curve. Twice differentiating the objective along that curve and using stationarity and the differentiated constraints gives the displayed nonnegative second derivative.

The regularity hypothesis is needed for these multiplier conditions to be necessary in this form. For example minimizing $f(x)=x$ subject to $c(x)=x^2=0$ has the unique feasible minimizer zero, but $f'(0)-yc'(0)=1$ for every $y$. The question does not explicitly state the qualification, so it must be supplied when using the usual [KKT conditions](../../../../../karush-kuhn-tucker-conditions.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
