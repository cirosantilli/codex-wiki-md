<h1 id="a/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [traction](../../../../../traction.md) $\mathbf t(\mathbf n)$ is force per unit area across an oriented surface with unit normal $\mathbf n$. The stress component $\sigma_{ij}$ is its $i$th component on a surface normal to the $j$th coordinate axis. [Cauchy's stress theorem](../../../../../cauchy-s-stress-theorem.md) states that this dependence is linear:

$$
\boxed{t_i(\mathbf n)=\sigma_{ij}n_j.}
$$

For the boundary of a [material volume](../../../../../material-volume.md), take the outward normal and the [traction](../../../../../traction.md) exerted by the surrounding fluid. Newton's law and the [divergence theorem](../../../../../divergence-theorem.md) give

$$
\frac d{dt}\int_{V(t)}\rho u_i\,dV
=\int_{\partial V(t)}\sigma_{ij}n_j\,dS
=\int_{V(t)}\partial_j\sigma_{ij}\,dV.
$$

Constant [density](../../../../../density.md) and [incompressibility](../../../../../incompressible-flow.md) make the transport-theorem integrand on the left $\rho Du_i/Dt$. The volume is arbitrary, so

$$
\boxed{\rho\frac{Du_i}{Dt}=\partial_j\sigma_{ij}.}
$$

Substitute the Newtonian constitutive law. With constant viscosity,

$$
\partial_j\sigma_{ij}=-\partial_i p+\mu\partial_j\partial_j u_i
+\mu\partial_i(\partial_j u_j)=-\partial_i p+\mu\nabla^2u_i.
$$

Hence

$$
\boxed{\rho(\mathbf u_t+(\mathbf u\cdot\nabla)\mathbf u)
=-\nabla p+\mu\nabla^2\mathbf u.}
$$

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the theoretical mechanics course of the University of Oxford](../../../../split.md)
6. [Theoretical mechanics course of the University of Oxford](../../../../../theoretical-mechanics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
