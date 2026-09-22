<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [simple Riemannian manifold](../../../../../../simple-riemannian-manifold.md) has strictly convex boundary, no [conjugate points](../../../../../../conjugate-points.md), and a unique connecting [geodesic](../../../../../../geodesic.md) depending smoothly on its endpoints. In particular its unit-speed geodesics are nontrapping. Write $\nu$ for the inward unit normal, and identify inward and outward parts of its boundary [unit tangent bundle](../../../../../../unit-tangent-bundle.md) by

$$
\partial_+SM=\{(x,v):x\in\partial M,\ |v|_g=1,\ \langle v,\nu\rangle\ge0\},
\qquad
\partial_-SM=\{(x,v):\langle v,\nu\rangle\le0\}.
$$

The signs are a convention; here $+$ means inward. If $(x,v)$ is strictly inward, let $\tau(x,v)>0$ be its first exit time. The [geodesic scattering relation](../../../../../../geodesic-scattering-relation.md) is

$$
\boxed{\alpha(x,v)=\phi_{\tau(x,v)}(x,v)
=\bigl(\gamma_{x,v}(\tau),\dot\gamma_{x,v}(\tau)\bigr)\in\partial_-SM.}
$$

Thus it records both the exit point and the outward unit velocity, not just the exit point. On strictly outward vectors extend $\alpha$ by following the same [geodesic flow](../../../../../../geodesic-flow.md) backwards to its previous entry point, retaining the velocity orientation. On tangential vectors set $\alpha(x,v)=(x,v)$. The extended [scattering relation](../../../../../../geodesic-scattering-relation.md) is an involution on the full boundary unit bundle, since its forward and backward constructions undo one another. On a [simple Riemannian manifold](../../../../../../simple-riemannian-manifold.md), the travel time equals the [boundary distance function](../../../../../../boundary-distance-function.md) between the two endpoints; travel time is often recorded separately as lens data.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
