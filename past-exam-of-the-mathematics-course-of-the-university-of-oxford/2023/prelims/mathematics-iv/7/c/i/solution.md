<h1 id="7/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a twice [continuously differentiable function](../../../../../../../continuously-differentiable-function.md) $F$, its [gradient](../../../../../../../gradient.md) and [Hessian matrix](../../../../../../../hessian-matrix.md) are

$$
\nabla F(x,y)=\begin{pmatrix}F_x\\F_y\end{pmatrix},\qquad
H_F(x,y)=\begin{pmatrix}F_{xx}&F_{xy}\\F_{yx}&F_{yy}\end{pmatrix}.
$$

A [critical point](../../../../../../../critical-point.md) solves $\nabla F=0$. The [Jacobian matrix](../../../../../../../jacobian-matrix.md) of this vector equation is $H_F$, so the [multivariable Newton iteration](../../../../../../../multivariable-newton-iteration.md) is

$$
\boxed{H_F(\mathbf x_k)\mathbf s_k=-\nabla F(\mathbf x_k),\qquad\mathbf x_{k+1}=\mathbf x_k+\mathbf s_k.}
$$

Equivalently $\mathbf x_{k+1}=\mathbf x_k-H_F(\mathbf x_k)^{-1}\nabla F(\mathbf x_k)$ when the [Hessian matrix](../../../../../../../hessian-matrix.md) is invertible. Solving the [linear system](../../../../../../../system-of-linear-equations.md) is the direct computational form. A [critical point](../../../../../../../critical-point.md) found in this way need not be a [local minimum](../../../../../../../local-minimum.md); its type requires a separate check.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [7](../../../7.md)
4. [Mathematics IV](../../../../mathematics-iv-split.md)
5. [Prelims](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
