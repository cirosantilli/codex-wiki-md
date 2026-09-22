<h1 id="12/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The first [partial derivatives](../../../../../../partial-derivative.md) factor as

$$
g_x=4x(2+x^2-3y^2),\qquad g_y=4y(2+y^2-3x^2).
$$

If either coordinate vanishes, the other equation forces the other coordinate to vanish as well. If both are nonzero, subtracting the two bracket equations gives $x^2=y^2$, and then $x^2=y^2=1$. Thus the complete list of [stationary points](../../../../../../stationary-point.md) is $(0,0)$ and the four points $(\pm1,\pm1)$.

The [Hessian matrix](../../../../../../hessian-matrix.md) is

$$
H_g=\begin{pmatrix}8+12x^2-12y^2&-24xy\\-24xy&8+12y^2-12x^2\end{pmatrix}.
$$

At the origin it is $8I$, which is a [positive-definite matrix](../../../../../../positive-definite-matrix.md). At the four other points its [eigenvalues](../../../../../../eigenvalue.md) are $32$ and $-16$, independently of the signs. The [second-derivative test](../../../../../../second-derivative-test.md) therefore gives

$$
\boxed{(0,0):\text{ strict local minimum, }g=0;\qquad
(\pm1,\pm1):\text{ saddle points, }g=4.}
$$

There are no [local maxima](../../../../../../local-maximum.md). The minimum at the origin is not global, since $g(t,t)=8t^2-4t^4\to-\infty$ as $|t|\to\infty$.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [12](../../../12.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
