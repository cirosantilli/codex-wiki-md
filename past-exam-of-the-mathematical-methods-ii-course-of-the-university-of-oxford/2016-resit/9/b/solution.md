<h1 id="9/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In the positive quadrant, the inverse transformation is single-valued:

$$
x=\sqrt{v/u},\qquad y=\sqrt{uv}.
$$

The two rays become $1\le u\le2$ and the two [hyperbolas](../../../../hyperbola.md) become $1\le v\le3$, so the curved original region becomes a rectangle. These are the middle two panels of the figure in part 2i. The forward [Jacobian determinant](../../../../jacobian-determinant.md) is

$$
\frac{\partial(u,v)}{\partial(x,y)}
=\begin{vmatrix}-y/x^2&1/x\\y&x\end{vmatrix}=-2u,
\qquad dx\,dy=\frac{du\,dv}{2u}.
$$

Since $x^3y=v^2/u$, the required [double integral](../../../../double-integral.md) is

$$
\int_1^2\int_1^3\frac{v^2}{2u^2}\,dv\,du
=\frac12\left(\frac12\right)\left(\frac{26}{3}\right)
=\boxed{\frac{13}{6}.}
$$

The signs of $x,y$ and $u>0$ justify the chosen square-root branch and the simplified absolute [Jacobian determinant](../../../../jacobian-determinant.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [9](../../9.md)
3. [2016 resit](../../../2016-resit-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
