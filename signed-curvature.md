# Signed curvature

↑ **Parent:** [Curvature](curvature.md)

Fix the standard [orientation of a vector space](orientation-of-a-vector-space.md) on the plane. For an oriented [regular curve](regular-curve.md) in that plane, let $T=(T_x,T_y)$ be its [unit tangent vector](unit-tangent-vector.md) and let $N_L=(-T_y,T_x)$ be its left [unit normal](unit-normal.md), obtained by an anticlockwise [rotation](rotation-mathematics.md) through $\pi/2$. Its [signed curvature](signed-curvature.md) $k$, also commonly written $\kappa_s$, is defined by

$$
\frac{dT}{ds}=kN_L,\qquad k=\det\!\left(T,\frac{dT}{ds}\right),\qquad \kappa=|k|.
$$

Here $s$ increases with the chosen traversal and $\det$ is the [determinant](determinant.md). Positive [signed curvature](signed-curvature.md) means turning left; negative [signed curvature](signed-curvature.md) means turning right. The left [unit normal](unit-normal.md) exists even when $k=0$; when $k<0$ it points opposite to the [principal normal vector](principal-normal-vector.md). See [Ghomi's university lecture notes, section 1.10](https://ghomi.math.gatech.edu/LectureNotes/LectureNotes4U.pdf).

For an arbitrary regular [parametric curve](parametric-curve.md) $r(t)=(x(t),y(t))$ traversed with increasing $t$, the [signed curvature](signed-curvature.md) is

$$
k(t)=\frac{x'(t)y''(t)-y'(t)x''(t)}{\bigl(x'(t)^2+y'(t)^2\bigr)^{3/2}}.
$$

For the anticlockwise [circle](circle.md) $r(t)=(R\cos t,R\sin t)$, the numerator is $R^2$ and the denominator is $R^3$, so $k=1/R$. For the clockwise traversal $q(t)=(R\cos t,-R\sin t)$, the numerator is $-R^2$, so $k=-1/R$, while unsigned [curvature](curvature.md) is $1/R$ in both cases. On this [circle](circle.md) $N_L$ points inward for anticlockwise traversal and outward for clockwise traversal. For any simple closed [regular curve](regular-curve.md) traversed anticlockwise, $N_L$ is the inward [unit normal](unit-normal.md), but [signed curvature](signed-curvature.md) can still be negative along nonconvex portions.

<a id="image-reversing-traversal-reverses-signed-curvature-and-the-left-normal-but-preserves-the-bend"></a>
![](signed-curvature-orientation.png)

**[Figure 4](#image-reversing-traversal-reverses-signed-curvature-and-the-left-normal-but-preserves-the-bend). Reversing traversal reverses signed curvature and the left normal, but preserves the bend**.

To see why the formula uses the cube of the [speed](speed.md), write $r'=vT$ and $r''=v'T+v^2(dT/ds)$. The term parallel to $T$ contributes zero to the [determinant](determinant.md), giving $\det(r',r'')=v^3\det(T,dT/ds)=v^3k$. Under a [reparametrization](reparametrization.md) $q(u)=r(\phi(u))$ with $\phi'\ne0$, the numerator gains a factor $(\phi')^3$ and the denominator gains $|\phi'|^3$. Thus orientation-preserving [reparametrization](reparametrization.md) preserves [signed curvature](signed-curvature.md), while reversing traversal changes its sign at corresponding points. Unsigned [curvature](curvature.md) is preserved in either case.

Locally write the [unit tangent vector](unit-tangent-vector.md) as $T=(\cos\theta,\sin\theta)$. Differentiating with respect to [arc length](arc-length.md) gives $k=d\theta/ds$: [signed curvature](signed-curvature.md) records the direction as well as the amount of turning. Its integral therefore measures net turning, as in the [turning tangent theorem](turning-tangent-theorem.md); the integral of $|k|$ is [total curvature](total-curvature.md) and counts both left and right turns positively.

**Table of contents**

- [Turning tangent theorem](turning-tangent-theorem.md)

## ↑ Ancestors (6)

1. [Curvature](curvature.md)
2. [Differential geometry](differential-geometry-split.md)
3. [Geometry and topology](geometry-and-topology-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Curvature of a plane curve](curvature-of-a-plane-curve.md)
- [Intrinsic curvature of an elastic filament](intrinsic-curvature-of-an-elastic-filament.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-2/25h/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-67/2/solution.md)
- [Signed curvature](signed-curvature.md)
- [Turning tangent theorem](turning-tangent-theorem.md)
