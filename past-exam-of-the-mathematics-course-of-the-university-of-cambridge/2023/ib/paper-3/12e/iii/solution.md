<h1 id="12e/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The tangent plane

$$
\boxed{x=1}
$$

cuts the hyperboloid in

$$
y^2=z^2,
$$

so its intersection is the pair of straight lines

$$
\gamma_\pm(t)=(1,\pm t,t).
$$

Their [accelerations](../../../../../../acceleration.md) vanish, hence are normal to the surface, so both lines are geodesics. Their [tangent vectors](../../../../../../tangent-vector.md) at their intersection $(1,0,0)$ are $(0,1,1)$ and $(0,-1,1)$, whose [inner product](../../../../../../inner-product.md) is zero. They therefore intersect at a [right angle](../../../../../../right-angle.md), giving the second case of [plane-section geodesics of the unit one-sheet hyperboloid](../../../../../../plane-section-geodesics-of-the-unit-one-sheet-hyperboloid.md).

There are also geodesics entirely contained in $z>0$. In the coordinates

$$
X(z,\phi)=\left(\sqrt{1+z^2}\cos\phi,
\sqrt{1+z^2}\sin\phi,z\right),
$$

the metric is

$$
\frac{1+2z^2}{1+z^2}\,dz^2+(1+z^2)\,d\phi^2.
$$

For a unit-speed geodesic, the [Clairaut first integral for a surface of revolution](../../../../../../clairaut-first-integral-for-a-surface-of-revolution.md) is $c=(1+z^2)\dot\phi$, and the constant-speed equation becomes

$$
\dot z^2=\frac{1+z^2-c^2}{1+2z^2}.
$$

Choose $c>1$ and initial height $z_0=\sqrt{c^2-1}$. The geodesic initially tangent to the parallel has $\dot z=0$, and the displayed identity prevents it from entering $0<z<z_0$. Since the parallel at $z_0>0$ is not itself a geodesic, the curve turns there and otherwise has $z>z_0$. Hence it remains entirely in $z>0$; this is a [geodesic trapped in one half of the unit one-sheet hyperboloid](../../../../../../geodesic-trapped-in-one-half-of-the-unit-one-sheet-hyperboloid.md).

Finally, the waist

$$
\gamma(t)=(\cos t,\sin t,0)
$$

is a geodesic and is preserved setwise by every [isometry](../../../../../../isometry.md) of the hyperboloid. Indeed, its [Gaussian curvature](../../../../../../gaussian-curvature.md) is

$$
K(z)=-\frac1{(1+2z^2)^2}.
$$

The value $K=-1$ occurs exactly at $z=0$. Since [Gaussian curvature](../../../../../../gaussian-curvature.md) is intrinsic and therefore preserved by [isometries](../../../../../../isometry.md), every isometry preserves the waist. Thus the answer to the final question is also yes, with the [isometry-invariant waist geodesic of the unit one-sheet hyperboloid](../../../../../../isometry-invariant-waist-geodesic-of-the-unit-one-sheet-hyperboloid.md) as an example.

<a id="12e/iii/image-plane-section-geodesics-on-the-unit-one-sheet-hyperboloid"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-3-hyperboloid-geodesics.png)

**[Figure 1](#12e/iii/image-plane-section-geodesics-on-the-unit-one-sheet-hyperboloid). Plane-section geodesics on the unit one-sheet hyperboloid**. Blue meridians are disjoint geodesics in the plane y equals zero, red ruling lines are geodesics meeting orthogonally in the tangent plane x equals one, and the purple waist is an isometry-invariant geodesic.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [12E](../../12e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
