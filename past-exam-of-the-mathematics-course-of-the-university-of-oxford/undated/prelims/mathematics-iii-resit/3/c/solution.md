<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $A=a^2>0$ and $E=e^{-(x^2+y^2)/A}>0$. The [partial derivatives](../../../../../../partial-derivative.md) factor as

$$
f_x=2xE\left(1-\frac{x^2-2y^2}{A}\right),\qquad
f_y=-2yE\left(2+\frac{x^2-2y^2}{A}\right).
$$

A [critical point](../../../../../../critical-point.md) has both [partial derivatives](../../../../../../partial-derivative.md) zero. If $x,y\ne0$, this would require $x^2-2y^2=A$ and $x^2-2y^2=-2A$, which is impossible. On the axes the remaining conditions give

$$
\boxed{(0,0),\quad(\pm|a|,0),\quad(0,\pm|a|).}
$$

At either [critical point](../../../../../../critical-point.md) with $x\ne0$, the [Hessian matrix](../../../../../../hessian-matrix.md) is

$$
H_f=\begin{pmatrix}-4/e&0\\0&-6/e\end{pmatrix}.
$$

It is [negative definite](../../../../../../negative-definite-matrix.md), so the [second-derivative test](../../../../../../second-derivative-test.md) shows that **both $(\pm|a|,0)$ are strict [local maxima](../../../../../../local-maximum.md)**, of value $a^2/e$. They also attain the [global maximum](../../../../../../global-maximum.md): $f\le x^2e^{-x^2/A}\le A/e$. For completeness, the [Hessian matrix](../../../../../../hessian-matrix.md) at $(0,\pm|a|)$ is $\operatorname{diag}(6/e,8/e)$, giving strict [local minima](../../../../../../local-minimum.md), while at the origin it is $\operatorname{diag}(2,-4)$, giving a [saddle point](../../../../../../saddle-point.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [Mathematics III resit](../../../mathematics-iii-resit-split.md)
4. [Prelims](../../../split.md)
5. [Undated](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
