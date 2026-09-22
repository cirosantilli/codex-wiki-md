# Curvature

↑ **Parent:** [Differential geometry](differential-geometry-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Curvature)

For a twice continuously differentiable [regular curve](regular-curve.md) $r(t)$ in [Euclidean space](euclidean-norm.md), its unsigned [curvature](curvature.md) measures how quickly its [unit tangent vector](unit-tangent-vector.md) changes per unit [arc length](arc-length.md). Write

$$
v(t)=\|r'(t)\|>0,\qquad \frac{ds}{dt}=v(t),\qquad T(t)=\frac{r'(t)}{v(t)}.
$$

The [curvature](curvature.md) is

$$
\kappa=\left\|\frac{dT}{ds}\right\|=\frac{1}{v(t)}\left\|\frac{dT}{dt}\right\|\geq0,
$$

where the [norm](norm.md) is the [Euclidean norm](euclidean-norm.md). Differentiating with respect to [arc length](arc-length.md) removes the effect of traversal [speed](speed.md); differentiating $T$ with respect to $t$ alone generally does not. See [Ghomi's university lecture notes, section 1.7](https://ghomi.math.gatech.edu/LectureNotes/LectureNotes2U.pdf).

For a [circle](circle.md) of [radius](radius.md) $R>0$, use $r(t)=(R\cos t,R\sin t)$. Then $v=R$, $T=(-\sin t,\cos t)$ and $\|dT/dt\|=1$, giving $\kappa=1/R$. A [straight line](straight-line.md) $r(t)=p+ta$ with $a\ne0$ has constant [unit tangent vector](unit-tangent-vector.md), so $\kappa=0$.

The same [circle](circle.md) traversed as $q(u)=(R\cos(3u),R\sin(3u))$ has [speed](speed.md) $3R$ and $\|dT/du\|=3$: its [curvature](curvature.md) remains $1/R$. By contrast, enlarging the [circle](circle.md) to [radius](radius.md) $2R$ changes its geometry and gives [curvature](curvature.md) $1/(2R)$. More generally, a [dilation](uniform-dilation.md) $r\mapsto ar$ with $a>0$ divides [curvature](curvature.md) by $a$, because it multiplies [arc length](arc-length.md) by $a$ while leaving [unit tangent vectors](unit-tangent-vector.md) unchanged. Thus [curvature](curvature.md) has units of inverse [length](length.md), and a [reparametrization](reparametrization.md) changes neither its value at a corresponding point nor the shape.

Differentiating $T\cdot T=1$, using the [dot product](dot-product.md), shows $T\cdot(dT/ds)=0$: the change is perpendicular to the [unit tangent vector](unit-tangent-vector.md). Wherever $\kappa>0$, the [principal normal vector](principal-normal-vector.md) $N_p=(dT/ds)/\kappa$ points toward the bend. For a [plane curve](plane-curve.md), the [osculating circle](osculating-circle.md) at such a point has [radius of curvature](radius-of-curvature.md) $\rho=1/\kappa$ and center $r+\rho N_p$. It matches the point, [tangent line](tangent-line.md), and [curvature](curvature.md), providing a local circular approximation. At $\kappa=0$ there is no finite [osculating circle](osculating-circle.md) defined by this formula. See [Ghomi's university lecture notes, section 1.13](https://ghomi.math.gatech.edu/LectureNotes/LectureNotes5U.pdf).

This makes [curvature](curvature.md) useful for comparing bends without confusing them with [speed](speed.md). If $t$ denotes time, differentiating $r'=vT$ gives [acceleration](acceleration.md) $r''=v'T+v^2(dT/ds)$, whose component perpendicular to the [unit tangent vector](unit-tangent-vector.md) has magnitude $v^2\kappa$. The [curvature of a plane curve](curvature-of-a-plane-curve.md) example below computes the bend and [osculating circle](osculating-circle.md) of a [parabola](parabola.md) explicitly.

For [smooth surfaces](smooth-surface.md), bending has more than one direction. The [principal curvatures](principal-curvature.md) $k_1,k_2$ instead define [Gaussian curvature](gaussian-curvature.md) $K=k_1k_2$ and [mean curvature](mean-curvature.md) $H=(k_1+k_2)/2$. These are surface quantities, distinct from the [curvature](curvature.md) of an individual [curve](curve.md). In particular, the [circle](circle.md) value $1/R$ must not be confused with the [Gaussian curvature](gaussian-curvature.md) $1/R^2$ of a [sphere](sphere.md) of [radius](radius.md) $R$. See [Ritter's Oxford lecture notes, section 12.2](https://www.maths.ox.ac.uk/system/files/attachments/B3.2%20Geometry%20of%20Surfaces.pdf).

**Table of contents**

- [Signed curvature](signed-curvature.md)
  - [Turning tangent theorem](turning-tangent-theorem.md)
- [Signed curvature of a plane graph](signed-curvature-of-a-plane-graph.md)

## ↑ Ancestors (5)

1. [Differential geometry](differential-geometry-split.md)
2. [Geometry and topology](geometry-and-topology-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (99)

- [Averaged stress-energy of transverse gravitational waves](averaged-stress-energy-of-transverse-gravitational-waves.md)
- [Axisymmetric clamped-plate deflection](axisymmetric-clamped-plate-deflection.md)
- [Bending moment](bending-moment.md)
- [Brans-Dicke theory](brans-dicke-theory.md)
- [Capillary instability of an annular liquid lining](capillary-instability-of-an-annular-liquid-lining.md)
- [Circular orbit as continuous free fall](circular-orbit-as-continuous-free-fall.md)
- [Curvature](curvature.md)
- [Curvature of a plane curve](curvature-of-a-plane-curve.md)
- [Curvature sign convention](curvature-sign-convention.md)
- [Differential geometry](differential-geometry-split.md)
- [Differential geometry of surfaces](differential-geometry-of-surfaces.md)
- [Einstein field equations](einstein-field-equations.md)
- [Flatness bound on the initial field in exponential inflation](flatness-bound-on-the-initial-field-in-exponential-inflation.md)
- [Fracture toughness](fracture-toughness.md)
- [Gaussian curvature](gaussian-curvature.md)
- [General relativity](general-relativity-split.md)
- [Geometry and topology](geometry-and-topology-split.md)
- [Lensmaker's equation](lensmaker-s-equation.md)
- [Level-line curvature](level-line-curvature.md)
- [Lichnerowicz spinor-square formula](lichnerowicz-spinor-square-formula.md)
- [Logarithmic conical helix](logarithmic-conical-helix.md)
- [Metric variation of a scalar-curvature coupling](metric-variation-of-a-scalar-curvature-coupling.md)
- [Minimal four-dimensional supergravity](minimal-four-dimensional-supergravity.md)
- [Nester two-form](nester-two-form.md)
- [Normal vector](normal-vector.md)
- [Off-axis pinhole test for coma](off-axis-pinhole-test-for-coma.md)
- [Osculating circle](osculating-circle.md)
- [Parametric curve interrogation](parametric-curve-interrogation.md)
- [Parametric surface interrogation](parametric-surface-interrogation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-44/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-68/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-68/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-68/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-47/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-47/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-59/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-71/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-71/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-71/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-71/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-71/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-71/7/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-57/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-68/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-77/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-3/4c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-55/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-55/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-55/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-55/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-58/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-2/24h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-2/35c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-66/5/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-66/5/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-66/6/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-81/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-1/2h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-66/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-66/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-75/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-2/24h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-2/24h/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-2/35e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-82/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-2/25h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-2/25h/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-2/36d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-64/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-64/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-68/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-329/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2/23i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-309/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-309/4/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-342/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-332/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-332/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-329/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-329/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-344/3/a/iii/solution.md)
- [Radius of curvature](radius-of-curvature.md)
- [Riemannian manifold](riemannian-manifold.md)
- [Riemannian metric](riemannian-metric.md)
- [Riemannian parallel-spinor Ricci-flatness](riemannian-parallel-spinor-ricci-flatness.md)
- [Scalar-tensor theory](scalar-tensor-theory.md)
- [Second moment of area](second-moment-of-area.md)
- [Segmentation interface curvature balance](segmentation-interface-curvature-balance.md)
- [Signed curvature](signed-curvature.md)
- [Spherical trigonometry](spherical-trigonometry.md)
- [Surface divergence](surface-divergence.md)
- [Tangential and normal acceleration](tangential-and-normal-acceleration.md)
- [Tensor index antisymmetrization](tensor-index-antisymmetrization.md)
- [Tensoriality](tensoriality.md)
- [Toughness-controlled magma intrusion](toughness-controlled-magma-intrusion.md)
- [Travel time at reciprocal-curvature speed](travel-time-at-reciprocal-curvature-speed.md)
- [Unit tangent vector](unit-tangent-vector.md)
- [Vapour-tip peeling of a magma intrusion](vapour-tip-peeling-of-a-magma-intrusion.md)
- [Young–Laplace equation](young-laplace-equation.md)
