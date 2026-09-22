<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [magnetic second-moment tensor](../../../../magnetic-second-moment-tensor.md) is $M_{ij}=B_iB_j$. This is the magnetic dyadic called the Maxwell tensor in the paper; the isotropic part of the usual [Maxwell stress tensor](../../../../maxwell-stress-tensor.md) is already contained in the [magnetohydrodynamic total pressure](../../../../magnetohydrodynamic-total-pressure.md). The [solenoidal magnetic-field constraint](../../../../solenoidal-magnetic-field-constraint.md) gives

$$
\partial_jM_{ij}
=B_j\partial_jB_i+B_i\partial_jB_j
=B_j\partial_jB_i.
$$

Consequently the [magnetohydrodynamic momentum equation](../../../../magnetohydrodynamic-momentum-equation.md) in part [a](../a.md) becomes $D_tu_i=-\partial_i p+\partial_jM_{ij}$, where $D_t=\partial_t+u_n\partial_n$ is the [material derivative](../../../../material-derivative.md). Applying its product rule and the [ideal magnetohydrodynamic induction equation](../../../../ideal-magnetohydrodynamic-induction-equation.md) gives

$$
\begin{aligned}
D_tM_{ij}
&=(D_tB_i)B_j+B_i(D_tB_j)\\
&=B_nB_j\partial_nu_i+B_iB_n\partial_nu_j
=\boxed{M_{nj}\partial_nu_i+M_{in}\partial_nu_j}.
\end{aligned}
$$

Thus the evolution uses only $\mathbf u,M,p$, together with $\partial_i u_i=0$. To determine $p$, take the [divergence](../../../../divergence.md) of the [magnetohydrodynamic momentum equation](../../../../magnetohydrodynamic-momentum-equation.md). Since $\partial_t\partial_i u_i=0$ and $u_j\partial_j\partial_i u_i=0$,

$$
\boxed{\nabla^2p=\partial_i\partial_jM_{ij}
-(\partial_i u_j)(\partial_j u_i).}
$$

This is the [pressure Poisson equation for incompressible flow](../../../../pressure-poisson-equation-for-incompressible-flow.md), with [boundary conditions](../../../../boundary-condition.md) supplied by the imposed normal [acceleration](../../../../acceleration.md) and normal [stress](../../../../stress.md), or by periodicity or decay at infinity as appropriate. For example, the normal component of the [magnetohydrodynamic momentum equation](../../../../magnetohydrodynamic-momentum-equation.md) requires $\mathbf n\cdot\nabla p=\mathbf n\cdot(\nabla\cdot M-D_t\mathbf u)$ at a prescribed boundary. The [pressure](../../../../pressure-split.md) is determined up to a spatially constant function of [time](../../../../time-in-physics.md).

For equivalence to one resolved [magnetic field](../../../../magnetic-field-split.md), the initial $M$ must actually be $\mathbf B\mathbf B^T$ for a [divergence-free vector field](../../../../divergence-free-vector-field.md). In particular it is a symmetric [positive semidefinite matrix](../../../../positive-semidefinite-matrix.md) of [matrix rank](../../../../matrix-rank.md) at most one. The tensor equations also admit more general stresses; the averaged $M$ in part [d](../d.md) need not have [matrix rank](../../../../matrix-rank.md) one.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the advanced fluid dynamics course of the University of Oxford](../../../split.md)
5. [Advanced fluid dynamics course of the University of Oxford](../../../../advanced-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
