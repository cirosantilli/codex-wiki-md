<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For [Newton's method for nonlinear systems](../../../../../../multivariable-newton-iteration.md), solve $J(\mathbf z_0)\boldsymbol\delta=-\mathbf F(\mathbf z_0)$ and set $\mathbf z_1=\mathbf z_0+\boldsymbol\delta$. The [Jacobian matrix](../../../../../../jacobian-matrix.md) here is

$$
J(x,y)=\begin{pmatrix}
3x^2+3&-2\\
3x^2&6y-1
\end{pmatrix}.
$$

At $(0,0)$,

$$
\mathbf F(0,0)=\begin{pmatrix}-1\\-1\end{pmatrix},\qquad
J(0,0)=\begin{pmatrix}3&-2\\0&-1\end{pmatrix}.
$$

The correction [linear system](../../../../../../system-of-linear-equations.md) is $3\delta_x-2\delta_y=1$, $-\delta_y=1$. Hence $\delta_y=-1$, $\delta_x=-1/3$, and one iteration gives

$$
\boxed{(x_1,y_1)=(-1/3,-1).}
$$

At the alternative starting value $(1,0)$,

$$
\mathbf F(1,0)=\begin{pmatrix}3\\0\end{pmatrix},\qquad
J(1,0)=\begin{pmatrix}6&-2\\3&-1\end{pmatrix}.
$$

This [Jacobian matrix](../../../../../../jacobian-matrix.md) is a [singular matrix](../../../../../../singular-matrix.md): its first row is twice its second. In fact the correction equations would be

$$
6\delta_x-2\delta_y=-3,\qquad 3\delta_x-\delta_y=0,
$$

which are inconsistent, since twice the second left side equals the first while twice its right side is $0$, rather than $-3$. Thus **Newton's iteration cannot take its first step from $(1,0)$**. This is failure of the correction [linear system](../../../../../../system-of-linear-equations.md), not merely nonuniqueness of a possible correction.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [7](../../7.md)
3. [Mathematics IV](../../../mathematics-iv-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
