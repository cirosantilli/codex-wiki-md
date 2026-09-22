<h1 id="11/solution">Solution</h1>

↑ **Parent:** [11](../11.md)

Since $\boldsymbol n\cdot\boldsymbol n=1$, the [vector](../../../../vector.md) $K\boldsymbol r$ is perpendicular to $\boldsymbol n$:

$$
\boldsymbol n\cdot K\boldsymbol r=\boldsymbol n\cdot\boldsymbol r-(\boldsymbol n\cdot\boldsymbol r)(\boldsymbol n\cdot\boldsymbol n)=0.
$$

It follows that $K^2\boldsymbol r=K\boldsymbol r$. If $\boldsymbol r=t\boldsymbol n$, then $K\boldsymbol r=0$; if $\boldsymbol n\cdot\boldsymbol r=0$, then $K\boldsymbol r=\boldsymbol r$. Thus $K=I-\boldsymbol n\boldsymbol n^T$ is the [orthogonal projection matrix](../../../../orthogonal-projection-matrix.md) onto $\boldsymbol n^\perp$: it removes exactly the component normal to the plane.

For the equally inclined plane choose $\boldsymbol n=(1,1,1)/\sqrt3$. Reversing its sign gives the same plane; other sign choices give equivalent reflections of the coordinate axes. One suitable [orthonormal basis](../../../../orthonormal-basis.md) of this plane is

$$
\boldsymbol e_1=\frac{(1,1,-2)}{\sqrt6},\qquad \boldsymbol e_2=\frac{(-1,1,0)}{\sqrt2}.
$$

Their [dot products](../../../../dot-product.md) with $\boldsymbol n$ vanish, their lengths are one, and their mutual [dot product](../../../../dot-product.md) is zero. The equal first two components of $\boldsymbol e_1$ give its equal inclinations to $\boldsymbol i,\boldsymbol j$. Because $\boldsymbol e_j$ is already in the projection plane, $\boldsymbol e_j\cdot K\boldsymbol r=\boldsymbol e_j\cdot\boldsymbol r$. The coordinates of the projected point are therefore

$$
\boxed{u=\frac{x+y-2z}{\sqrt6},\qquad v=\frac{-x+y}{\sqrt2}.}
$$

For a [circle](../../../../circle.md) of radius $R$ centered at the origin in $z=0$, its equation $x^2+y^2=R^2$ becomes $3u^2+v^2=R^2$. This is an [ellipse](../../../../ellipse.md) with semiaxes $R/\sqrt3$ and $R$. Translating the original center only translates its [orthogonal projection](../../../../orthogonal-projection.md), so the result applies to every circle in that plane. Consequently

$$
\boxed{\frac{\text{minor axis}}{\text{major axis}}=\frac1{\sqrt3}.}
$$

The general reason is the [orthogonal projection of a circle between planes](../../../../orthogonal-projection-of-a-circle-between-planes.md): the direction common to the planes retains its length, while the perpendicular direction is shortened by the cosine of their angle.

## ↑ Ancestors (12)

1. [11](../11.md)
2. [Paper 1](../../paper-1-split.md)
3. [2008](../../split.md)
4. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
