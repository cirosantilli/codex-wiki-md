<h1 id="12g/solution">Solution</h1>

↑ **Parent:** [12G](../12g.md)

For [stereographic projection](../../../../../stereographic-projection.md), choose the north pole $N=(0,0,1)$ of the [unit sphere](../../../../../unit-sphere.md) and identify the plane $Z=0$ with the [complex plane](../../../../../complex-plane.md) by $z=X+iY$. Project a point $P=(X,Y,Z)\ne N$ along the line joining it to $N$; adjoin $z=\infty$ for the north pole to identify the whole [sphere](../../../../../sphere.md) with the [Riemann sphere](../../../../../riemann-sphere.md). A point of that line is $N+t(P-N)$. Its last coordinate vanishes when $t=1/(1-Z)$, giving

$$
\boxed{z=\frac{X+iY}{1-Z}.}
$$

Using $X^2+Y^2+Z^2=1$, or solving this line's second intersection with the [sphere](../../../../../sphere.md), gives the inverse

$$
\boxed{X=\frac{2\operatorname{Re}z}{1+|z|^2},\quad Y=\frac{2\operatorname{Im}z}{1+|z|^2},\quad Z=\frac{|z|^2-1}{1+|z|^2}.}
$$

A [great circle](../../../../../great-circle.md) lies in a plane $h_1X+h_2Y+h_3Z=0$ through the origin. Its projected equation is

$$
2h_1\operatorname{Re}z+2h_2\operatorname{Im}z+h_3(|z|^2-1)=0.
$$

It is a straight line only if $h_3=0$, meaning the plane contains the north pole and the south pole. Thus if all three sides of a nondegenerate [spherical triangle](../../../../../spherical-triangle.md) projected to straight sides of a Euclidean triangle, all three distinct side planes would contain both poles. Each pair of side planes could then meet on the [sphere](../../../../../sphere.md) only at those same two poles, which cannot supply three distinct triangle vertices. **A nondegenerate [spherical triangle](../../../../../spherical-triangle.md) cannot project to a Euclidean triangle.** If a side passes through the projection pole, its image is unbounded and also cannot be a finite triangle side.

A nonidentity [rotation in three dimensions](../../../../../rotation-in-three-dimensions.md) has an axis through the origin: an orthogonal three-by-three [matrix](../../../../../matrix.md) of determinant one has an [eigenvalue](../../../../../eigenvalue.md) one, since nonreal [eigenvalues](../../../../../eigenvalue.md) pair as conjugates, real [eigenvalues](../../../../../eigenvalue.md) are $\pm1$, and their product is one. Its axis meets the [unit sphere](../../../../../unit-sphere.md) in an [antipodal pair](../../../../../antipodal-pair.md), which is fixed. In the identity case every point is fixed, so an [antipodal pair](../../../../../antipodal-pair.md) can again be selected. Projecting $P$ and $-P$ gives

$$
p=\frac{X+iY}{1-Z},\qquad q=-\frac{X+iY}{1+Z},\qquad p\overline q=-\frac{X^2+Y^2}{1-Z^2}=-1
$$

whenever both points are finite. Thus the associated [Möbius transformation](../../../../../mobius-transformation.md) fixes an [antipodal pair](../../../../../antipodal-pair.md) satisfying the claimed relation. **The universally valid relation is $q=-1/\overline p$ on the [Riemann sphere](../../../../../riemann-sphere.md)**, with $0$ and $\infty$ paired. A rotation about the projection axis fixes exactly that pair, so the PDF's literal finite product needs this extended-coordinate convention. This is the [antipodal stereographic coordinate relation](../../../../../antipodal-stereographic-coordinate-relation.md).

## ↑ Ancestors (10)

1. [12G](../12g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
