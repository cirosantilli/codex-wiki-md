<h1 id="3c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [parallel axis theorem](../../../../../../parallel-axis-theorem.md) says that for an axis through $x$, parallel to the centre-of-mass axis in direction $\hat d$,

$$
I_T(x)=I_T(x_T)+M_T|(x-x_T)\times\hat d|^2.
$$

Let

$$
\rho_A^2=|(x_A-x_C)\times\hat d|^2,
\qquad
\rho_B^2=|(x_B-x_C)\times\hat d|^2.
$$

Moments about the axis through $x_C$ add, so

$$
I_C(x_C)=I_A(x_A)+M_A\rho_A^2
+I_B(x_B)+M_B\rho_B^2.
$$

Using $M_A=M_C-M_B$ and solving gives

$$
\boxed{
M_B=\frac{I_C(x_C)-I_A(x_A)-I_B(x_B)-M_C\rho_A^2}
{\rho_B^2-\rho_A^2}}
$$

when the denominator is nonzero. In the degenerate equal-distance case, this inertia equation alone does not determine $M_B$; the centre-of-mass equation $M_Cx_C=M_Ax_A+M_Bx_B$ supplies the remaining information.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3C](../../3c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
