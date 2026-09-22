<h1 id="a/1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use [conservation of mass](../../../../../mass-conservation.md) and Newton's [momentum balance](../../../../../momentum-balance-for-a-material-fluid-element.md), in addition to the supplied [constitutive law](../../../../../constitutive-equation.md). For a [material volume](../../../../../material-volume.md),

$$
\frac d{dt}\int_{V(t)}\rho\mathbf u\,dV=\int_{\partial V(t)}\boldsymbol\sigma\mathbf n\,dS+\int_{V(t)}\rho\mathbf g\,dV.
$$

The [Reynolds transport theorem](../../../../../reynolds-transport-theorem.md) and $\rho_t+\nabla\cdot(\rho\mathbf u)=0$ reduce the left side to $\int\rho D\mathbf u/Dt$. The [divergence theorem](../../../../../divergence-theorem.md) then gives $\rho D u_i/Dt=\partial_j\sigma_{ij}+\rho g_i$. For constant $\mu$,

$$
\partial_j\sigma_{ij}=-\partial_ip+\mu\partial_j\partial_ju_i+\mu\partial_i(\partial_ju_j).
$$

[Incompressibility](../../../../../incompressible-flow.md) removes the last term. Thus

$$
\boxed{\rho\frac{D\mathbf u}{Dt}=-\nabla p+\mu\nabla^2\mathbf u+\rho\mathbf g.}
$$

The stress formula and zero divergence alone are not a dynamical law: the [force](../../../../../force-split.md) balance supplies the required physical input.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the theoretical mechanics course of the University of Oxford](../../../../split.md)
6. [Theoretical mechanics course of the University of Oxford](../../../../../theoretical-mechanics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
