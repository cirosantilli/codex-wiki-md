<h1 id="a/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a [material volume](../../../../../material-volume.md) $V(t)$ moving with [velocity](../../../../../velocity.md) $\mathbf u$, the [Reynolds transport theorem](../../../../../reynolds-transport-theorem.md) is

$$
\frac d{dt}\int_{V(t)}f\,dV=\int_{V(t)}[\partial_tf+\nabla\cdot(f\mathbf u)]\,dV.
$$

It applies componentwise to vector quantities. [Cauchy's stress theorem](../../../../../cauchy-s-stress-theorem.md) represents [traction](../../../../../traction.md) on a surface with outward unit normal $\mathbf n$ as $t_i=\sigma_{ij}n_j$. [Conservation of mass](../../../../../mass-conservation.md) gives $d\int_{V(t)}\rho\,dV/dt=0$ and hence $\partial_t\rho+\nabla\cdot(\rho\mathbf u)=0$. Constant [density](../../../../../density.md) reduces this to $\boxed{\nabla\cdot\mathbf u=0}$.

With no [body force](../../../../../body-force.md), [conservation of momentum](../../../../../momentum-conservation.md) and the [divergence theorem](../../../../../divergence-theorem.md) give

$$
\frac d{dt}\int_{V(t)}\rho u_i\,dV=\int_{\partial V}\sigma_{ij}n_j\,dS=\int_V\partial_j\sigma_{ij}\,dV.
$$

Applying transport and then [mass conservation](../../../../../mass-conservation.md) cancels the terms proportional to $u_i$, leaving $\rho(\partial_tu_i+u_j\partial_ju_i)=\partial_j\sigma_{ij}$. For the stated Newtonian stress, constant [viscosity](../../../../../dynamic-viscosity-split.md) gives $\partial_j\sigma_{ij}=-\partial_ip+\mu\Delta u_i+\mu\partial_i(\nabla\cdot\mathbf u)$. The last term vanishes. Since the [material volume](../../../../../material-volume.md) was arbitrary,

$$
\boxed{\rho[\mathbf u_t+(\mathbf u\cdot\nabla)\mathbf u]=-\nabla p+\mu\Delta\mathbf u.}
$$

A [body force](../../../../../body-force.md), if present, would have to be added to the momentum balance; it is absent from the specified model.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the theoretical mechanics course of the University of Oxford](../../../../split.md)
6. [Theoretical mechanics course of the University of Oxford](../../../../../theoretical-mechanics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
