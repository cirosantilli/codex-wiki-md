<h1 id="1/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For an arbitrary [material volume](../../../../../material-volume.md) $V(t)$, [Newton's second law](../../../../../newton-s-second-law.md) equates the rate of change of [linear momentum](../../../../../momentum-split.md) to the resultant contact [force](../../../../../force-split.md), since there is no [body force](../../../../../body-force.md):

$$
\frac d{dt}\int_{V(t)}\rho u_i\,dV
=\int_{\partial V(t)}t_i(\mathbf n)\,dS
=\int_{\partial V(t)}\sigma_{ij}n_j\,dS.
$$

Use the [Reynolds transport theorem](../../../../../reynolds-transport-theorem.md) on the left. Expanding the product and using the [continuity equation](../../../../../continuity-equation.md) leaves

$$
\partial_t(\rho u_i)+\partial_j(\rho u_i u_j)
=\rho(\partial_tu_i+u_j\partial_ju_i)
+u_i[\partial_t\rho+\partial_j(\rho u_j)]
=\rho\frac{Du_i}{Dt}.
$$

On the right, the [divergence theorem](../../../../../divergence-theorem.md) applied to each row of the [Cauchy stress tensor](../../../../../cauchy-stress-tensor.md) gives

$$
\int_{\partial V(t)}\sigma_{ij}n_j\,dS
=\int_{V(t)}\partial_j\sigma_{ij}\,dV.
$$

Consequently the [volume integral](../../../../../volume-integral.md) of $\rho Du_i/Dt-\partial_j\sigma_{ij}$ vanishes on every [material volume](../../../../../material-volume.md). Localizing as in part (i) gives the [Cauchy momentum equation](../../../../../cauchy-momentum-equation.md):

$$
\boxed{\rho\left(\frac{\partial\mathbf u}{\partial t}
+(\mathbf u\cdot\nabla)\mathbf u\right)
=\mathbf e_i\frac{\partial\sigma_{ij}}{\partial x_j}.}
$$

The left side is [mass density](../../../../../density.md) times [material acceleration](../../../../../material-acceleration.md); the right side is the [divergence](../../../../../divergence.md) of the [Cauchy stress tensor](../../../../../cauchy-stress-tensor.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
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
