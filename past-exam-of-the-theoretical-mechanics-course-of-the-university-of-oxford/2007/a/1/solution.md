<h1 id="a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $t(n)$ denote [traction](../../../../traction.md): the force per unit area exerted across an oriented internal surface with unit normal $n$. Define $\sigma_{ij}$ as component $i$ of the [traction](../../../../traction.md) on a coordinate plane whose normal is $e_j$. [Balance of linear momentum](../../../../balance-of-linear-momentum.md) on a shrinking tetrahedron makes the surface-force terms, of order area, dominate its inertia and [body forces](../../../../body-force.md), of order volume. Resolving its oblique face into the three coordinate projected areas gives Cauchy's [traction](../../../../traction.md) formula

$$
\boxed{t(n)=\sigma n,\qquad t_i(n)=\sigma_{ij}n_j.}
$$

Opposite faces have opposite [tractions](../../../../traction.md), as follows independently from a shrinking pillbox. This fixes both the index and normal conventions.

For a [material volume](../../../../material-volume.md) $V(t)$, the [Reynolds transport theorem](../../../../reynolds-transport-theorem.md) says $d\int_{V(t)}f\,dV/dt=\int_{V(t)}[f_t+\nabla\cdot(fu)]dV$. Apply it componentwise to $f=\rho u_i$ and use [mass conservation](../../../../mass-conservation.md). With no [body force](../../../../body-force.md) in this calculation, [balance of linear momentum](../../../../balance-of-linear-momentum.md) and the [divergence theorem](../../../../divergence-theorem.md) give

$$
\int_{V(t)}\rho\frac{Du_i}{Dt}\,dV
=\int_{\partial V(t)}\sigma_{ij}n_j\,dS
=\int_{V(t)}\partial_j\sigma_{ij}\,dV.
$$

Arbitrariness of the [material volume](../../../../material-volume.md) yields $\boxed{\rho Du_i/Dt=\partial_j\sigma_{ij}}$, with $D/Dt=\partial_t+u_j\partial_j$.

For constant [dynamic viscosity](../../../../dynamic-viscosity-split.md) and incompressible [velocity](../../../../velocity.md), $\partial_ju_j=0$, so

$$
\partial_j\sigma_{ij}=-\partial_ip+\mu\partial_j\partial_ju_i+
\mu\partial_i(\partial_ju_j)=-\partial_ip+\mu\nabla^2u_i.
$$

Thus $\boxed{\rho(u_t+u\cdot\nabla u)=-\nabla p+\mu\nabla^2u}$.

In fully developed steady [pipe flow](../../../../pipe-flow.md) $u=w(x,y)e_z$, the convective acceleration vanishes. The transverse equations give $p_x=p_y=0$ and the axial equation gives $p_z=\mu(w_{xx}+w_{yy})$. One side depends only on $z$ and the other only on $(x,y)$, so both equal a constant. Hence

$$
\boxed{w_{xx}+w_{yy}=p_z/\mu,\qquad p_z=\text{constant}.}
$$

If $n$ is outward from the fluid cross-section, the wall-on-fluid axial shear per length is $\mu\oint\partial_nw\,ds=\mu\int_A\Delta w\,dA=Ap_z$. The fluid-on-pipe force is its negative:

$$
\boxed{\text{drag per unit length}=-Ap_z.}
$$

For forward [pressure](../../../../pressure-split.md)-driven flow $p_z<0$, this force points along the flow. Its value depends on [cross-sectional area](../../../../cross-sectional-area.md) and [pressure](../../../../pressure-split.md) drop, even though the detailed [velocity](../../../../velocity.md) profile depends on the shape.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the theoretical mechanics course of the University of Oxford](../../../split.md)
5. [Theoretical mechanics course of the University of Oxford](../../../../theoretical-mechanics-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
