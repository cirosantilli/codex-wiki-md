<h1 id="question-1/a/solution">Solution</h1>

↑ **Parent:** [a](../a.md)

Put $r=\sqrt{x^2+y^2}$. The definitions of the [parabolic polar coordinates](../../../../../../parabolic-polar-coordinates.md) give $u^2=x+r$ and $v^2=-x+r$. Subtracting and multiplying these equations yields

$$
u^2-v^2=2x,\qquad u^2v^2=r^2-x^2=y^2.
$$

Since $u,v,y\geq0$, taking the nonnegative [square root](../../../../../../square-root.md) gives

$$
\boxed{x=\frac{u^2-v^2}{2},\qquad y=uv}.
$$

The [Jacobian matrix](../../../../../../jacobian-matrix.md) has columns $(u,v)$ and $(-v,u)$. Its [Jacobian determinant](../../../../../../jacobian-determinant.md) is therefore

$$
\frac{\partial(x,y)}{\partial(u,v)}
=\det\begin{pmatrix}u&-v\\v&u\end{pmatrix}
=\boxed{u^2+v^2}.
$$

Here the displayed fraction denotes the [Jacobian determinant](../../../../../../jacobian-determinant.md), as in the paper. The [change of variables formula](../../../../../../change-of-variables-formula.md) consequently gives $dx\,dy=(u^2+v^2)\,du\,dv$. The [Jacobian determinant](../../../../../../jacobian-determinant.md) is positive except at the origin, and the definitions supply the unique nonnegative inverse throughout the region $y\geq0$.

## ↑ Ancestors (12)

1. [a](../a.md)
2. [Question 1](../../question-1.md)
3. [Mathematics V resit](../../../mathematics-v-resit-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
