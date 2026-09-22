<h1 id="7/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For an unconstrained differentiable [function](../../../../../../../function-split.md) of two real variables, an interior [local minimum](../../../../../../../local-minimum.md) must solve the simultaneous [stationary point](../../../../../../../stationary-point.md) equations

$$
f_x(x,y)=0,\qquad f_y(x,y)=0,
\quad\text{or}\quad \nabla f(x,y)=0.
$$

Apply [Newton's method in optimization](../../../../../../../newton-s-method-in-optimization.md) to this [gradient](../../../../../../../gradient.md) equation. The [Jacobian matrix](../../../../../../../jacobian-matrix.md) of the [gradient](../../../../../../../gradient.md) is the [Hessian matrix](../../../../../../../hessian-matrix.md)

$$
H(x,y)=\begin{pmatrix}f_{xx}&f_{xy}\\f_{yx}&f_{yy}\end{pmatrix}.
$$

At $p_n=(x_n,y_n)^T$, solve the [linear system](../../../../../../../system-of-linear-equations.md) $H(p_n)s_n=-\nabla f(p_n)$, then set $p_{n+1}=p_n+s_n$. When the [Hessian matrix](../../../../../../../hessian-matrix.md) is invertible, this is

$$
\boxed{p_{n+1}=p_n-H(p_n)^{-1}\nabla f(p_n).}
$$

This follows by setting the first order [Taylor expansion](../../../../../../../taylor-expansion.md) $\nabla f(p_n+s_n)\simeq\nabla f(p_n)+H(p_n)s_n$ equal to zero. Solving the [linear system](../../../../../../../system-of-linear-equations.md) avoids explicitly computing a [matrix inverse](../../../../../../../matrix-inverse-split.md). A [stationary point](../../../../../../../stationary-point.md) need not be a [local minimum](../../../../../../../local-minimum.md): for example, a [positive-definite matrix](../../../../../../../positive-definite-matrix.md) $H(p)$ suffices to classify a [stationary point](../../../../../../../stationary-point.md) as a strict [local minimum](../../../../../../../local-minimum.md), whereas an indefinite [Hessian matrix](../../../../../../../hessian-matrix.md) identifies a [saddle point of a scalar function](../../../../../../../saddle-point-of-a-scalar-function.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Mathematics IV resit](../../../../mathematics-iv-resit-split.md)
5. [Prelims](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
