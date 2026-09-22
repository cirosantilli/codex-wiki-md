<h1 id="9/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The centered regressors make the first [normal equation](../../../../../../../normal-equation.md) read $n\hat\beta_0=\sum_iY_i$. Define

$$
A=\sum_i x_{i1}^2,\quad B=\sum_i x_{i1}x_{i2},\quad C=\sum_i x_{i2}^2,\quad
u=\sum_i x_{i1}Y_i,\quad v=\sum_i x_{i2}Y_i.
$$

The remaining equations are $A\hat\beta_1+B\hat\beta_2=u$ and $B\hat\beta_1+C\hat\beta_2=v$. Provided $D=AC-B^2>0$, [matrix inversion](../../../../../../../matrix-inversion.md) gives

$$
\boxed{\hat\beta_0=\overline Y,\qquad
\hat\beta_1=\frac{Cu-Bv}{D},\qquad \hat\beta_2=\frac{Av-Bu}{D}.}
$$

By the [Cauchy-Schwarz inequality](../../../../../../../cauchy-schwarz-inequality.md), $D\geq0$. If $D=0$, the two regressor columns are [linearly dependent](../../../../../../../linear-dependence.md), and their separate slopes are not uniquely identifiable. One still has well-defined [linear least squares](../../../../../../../linear-least-squares.md) fitted values, but cannot use the displayed divisions by $D$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [9](../../../9.md)
4. [Mathematics III](../../../../mathematics-iii-split.md)
5. [Prelims](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
