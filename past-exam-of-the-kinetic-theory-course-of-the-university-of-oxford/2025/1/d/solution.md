<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $c_i=v_i-u_i$ and introduce the raw third [velocity moment](../../../../velocity-moment.md) $M_{ijk}$ and the [third central velocity moment](../../../../third-central-velocity-moment.md) $Q_{ijk}$:

$$
M_{ijk}=\int v_iv_jv_kf\,d^3v,\qquad \boxed{Q_{ijk}=\int c_ic_jc_kf\,d^3v.}
$$

The expansion of their product gives

$$
M_{ijk}=\rho u_iu_ju_k+u_iP_{jk}+u_jP_{ik}+u_kP_{ij}+Q_{ijk}.
$$

The [heat flux](../../../../heat-flux-density.md) is $q_i=Q_{ijj}/2$ for unit [mass](../../../../mass.md).

Multiply the [BGK model](../../../../bgk-model.md) by $v_iv_j$. The external [force](../../../../force-split.md) term is

$$
-\partial_kU\int v_iv_j\partial_{v_k}f\,d^3v=\rho(u_j\partial_iU+u_i\partial_jU).
$$

Therefore the raw second [velocity moment](../../../../velocity-moment.md) satisfies

$$
\partial_t\Pi_{ij}+\partial_kM_{ijk}=-\rho(u_i\partial_jU+u_j\partial_iU)-\frac{\Pi_{ij}-\Pi_{ij}^{(0)}}{\tau}.
$$

The matching [local Maxwellian](../../../../local-maxwellian.md) has $\Pi_{ij}^{(0)}=\rho u_iu_j+\rho\Theta\delta_{ij}$, so

$$
\Pi_{ij}-\Pi_{ij}^{(0)}=P_{ij}-P_{ij}^{(0)},\qquad P_{ij}^{(0)}=\rho\Theta\delta_{ij}.
$$

To remove the bulk motion, let $D_t=\partial_t+u_k\partial_k$ be the [material derivative](../../../../material-derivative.md). The [continuity equation](../../../../continuity-equation.md) and the [momentum conservation](../../../../momentum-conservation.md) equation imply

$$
\rho D_tu_i=-\partial_kP_{ik}-\rho\partial_iU,
$$

and hence

$$
\partial_t(\rho u_iu_j)+\partial_k(\rho u_iu_ju_k)=-u_j\partial_kP_{ik}-u_i\partial_kP_{jk}-\rho(u_i\partial_jU+u_j\partial_iU).
$$

Subtract this identity from the raw second [velocity moment](../../../../velocity-moment.md) equation and insert the expansion of $M_{ijk}$. The terms $u_i\partial_kP_{jk}$ and $u_j\partial_kP_{ik}$ cancel by the [product rule](../../../../product-rule.md). The external [force](../../../../force-split.md) terms also cancel, since a common acceleration changes the local [mean velocity](../../../../mean-velocity-of-a-kinetic-distribution.md) without directly changing the relative [velocities](../../../../velocity.md). What remains is

$$
\boxed{\partial_tP_{ij}+\partial_k(u_kP_{ij}+Q_{ijk})+P_{ik}\partial_ku_j+P_{jk}\partial_ku_i=-\frac{P_{ij}-\rho\Theta\delta_{ij}}{\tau}.}
$$

The trace of the relaxation term is zero because $P_{ii}=3\rho\Theta$. Thus the [BGK model](../../../../bgk-model.md) relaxes anisotropy of the [pressure tensor](../../../../pressure-tensor.md) while preserving the local random [kinetic energy](../../../../kinetic-energy.md). The evolution is still a [velocity-moment hierarchy](../../../../velocity-moment-hierarchy.md), since $Q_{ijk}$ requires further information about $f$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the kinetic theory course of the University of Oxford](../../../split.md)
5. [Kinetic theory course of the University of Oxford](../../../../kinetic-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
