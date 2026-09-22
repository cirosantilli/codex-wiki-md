<h1 id="11/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [gradient](../../../../gradient.md) equations are $y=x^3$ and $x=y^3$. Their real solutions are $(0,0)$, $(1,1)$ and $(-1,-1)$. The [Hessian matrix](../../../../hessian-matrix.md) is $\begin{pmatrix}-12x^2&4\\4&-12y^2\end{pmatrix}$, so the origin has [eigenvalues](../../../../eigenvalue.md) $\pm4$ and is a [saddle point](../../../../saddle-point.md), with value zero. At either other point the [eigenvalues](../../../../eigenvalue.md) are $-8,-16$, giving strict maxima with value two. They are global maxima because

$$
4xy-x^4-y^4\le4xy-2x^2y^2=2-2(xy-1)^2\le2,
$$

and equality occurs precisely at those two points.

In [polar coordinates](../../../../polar-coordinates.md), the zero contour is

$$
0=2r^2\sin2\theta-r^4(\cos^4\theta+\sin^4\theta).
$$

Besides the saddle $r=0$, its nonzero branches satisfy

$$
\boxed{r^2=\frac{2\sin2\theta}{\cos^4\theta+\sin^4\theta}
=\frac{8\sin2\theta}{3+\cos4\theta}.}
$$

The denominator is positive; real radii require $\sin2\theta\ge0$. The branches form two closed lobes in the first and third quadrants, meeting at the origin. Positive contours lie inside these lobes around the maxima, and negative contours extend outside. Along the coordinate axes the function is negative away from the saddle, whereas along $y=x$ it is initially positive; these signs show the crossing geometry in the sketch.

## ↑ Ancestors (12)

1. [D](../d.md)
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
