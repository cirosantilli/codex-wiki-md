<h1 id="11/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use only the [dot product](../../../../../../dot-product.md) to minimize the squared [Euclidean distance](../../../../../../euclidean-distance.md) from the origin:

$$
D(t)^2=(\boldsymbol a_2+t\boldsymbol n_2)\cdot(\boldsymbol a_2+t\boldsymbol n_2)
=\|\boldsymbol a_2\|^2+2t(\boldsymbol a_2\cdot\boldsymbol n_2)+t^2\|\boldsymbol n_2\|^2.
$$

Completing the square gives

$$
D(t)^2=\|\boldsymbol n_2\|^2
\left(t+\frac{\boldsymbol a_2\cdot\boldsymbol n_2}{\|\boldsymbol n_2\|^2}\right)^2
+\|\boldsymbol a_2\|^2-
\frac{(\boldsymbol a_2\cdot\boldsymbol n_2)^2}{\|\boldsymbol n_2\|^2}.
$$

The square is minimized at $t_0=-(\boldsymbol a_2\cdot\boldsymbol n_2)/\|\boldsymbol n_2\|^2$, yielding

$$
\boxed{d_0=\sqrt{\boldsymbol a_2\cdot\boldsymbol a_2
-\frac{(\boldsymbol a_2\cdot\boldsymbol n_2)^2}{\boldsymbol n_2\cdot\boldsymbol n_2}}.}
$$

Geometrically this subtracts the squared length of the [orthogonal projection](../../../../../../orthogonal-projection.md) parallel to the line. At the minimizing point, $(\boldsymbol a_2+t_0\boldsymbol n_2)\cdot\boldsymbol n_2=0$, as required for perpendicular distance.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [C](../../c.md)
3. [11](../../../11.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
