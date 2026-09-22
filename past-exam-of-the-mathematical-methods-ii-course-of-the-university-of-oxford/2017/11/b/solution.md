<h1 id="11/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An interior [stationary point](../../../../stationary-point.md) has $f_x=f_y=0$. Assuming twice continuous differentiability nearby, the two-dimensional [Taylor series](../../../../taylor-series.md) about it is

$$
f(p+h)=f(p)+\frac12h^THh+o(|h|^2),\qquad
H=\begin{pmatrix}A&B\\B&C\end{pmatrix},
$$

where $A=f_{xx}$, $B=f_{xy}$ and $C=f_{yy}$. Let $D=AC-B^2$. The [second-derivative test](../../../../second-derivative-test.md) gives a strict local minimum if $D>0,A>0$, a strict local maximum if $D>0,A<0$, and a [saddle point](../../../../saddle-point.md) if $D<0$.

For example, if $A\ne0$, the quadratic form is $A(h_x+Bh_y/A)^2+(D/A)h_y^2$, which proves these sign tests. If $D=0$, the quadratic part is inconclusive: $x^4+y^4$ has a minimum while $x^4-y^4$ has a saddle at the origin, although both have zero [Hessian matrix](../../../../hessian-matrix.md) there. Higher-order terms or direct inequalities must then be examined.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [11](../../11.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
