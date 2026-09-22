<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $V(t)$ be any material [volume](../../../../volume.md), moving with the [velocity field](../../../../velocity-field.md) $\mathbf u$. The [Reynolds transport theorem](../../../../reynolds-transport-theorem.md) in the required form is

$$
\frac d{dt}\int_{V(t)}f\,dV=\int_{V(t)}\left[\partial_t f+\nabla\cdot(f\mathbf u)\right]dV,
$$

applied componentwise when $f$ is vector-valued. [Mass conservation](../../../../mass-conservation.md) gives

$$
0=\frac d{dt}\int_{V(t)}\rho\,dV
=\int_{V(t)}\left[\rho_t+\nabla\cdot(\rho\mathbf u)\right]dV.
$$

Since the material [volume](../../../../volume.md) is arbitrary, the local [continuity equation](../../../../continuity-equation.md) follows:

$$
\boxed{\rho_t+\nabla\cdot(\rho\mathbf u)=0.}
$$

For an inviscid fluid with no [body force](../../../../body-force.md), the [balance of linear momentum](../../../../balance-of-linear-momentum.md) equates the rate of change of total [momentum](../../../../momentum-split.md) to the boundary [pressure](../../../../pressure-split.md) force:

$$
\frac d{dt}\int_{V(t)}\rho\mathbf u\,dV
=-\int_{\partial V(t)}p\mathbf n\,dS=-\int_{V(t)}\nabla p\,dV,
$$

using the [divergence theorem](../../../../divergence-theorem.md). The integrand on the left expands as

$$
\partial_t(\rho\mathbf u)+\nabla\cdot(\rho\mathbf u\otimes\mathbf u)
=\rho\frac{D\mathbf u}{Dt}+\mathbf u\left[\rho_t+\nabla\cdot(\rho\mathbf u)\right].
$$

The bracket vanishes by [mass conservation](../../../../mass-conservation.md), leaving the [Euler momentum equation](../../../../euler-equations-for-an-inviscid-fluid-split.md)

$$
\boxed{\rho\frac{D\mathbf u}{Dt}=-\nabla p,\qquad
\frac{D}{Dt}=\partial_t+\mathbf u\cdot\nabla.}
$$

Unlike the [incompressible flow](../../../../incompressible-flow.md) case, the [mass density](../../../../density.md) need not be constant along a [fluid element](../../../../fluid-element.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the fluids and waves course of the University of Oxford](../../../split.md)
5. [Fluids and waves course of the University of Oxford](../../../../fluids-and-waves-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
