<h1 id="11/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The stationarity equations are $4x^3-16y=0$ and $4y^3-16x=0$. Thus $y=x^3/4$ and $x=y^3/4$, so $x(x^8-256)=0$. The real solutions are $(0,0)$, $(2,2)$ and $(-2,-2)$. The [Hessian matrix](../../../../hessian-matrix.md) is

$$
H=\begin{pmatrix}12x^2&-16\\-16&12y^2\end{pmatrix}.
$$

At the origin its determinant is $-256$, giving a saddle. At either nonzero stationary point it has eigenvalues $32,64$, so both are strict minima, with value $-32$:

$$
\boxed{(0,0):\text{saddle},\quad f=0;\qquad (2,2),(-2,-2):\text{minima},\quad f=-32.}
$$

They are also global minima, because $f=(x^2-y^2)^2+2(xy-4)^2-32\geq-32$, with equality exactly at those two points. This is the special coefficient choice in a [quartic double well with bilinear coupling](../../../../quartic-double-well-with-bilinear-coupling.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [11](../../11.md)
3. [2013 resit](../../../2013-resit-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
