<h1 id="k/k1/solution">Solution</h1>

↑ **Parent:** [K1](../k1.md)

For a [material volume](../../../../material-volume.md) $V(t)$, Newton's second law equates the rate of change of momentum to [pressure](../../../../pressure-split.md) and body forces:

$$
\frac d{dt}\int_{V(t)}\rho\mathbf u\,dV
=-\int_{\partial V(t)}p\mathbf n\,dS+\int_{V(t)}\rho\mathbf g\,dV.
$$

Apply the supplied [Reynolds transport theorem](../../../../reynolds-transport-theorem.md) to each component of $\mathbf u$, and apply the [divergence theorem](../../../../divergence-theorem.md) to the [pressure](../../../../pressure-split.md) force. The result is

$$
\int_{V(t)}\left[\rho\left(\partial_t\mathbf u+(\mathbf u\cdot\nabla)\mathbf u\right)
+\nabla p-\rho\mathbf g\right]dV=0.
$$

Since the [material volume](../../../../material-volume.md) at the chosen time is arbitrary, the integrand vanishes pointwise for smooth fields. Dividing by positive [density](../../../../density.md) gives the [Euler equations](../../../../euler-equations-for-an-inviscid-fluid-split.md)

$$
\boxed{\partial_t\mathbf u+(\mathbf u\cdot\nabla)\mathbf u
=-\rho^{-1}\nabla p+\mathbf g.}
$$

At a fixed time $t$, a [streamline](../../../../streamline.md) is a curve tangent everywhere to the instantaneous velocity. Parametrize it by $d\mathbf x/ds=\mathbf u(\mathbf x(s),t)$. Then

$$
\frac d{ds}f(\mathbf x(s),t)=\nabla f\cdot\mathbf u=0,
$$

so $f$ is constant along it when the displayed directional derivative vanishes. Here time is held fixed: streamlines need not coincide with particle paths in an unsteady flow.

## ↑ Ancestors (12)

1. [K1](../k1.md)
2. [K](../../k.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
