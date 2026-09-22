<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

The [gradient](../../../gradient.md) equations are $f_x=2x(1-y)=0$ and $f_y=4y-x^2=0$. The [critical points](../../../critical-point.md) are $(0,0)$ and $(\pm2,1)$. Their [Hessian matrix](../../../hessian-matrix.md) is

$$
H=\begin{pmatrix}2-2y&-2x\\-2x&4\end{pmatrix}.
$$

At the origin $H=\operatorname{diag}(2,4)$ is positive definite. At either other point its [determinant](../../../determinant.md) is $-16$, so its [eigenvalues](../../../eigenvalue.md) have opposite signs. Thus

$$
\boxed{(0,0)\text{ is a strict local minimum},\qquad (2,1),(-2,1)\text{ are saddle points}.}
$$

The minimum value is zero and both saddle values are two. The origin is not a global minimum: at any fixed $y>1$, the term $(1-y)x^2$ makes $f$ arbitrarily negative as $|x|$ increases.

For the [contour plot](../../../contour-plot.md), the local contours around the origin are approximately $x^2+2y^2=c$. The exact saddle contour factors as

$$
f-2=(y-1)(2y+2-x^2),
$$

so it is the union of $y=1$ and $y=x^2/2-1$, crossing at the two saddles. Other levels obey $x^2=(c-2y^2)/(1-y)$ where $y\ne1$; the right panel of the original figure in part 3(a) shows how these branches join around the minimum and pass through the saddle contour.

## ↑ Ancestors (11)

1. [6](../6.md)
2. [2017 resit](../../2017-resit-split.md)
3. [Past exam of the mathematical methods II course of the University of Oxford](../../split.md)
4. [Mathematical methods II course of the University of Oxford](../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
