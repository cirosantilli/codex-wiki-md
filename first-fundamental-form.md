# First fundamental form

↑ **Parent:** [Differential geometry](differential-geometry-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/First_fundamental_form)

The first fundamental form of a [smooth surface](smooth-surface.md) $S\subseteq\mathbb R^3$ is the restriction of the ambient [inner product](inner-product-split.md) to each [tangent space](tangent-space.md) $T_pS$. For a regular [parametric surface](parametric-surface.md) $X(u,v)$, it is

$$
I=E\,du^2+2F\,du\,dv+G\,dv^2,
\qquad
E=X_u^2,\quad F=X_u\cdot X_v,\quad G=X_v^2.
$$

Here $X_u^2$ means $X_u\cdot X_u$, not a componentwise square. The coefficients form the [Gram matrix](gram-matrix.md) of the two coordinate [tangent vectors](tangent-vector-split.md). Regularity makes this a [positive-definite matrix](positive-definite-matrix.md), so $E>0$ and $EG-F^2>0$.

To calculate the [length of a curve](length-of-a-curve.md) $\gamma(t)=X(u(t),v(t))$, apply the [chain rule](chain-rule.md) and integrate its speed:

$$
L(\gamma)=\int\sqrt{E\dot u^2+2F\dot u\dot v+G\dot v^2}\,dt.
$$

The same [inner product](inner-product-split.md) gives the [angle](angle.md) $\alpha$ between nonzero [tangent vectors](tangent-vector-split.md) $V,W$ through $\cos\alpha=I(V,W)/\sqrt{I(V,V)I(W,W)}$, and gives the [area element](area-element-of-a-surface.md) $dA=\sqrt{EG-F^2}\,du\,dv$ as a positive density. One compact expression therefore supplies rulers, protractors, and [surface area](surface-area.md) measurements.

For the lateral surface of a [circular cylinder](circular-cylinder.md), take the circumferential [arc length](arc-length.md) $u$ rather than the [angle](angle.md):

$$
X(u,v)=\left(R\cos\frac uR,R\sin\frac uR,v\right),\qquad X_u=\left(-\sin\frac uR,\cos\frac uR,0\right),\qquad X_v=(0,0,1).
$$

Direct [inner products](inner-product-split.md) give $E=G=1,F=0$, hence $I=du^2+dv^2$. This is exactly the [Euclidean metric](euclidean-metric.md) on the unrolled [plane](plane.md). For instance, a path with $u=3t,v=4t$, $0\leq t\leq1$, has [length](length.md) $5$ on either surface. Every corresponding path retains its [length](length.md), not merely this example, so sufficiently small neighborhoods retain their intrinsic distances. The [local isometry](local-isometry.md) preserves [angles](angle.md) and [surface areas](surface-area.md) too. Globally $u$ is periodic with period $2\pi R$: unrolling requires a seam, and the whole [circular cylinder](circular-cylinder.md) is not a single planar [manifold chart](manifold-chart.md).

**Table of contents**

- [Local isometry](local-isometry.md)
  - [Local isometries are determined by first-order data](local-isometries-are-determined-by-first-order-data.md)
  - [Complete local isometry is a covering](complete-local-isometry-is-a-covering.md)
  - [Geodesic preservation by a local isometry](geodesic-preservation-by-a-local-isometry.md)
    - [Geodesic-preserving homothety that is not a local isometry](geodesic-preserving-homothety-that-is-not-a-local-isometry.md)
  - [Riemannian isometry](riemannian-isometry.md)
    - [Orientation-reversing Riemannian isometry](orientation-reversing-riemannian-isometry.md)
  - [Local isometry from a circular cone to the plane](local-isometry-from-a-circular-cone-to-the-plane.md)
    - [Geodesics on a punctured circular cone](geodesics-on-a-punctured-circular-cone.md)
- [Area element of a surface](area-element-of-a-surface.md)
  - [Surface area](surface-area.md)
    - [Signed area](signed-area.md)
  - [Vector area element](vector-area-element.md)
    - [Vector area element of an implicit surface](vector-area-element-of-an-implicit-surface.md)
    - [Vector area](vector-area.md)
      - [Vector areas of a closed polyhedron sum to zero](vector-areas-of-a-closed-polyhedron-sum-to-zero.md)
      - [Vector area of a polygonal boundary](vector-area-of-a-polygonal-boundary.md)

## ↑ Ancestors (5)

1. [Differential geometry](differential-geometry-split.md)
2. [Geometry and topology](geometry-and-topology-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (58)

- [Constant-angle geodesic coordinate grids are locally flat](constant-angle-geodesic-coordinate-grids-are-locally-flat.md)
- [Differential geometry](differential-geometry-split.md)
- [Differential geometry of surfaces](differential-geometry-of-surfaces.md)
- [Euler formula for normal curvature](euler-formula-for-normal-curvature.md)
- [First fundamental form of a surface of revolution](first-fundamental-form-of-a-surface-of-revolution.md)
- [Fundamental forms of an elliptic ring torus](fundamental-forms-of-an-elliptic-ring-torus.md)
- [Gaussian curvature](gaussian-curvature.md)
- [Induced metric](induced-metric.md)
- [Line element on a sphere](line-element-on-a-sphere.md)
- [Local isometry from a circular cone to the plane](local-isometry-from-a-circular-cone-to-the-plane.md)
- [Mean curvature](mean-curvature.md)
- [Mean curvature of a catenoid](mean-curvature-of-a-catenoid.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-4/12a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-4/24h/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-66/5/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-2/12h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-3/2h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-2/24h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-15/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-3/12a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-3/2g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-4/12g/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-4/12g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-3/23h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-3/23h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-4/12g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-3/24h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-1/3f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-4/15f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2/22g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-3/21g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-4/15f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-3/14g/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-3/14g/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-3/14g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-4/15g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-3/25i/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-4/25i/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-311/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3/25i/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4/25i/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-1/11f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-3/12e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1/26f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1/26f/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-2/11f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-3/25i/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-2/11f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-3/12e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4/25g/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-3/2g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-1/26j/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-3/25i/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-4/25i/a/solution.md)
- [Second fundamental form of a ring torus](second-fundamental-form-of-a-ring-torus.md)
- [Shape operator](shape-operator.md)
- [Smooth embedded surface](smooth-embedded-surface.md)
- [Theorema Egregium](theorema-egregium.md)
