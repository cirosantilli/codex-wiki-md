<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [b](../b.md)

To find a [critical point](../../../../../../critical-point.md), apply [multivariable Newton iteration](../../../../../../multivariable-newton-iteration.md) to the [gradient](../../../../../../gradient.md), rather than to the scalar value $F$. The [gradient](../../../../../../gradient.md) and [Hessian matrix](../../../../../../hessian-matrix.md) are

$$
\nabla F=\begin{pmatrix}2x+2y\\2x-2y+3y^2\end{pmatrix},\qquad
\nabla^2F=\begin{pmatrix}2&2\\2&-2+6y\end{pmatrix}.
$$

Write the correction as $\mathbf s_0=\mathbf x_1-\mathbf x_0$. At $\mathbf x_0=(-1,-1)$, [Newton's method in optimization](../../../../../../newton-s-method-in-optimization.md) requires

$$
\begin{pmatrix}2&2\\2&-8\end{pmatrix}\mathbf s_0=-\begin{pmatrix}-4\\3\end{pmatrix}=\begin{pmatrix}4\\-3\end{pmatrix}.
$$

Subtracting the second [equation](../../../../../../equation.md) from the first gives $10s_y=7$, so $s_y=7/10$ and $s_x=13/10$. Hence

$$
\boxed{(x_1,y_1)=\left(\frac3{10},-\frac3{10}\right).}
$$

The [gradient](../../../../../../gradient.md) there is

$$
\nabla F(3/10,-3/10)=\begin{pmatrix}0\\147/100\end{pmatrix}\ne\mathbf0.
$$

**A [critical point](../../../../../../critical-point.md) has not been found after one iteration.**

At the alternative starting [point](../../../../../../point-geometry.md) $(0,2/3)$, the [Hessian matrix](../../../../../../hessian-matrix.md) and [gradient](../../../../../../gradient.md) are

$$
\nabla^2F=\begin{pmatrix}2&2\\2&2\end{pmatrix},\qquad
\nabla F=\begin{pmatrix}4/3\\0\end{pmatrix}.
$$

The correction would need to satisfy $2s_x+2s_y=-4/3$ and $2s_x+2s_y=0$ simultaneously. This [linear system](../../../../../../system-of-linear-equations.md) is inconsistent. **The standard iteration cannot take even its first step**: the [Hessian matrix](../../../../../../hessian-matrix.md) is a [singular matrix](../../../../../../singular-matrix.md), and the required correction does not exist. This is a [Newton correction compatibility condition](../../../../../../newton-correction-compatibility-condition.md) failure, not merely an ambiguity between several corrections.

## ↑ Ancestors (12)

1. [b](../b.md)
2. [7](../../7.md)
3. [Mathematics IV](../../../mathematics-iv-split.md)
4. [Prelims](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
