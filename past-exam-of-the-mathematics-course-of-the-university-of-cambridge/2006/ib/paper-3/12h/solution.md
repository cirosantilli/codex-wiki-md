<h1 id="12h/solution">Solution</h1>

↑ **Parent:** [12H](../12h.md)

Use the unit [sphere](../../../../../sphere.md) $X^2+Y^2+Z^2=1$, its north pole $(0,0,1)$, and the equatorial complex plane $Z=0$. The line from the north pole to a [sphere](../../../../../sphere.md) point meets that plane at

$$
\boxed{z=\frac{X+iY}{1-Z}.}
$$

The north pole maps to $\infty$. The inverse [stereographic projection](../../../../../stereographic-projection.md) is

$$
(X,Y,Z)=\left(\frac{2\Re z}{1+|z|^2},\frac{2\Im z}{1+|z|^2},\frac{|z|^2-1}{1+|z|^2}\right).
$$

The antipodal point has coordinate $w=-(X+iY)/(1+Z)$. Since $X^2+Y^2=(1-Z)(1+Z)$, this is $-1/\bar z$ when both sides are finite and nonzero. Zero and infinity correspond to the two poles and are exchanged by the same extended convention. The inverse formula also proves the converse, giving the [antipodal stereographic coordinate relation](../../../../../antipodal-stereographic-coordinate-relation.md)

$$
\boxed{w=-1/\bar z\iff\text{the sphere points are antipodal}.}
$$

The requested rotation result is that [sphere](../../../../../sphere.md) rotations correspond exactly to [Möbius transformations](../../../../../mobius-transformation.md)

$$
z\longmapsto\frac{az+b}{-\bar b z+\bar a},\qquad |a|^2+|b|^2=1.
$$

The [matrices](../../../../../matrix.md) $\begin{pmatrix}a&b\\-\bar b&\bar a\end{pmatrix}$ form $SU(2)$, and opposite [matrices](../../../../../matrix.md) induce the same transformation. Thus the rotation group $SO(3)$ is identified with $SU(2)/\{\pm I\}$. This is the [sphere rotations as special-unitary Möbius transformations](../../../../../sphere-rotations-as-special-unitary-mobius-transformations.md) result, which need not be proved here.

For a planar [circle](../../../../../circle.md) $|z-c|=r$, $c=a+ib$ and $r>0$, substitute $|z|^2=(1+Z)/(1-Z)$ and $\Re(\bar cz)=(aX+bY)/(1-Z)$. Multiplication by $1-Z$ gives the [circle-plane relation under stereographic projection](../../../../../circle-plane-relation-under-stereographic-projection.md):

$$
-2aX-2bY+(1-|c|^2+r^2)Z+1+|c|^2-r^2=0.
$$

The lift lies in this plane, and conversely its intersection with the [sphere](../../../../../sphere.md) projects onto the [circle](../../../../../circle.md). It is a nondegenerate [circle](../../../../../circle.md) on the [sphere](../../../../../sphere.md). The north pole is not on the displayed plane, since substitution there gives two rather than zero.

A [great circle](../../../../../great-circle.md) is the intersection with a plane through the [sphere](../../../../../sphere.md)'s centre. Here this holds exactly when

$$
\boxed{r^2=1+|c|^2.}
$$

The unit [circle](../../../../../circle.md) lifts to the equator. If a different [circle](../../../../../circle.md) lifts to a [great circle](../../../../../great-circle.md), its plane and the equatorial plane are distinct planes through the origin, so their intersection cuts the [sphere](../../../../../sphere.md) at two antipodal equatorial points. Their planar coordinates are $z$ and $-z$ on $|z|=1$.

Conversely, if the planar [circle](../../../../../circle.md) meets the unit [circle](../../../../../circle.md) in $z$ and $-z$, their lifts are antipodal equatorial points. The plane of the lifted [circle](../../../../../circle.md) contains their midpoint, the origin, so that [circle](../../../../../circle.md) is great. Equivalently, adding $|z-c|^2=r^2$ and $|-z-c|^2=r^2$ gives $r^2=1+|c|^2$. The exclusion of the unit [circle](../../../../../circle.md) ensures the two intersection points are a genuine pair rather than coincident circles. This proves the [antipodal equatorial intersection criterion for a great circle](../../../../../antipodal-equatorial-intersection-criterion-for-a-great-circle.md).

## ↑ Ancestors (10)

1. [12H](../12h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
