<h1 id="12/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [variation of parameters](../../../../variation-of-parameters.md), writing $y_p=t_1u_1+t_2u_2$ and imposing $t_1'u_1+t_2'u_2=0$. [Differentiation](../../../../differentiation.md) then gives $y_p'=t_1u_1'+t_2u_2'$. Since the $u_j$ solve the homogeneous equation,

$$
L(y_p)=t_1'u_1'+t_2'u_2'.
$$

Thus solve the two-by-two [linear system](../../../../system-of-linear-equations.md)

$$
\begin{pmatrix}u_1&u_2\\u_1'&u_2'\end{pmatrix}
\begin{pmatrix}t_1'\\t_2'\end{pmatrix}
=\begin{pmatrix}0\\R\end{pmatrix}.
$$

Its [determinant](../../../../determinant.md) is the nonzero [Wronskian](../../../../wronskian.md) $W$. [Cramer's rule](../../../../cramer-s-rule.md) gives $t_1'=-u_2R/W$ and $t_2'=u_1R/W$, and [integration](../../../../integral-split.md) gives the stated antiderivatives. Their [integration](../../../../integral-split.md) constants only add homogeneous solutions. The construction applies on a regular interval where the forcing and coefficients are defined and $W\ne0$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [12](../../12.md)
3. [2019 resit](../../../2019-resit-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
