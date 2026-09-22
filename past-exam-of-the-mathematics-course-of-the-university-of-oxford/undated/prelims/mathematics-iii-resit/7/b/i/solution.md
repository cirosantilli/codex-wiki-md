<h1 id="7/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Differentiate the [ordinary least squares](../../../../../../../ordinary-least-squares.md) objective in [a](../../a.md). Its [normal equations for linear least squares](../../../../../../../normal-equations-for-linear-least-squares.md) are

$$
\sum_i(Y_i-\widehat\alpha-\widehat\beta x_i)=0,\qquad
\sum_i x_i(Y_i-\widehat\alpha-\widehat\beta x_i)=0.
$$

Using $\sum_i x_i=0$ and $S_{xx}=\sum_i x_i^2>0$ gives

$$
\boxed{\widehat\alpha=\overline Y,\qquad
\widehat\beta=\frac{\sum_i x_iY_i}{S_{xx}}.}
$$

The [Hessian matrix](../../../../../../../hessian-matrix.md) of the objective in $(a,b)$ is $2\operatorname{diag}(n,S_{xx})$, which is [positive-definite](../../../../../../../positive-definite-bilinear-form.md), so this is its unique [global minimum](../../../../../../../global-minimum.md). For the observed [estimates](../../../../../../../statistical-estimate.md), replace $Y_i$ by $y_i$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Mathematics III resit](../../../../mathematics-iii-resit-split.md)
5. [Prelims](../../../../split.md)
6. [Undated](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
