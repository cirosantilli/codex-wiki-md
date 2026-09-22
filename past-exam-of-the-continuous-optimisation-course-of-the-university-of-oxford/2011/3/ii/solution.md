<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The equality [gradients](../../../../gradient.md) are independent everywhere. At an interior point of the ellipsoid, there is no active inequality, so the [Mangasarian–Fromovitz constraint qualification](../../../../mangasarian-fromovitz-constraint-qualification.md) holds. At a boundary point $x=x_0+z$, a qualifying direction must satisfy $Av=0$ and $2x^TQv<0$.

If $\rho^2<1$, choose $v=x_0-x=-z$. At a boundary point $z^TQz=1-\rho^2>0$, and

$$
2x^TQv=-2z^TQz<0.
$$

Thus the qualification holds at every feasible point. If $\rho^2=1$, the only feasible point is $x_0$; for every $v\in\ker A$, $x_0^TQv=0$, so no strict direction exists. This proves

$$
\boxed{\text{MFCQ at one feasible point}\iff\rho^2<1
\iff\text{MFCQ at every feasible point}.}
$$

The equivalence also identifies this case with strict feasibility of the inequality on the affine equality space.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the continuous optimisation course of the University of Oxford](../../../split.md)
5. [Continuous optimisation course of the University of Oxford](../../../../continuous-optimisation-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
