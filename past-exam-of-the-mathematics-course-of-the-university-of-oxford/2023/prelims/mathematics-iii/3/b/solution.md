<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a twice [continuously differentiable function](../../../../../../continuously-differentiable-function.md), an interior [local extremum](../../../../../../local-extremum.md) requires $f_x=f_y=0$. At such a [critical point](../../../../../../critical-point.md), put $D=f_{xx}f_{yy}-f_{xy}^2$. The [second-derivative test](../../../../../../second-derivative-test.md) gives a strict [local minimum](../../../../../../local-minimum.md) if $D>0$ and $f_{xx}>0$, a strict [local maximum](../../../../../../local-maximum.md) if $D>0$ and $f_{xx}<0$, and a [saddle point](../../../../../../saddle-point.md) if $D<0$. When $D=0$, the test is inconclusive. More generally the [Hessian matrix](../../../../../../hessian-matrix.md) is necessarily [positive semidefinite](../../../../../../positive-semidefinite-matrix.md) at a [local minimum](../../../../../../local-minimum.md) and [negative semidefinite](../../../../../../negative-semidefinite-matrix.md) at a [local maximum](../../../../../../local-maximum.md), but these non-strict signs alone are not sufficient.

For this [polynomial](../../../../../../polynomial-split.md),

$$
f_x=2x+2y-y^2,\quad f_y=2x+2y-2xy,\quad
H=\begin{pmatrix}2&2-2y\\2-2y&2-2x\end{pmatrix}.
$$

Subtracting the two stationarity equations gives $y(2x-y)=0$. If $y=0$, then $x=0$; if $y=2x$, the remaining equation gives $x=0$ or $x=3/2$. Thus the only [critical points](../../../../../../critical-point.md) are $(0,0)$ and $(3/2,3)$.

At $(3/2,3)$, $\det H=-18<0$, so it is a [saddle point](../../../../../../saddle-point.md). At $(0,0)$ the determinant is zero, but along $y=-x$ the value is $-x^3$, which takes both signs arbitrarily near zero. Therefore

$$
\boxed{(0,0)\text{ and }(3/2,3)\text{ are both saddle points}.}
$$

In particular a vanishing [Hessian determinant](../../../../../../hessian-determinant.md) does not exclude a [saddle point](../../../../../../saddle-point.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [Mathematics III](../../../mathematics-iii-split.md)
4. [Prelims](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
