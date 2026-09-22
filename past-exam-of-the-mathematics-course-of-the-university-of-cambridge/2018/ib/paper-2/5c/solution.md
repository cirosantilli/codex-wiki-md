<h1 id="5c/solution">Solution</h1>

↑ **Parent:** [5C](../5c.md)

Along a curve $s\mapsto(x(s),y(s))$, the [chain rule](../../../../../chain-rule.md) gives

$$
\frac d{ds}u_x=u_{xx}\dot x+u_{xy}\dot y,
\qquad
\frac d{ds}u_y=u_{xy}\dot x+u_{yy}\dot y.
$$

Together with the [second-order partial differential equation](../../../../../second-order-partial-differential-equation.md), these form a [linear system](../../../../../system-of-linear-equations.md) for $(u_{xx},u_{xy},u_{yy})$ whose coefficient matrix is

$$
\begin{pmatrix}
\dot x&\dot y&0\\
0&\dot x&\dot y\\
a&2b&c
\end{pmatrix}.
$$

A [characteristic curve](../../../../../characteristic-curve.md) is precisely one along which this system is singular, equivalently where the [principal symbol](../../../../../principal-symbol-of-a-partial-differential-equation.md) vanishes on a normal covector. Taking the [determinant](../../../../../determinant.md) yields

$$
\boxed{a\dot y^2-2b\dot x\dot y+c\dot x^2=0.}
$$

## ↑ Ancestors (10)

1. [5C](../5c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
