<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $h=x-x_0$, $k=y-y_0$, and let $a=f_{xx}$, $b=f_{xy}$ and $c=f_{yy}$ be evaluated at the [critical point](../../../../../../critical-point.md). Assuming $f$ is twice continuously differentiable nearby, the [Taylor expansion](../../../../../../taylor-expansion.md) is

$$
f(x_0+h,y_0+k)-f(x_0,y_0)
=\frac12(ah^2+2bhk+ck^2)+o(h^2+k^2).
$$

The linear terms vanish because the [gradient](../../../../../../gradient.md) is zero. For $a>0$, [completing the square](../../../../../../completing-the-square.md) gives

$$
\frac12(ah^2+2bhk+ck^2)=\frac1{2a}\left((ah+bk)^2+(ac-b^2)k^2\right).
$$

Consequently the requested constant is the [Hessian determinant](../../../../../../hessian-determinant.md)

$$
\boxed{D=f_{xx}f_{yy}-f_{xy}^2.}
$$

The displayed identity in the question is an identity for the quadratic part; for a general $f$, its right-hand side needs the remainder $o(h^2+k^2)$.

If $D>0$, the [quadratic form](../../../../../../quadratic-form-split.md) is positive for every nonzero $(h,k)$. On the [unit circle](../../../../../../complex-unit-circle.md) it has a positive minimum, so it dominates the remainder sufficiently near the [critical point](../../../../../../critical-point.md). Hence the point is a **strict [local minimum](../../../../../../local-minimum.md)**.

If $D<0$, along $k=0$ the quadratic term is $ah^2/2>0$, whereas along $h=-bk/a$ it is $Dk^2/(2a)<0$. Along each line the remainder is of smaller order. Thus values both above and below $f(x_0,y_0)$ occur arbitrarily nearby, giving a **[saddle point](../../../../../../saddle-point.md)**.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [Mathematics III](../../../mathematics-iii-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
