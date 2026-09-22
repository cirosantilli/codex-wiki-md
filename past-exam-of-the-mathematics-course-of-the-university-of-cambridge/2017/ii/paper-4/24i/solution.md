<h1 id="24i/solution">Solution</h1>

↑ **Parent:** [24I](../24i.md)

For $v\in T_pS$ sufficiently small, let $\gamma_v$ be the [geodesic](../../../../../geodesic.md) with $\gamma_v(0)=p$, $\dot\gamma_v(0)=v$, and define $\exp_p(v)=\gamma_v(1)$. The domain consists more generally of initial velocities whose [geodesic](../../../../../geodesic.md) exists through time one. Uniqueness and affine rescaling give $\exp_p(tv)=\gamma_v(t)$ near zero, so

$$
\boxed{d\exp_p|_0(v)=v.}
$$

Thus the differential is the identity under the natural identification of tangent spaces, and the [inverse function theorem](../../../../../inverse-function-theorem.md) makes the [exponential map](../../../../../exponential-map-riemannian-geometry.md) a [local diffeomorphism](../../../../../local-diffeomorphism.md) near zero.

A punctured plane has [geodesics](../../../../../geodesic.md) reaching its missing point in finite time, so its [exponential map](../../../../../exponential-map-riemannian-geometry.md) need not be global; adding the point remedies this example. But **an extension cannot always remedy the failure**. On the [punctured circular cone](../../../../../punctured-circular-cone.md) $S=\{(r\cos\theta,r\sin\theta,r):r>0\}$, radial generators are [geodesics](../../../../../geodesic.md) and reach the missing point in finite intrinsic length. Any globally defined extension would have to include their limiting point $(0,0,0)$. The cone's tangent planes have different limits as $\theta$ varies; no smooth embedded surface through that point can contain this [punctured circular cone](../../../../../punctured-circular-cone.md). Hence no such extension exists for this $S$.

For an [oriented surface](../../../../../oriented-surface.md) and a closed topological disc $D$ with smooth positively oriented boundary, the [Gauss-Bonnet theorem](../../../../../gauss-bonnet-theorem.md) with boundary says

$$
\boxed{\int_D K\,dA+\int_{\partial D}k_g\,ds=2\pi\chi(D)=2\pi.}
$$

Here $k_g$ is signed [geodesic curvature](../../../../../geodesic-curvature.md) with the disc on the left. A smooth boundary has no corner terms; piecewise smooth boundaries require exterior-angle terms.

For the flat disc in the problem this gives $\int_{\partial D}k_g\,ds=2\pi$. Conditions (i) and (ii) mean that the proposed replacement disc has the same boundary and agrees with the original [smooth surface](../../../../../smooth-surface.md) from the outside. Smoothness therefore gives the same tangent planes, metric [derivatives](../../../../../derivative.md) and boundary [geodesic curvature](../../../../../geodesic-curvature.md) on the replacement, with consistent [orientation](../../../../../orientation-of-a-simplex.md). Applying Gauss-Bonnet to that disc forces

$$
\boxed{\int_{\widetilde D}\widetilde K\,d\widetilde A=0.}
$$

Thus these gluing conditions fix the [total curvature](../../../../../total-curvature.md) of any smooth replacement disc, regardless of its detailed interior shape.

The nonnegative continuous [Gaussian curvature](../../../../../gaussian-curvature.md) on the compact replacement disc, together with its zero integral established by Gauss-Bonnet, forces it to vanish at every point of that disc. Outside it the replacement surface agrees with the original flat surface, so its curvature also vanishes there; smoothness covers the common boundary. Consequently no point of the replacement surface can have positive [Gaussian curvature](../../../../../gaussian-curvature.md). Therefore **no surface can satisfy all three conditions**. A disc with some positive curvature could only have compensating negative curvature or alter the smooth boundary gluing, both excluded here.

## ↑ Ancestors (10)

1. [24I](../24i.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
