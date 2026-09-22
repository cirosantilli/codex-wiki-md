<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $V(t)$ have a boundary moving with [velocity](../../../../../velocity.md) $\mathbf v_b$, and let $\mathbf n$ be its outward unit [normal vector](../../../../../normal-vector.md). For a smooth scalar field $q$, the [Reynolds transport theorem](../../../../../reynolds-transport-theorem.md) is

$$
\frac{d}{dt}\int_{V(t)}q\,dV
=\int_{V(t)}\partial_tq\,dV
+\int_{\partial V(t)}q\mathbf v_b\cdot\mathbf n\,dS
=\int_{V(t)}[\partial_tq+\nabla\cdot(q\mathbf v_b)]\,dV.
$$

In the last expression, extend $\mathbf v_b$ smoothly into $V(t)$ and use the [divergence theorem](../../../../../divergence-theorem.md). For a [material volume](../../../../../material-volume.md), its boundary moves with the fluid [velocity](../../../../../velocity.md) $\mathbf u$, so $\mathbf v_b=\mathbf u$. Equivalently, the [Reynolds transport theorem](../../../../../reynolds-transport-theorem.md) for a [material volume](../../../../../material-volume.md) reads

$$
\frac{d}{dt}\int_{V(t)}q\,dV
=\int_{V(t)}\left(\frac{Dq}{Dt}+q\nabla\cdot\mathbf u\right)dV,
\qquad \frac D{Dt}=\partial_t+\mathbf u\cdot\nabla,
$$

where $D/Dt$ is the [material derivative](../../../../../material-derivative.md).

For an arbitrary moving region, [mass conservation](../../../../../mass-conservation.md) includes the relative [mass flow rate](../../../../../mass-flow-rate.md) across its boundary:

$$
\frac{d}{dt}\int_{V(t)}\rho\,dV
=-\int_{\partial V(t)}\rho(\mathbf u-\mathbf v_b)\cdot\mathbf n\,dS.
$$

Substitution of the [Reynolds transport theorem](../../../../../reynolds-transport-theorem.md) and the [divergence theorem](../../../../../divergence-theorem.md) gives

$$
\int_{V(t)}[\partial_t\rho+\nabla\cdot(\rho\mathbf u)]\,dV=0.
$$

Since the region is arbitrary, a continuous integrand must vanish: if it had a positive or negative value at a point, a sufficiently small surrounding region would have an [integral](../../../../../integral-split.md) of the same sign. This gives the [continuity equation](../../../../../continuity-equation.md). With constant positive [mass density](../../../../../density.md) $\rho$, it reduces to

$$
\boxed{\nabla\cdot\mathbf u=0.}
$$

Thus **the flow is incompressible**. For a [material volume](../../../../../material-volume.md), the same argument starts directly from conservation of its total [mass](../../../../../mass.md), with zero relative boundary flux.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the viscous flow course of the University of Oxford](../../../../split.md)
6. [Viscous flow course of the University of Oxford](../../../../../viscous-flow-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
