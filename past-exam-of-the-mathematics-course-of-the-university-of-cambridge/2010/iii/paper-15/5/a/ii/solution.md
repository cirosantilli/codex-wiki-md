<h1 id="5/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A [vector field along a map](../../../../../../../vector-field-along-a-map.md) $\gamma$ assigns $V(t)\in T_{\gamma(t)}M$ smoothly to each parameter value. Equivalently, it is a [section of a vector bundle](../../../../../../../section-of-a-vector-bundle.md) $\gamma^*TM$. The [pullback connection](../../../../../../../pullback-connection.md) defines its [covariant derivative along a curve](../../../../../../../covariant-derivative-along-a-curve.md), $D_tV$. To make the definition explicit, use [connection coefficients](../../../../../../../connection-components.md) with the convention

$$
\nabla_{\partial_i}\partial_j=\Gamma^k{}_{ij}\partial_k.
$$

For $V=V^k(t)\partial_k|_{\gamma(t)}$ the derivative is

$$
D_tV=\left(\frac{dV^k}{dt}
+\Gamma^k{}_{ij}(\gamma(t))\dot\gamma^i(t)V^j(t)\right)\partial_k.
$$

The [change of frame of a vector-bundle connection](../../../../../../../change-of-frame-of-a-vector-bundle-connection.md) ensures this expression is independent of the [coordinate chart](../../../../../../../manifold-chart.md). It remains meaningful when $\dot\gamma=0$ and does not require extending $V$ to one ambient [vector field](../../../../../../../vector-field.md).

**The field is parallel exactly when $\boxed{D_tV=0}$**. A [geodesic](../../../../../../../geodesic.md) for $\nabla$, with its specified affine parameter, is a [smooth curve](../../../../../../../smooth-curve.md) whose own tangent is parallel:

$$
\boxed{D_t\dot\gamma=0,
\qquad \ddot\gamma^k+\Gamma^k{}_{ij}(\gamma)\dot\gamma^i\dot\gamma^j=0.}
$$

This definition applies to any [affine connection](../../../../../../../affine-connection.md), whether or not it is a [metric connection](../../../../../../../metric-connection.md). A non-affine change of parameter generally gives a [pregeodesic](../../../../../../../pregeodesic.md) instead of this parametrized [geodesic](../../../../../../../geodesic.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Paper 15](../../../../paper-15-split.md)
5. [Iii](../../../../split.md)
6. [2010](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
