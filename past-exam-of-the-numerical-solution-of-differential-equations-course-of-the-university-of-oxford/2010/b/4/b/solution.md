<h1 id="b/4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

At $x_r=rh$, the [central finite difference](../../../../../central-finite-difference.md) equations are

$$
-\frac{U_{r+1}-2U_r+U_{r-1}}{h^2}
+p_r\frac{U_{r+1}-U_{r-1}}{2h}+q_rU_r=f(x_r,U_r),\quad1\leq r\leq m-1,
$$

with $U_0=\alpha$, $U_m=\beta$. For $f=f(x)$ this is a [linear system](../../../../../system-of-linear-equations.md) $A_hU_h=b_h$, with row coefficients

$$
a_r=-h^{-2}-p_r/(2h),\quad d_r=2h^{-2}+q_r,\quad c_r=-h^{-2}+p_r/(2h).
$$

The right-hand side starts from $f(x_r)$ and includes $-a_1\alpha$ in its first entry and $-c_{m-1}\beta$ in its last entry. Under $h\max p<2$, both off-diagonal coefficients are negative, so $|a_r|+|c_r|=2h^{-2}<d_r$. Omitting nonexistent endpoint columns can only reduce this sum. Therefore **$A_h$ is strictly diagonally dominant**. In particular the linear discrete system is nonsingular.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the numerical solution of differential equations course of the University of Oxford](../../../../split.md)
6. [Numerical solution of differential equations course of the University of Oxford](../../../../../numerical-solution-of-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
