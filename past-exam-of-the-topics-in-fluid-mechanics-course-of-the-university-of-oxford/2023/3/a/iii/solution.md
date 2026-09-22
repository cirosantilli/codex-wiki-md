<h1 id="3/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [product rule](../../../../../product-rule.md) and fluctuation [incompressibility](../../../../../incompressible-flow.md) give the pointwise identity

$$
(u_i'u_j')_{,j}=u_j'u_{i,j}'+u_i'u_{j,j}'=u_j'u_{i,j}'.
$$

Averaging therefore gives

$$
\boxed{\overline{u_j'u_{i,j}'}=\overline{(u_i'u_j')_{,j}}
=\partial_j\overline{u_i'u_j'}.}
$$

The fluctuation term is consequently the [divergence](../../../../../divergence.md) of a [Reynolds stress](../../../../../reynolds-stress.md). The [eddy viscosity](../../../../../eddy-viscosity.md) model represents this momentum transport through a coefficient multiplying the mean [strain-rate tensor](../../../../../strain-rate-tensor.md):

$$
-\rho\overline{u_i'u_j'}\simeq\mu_T(U_{i,j}+U_{j,i})
$$

for its shear or deviatoric part. For example, $-\rho\overline{u'v'}\simeq\mu_TU_y$ in a thin parallel [shear flow](../../../../../shear-flow.md). The [dynamic viscosity](../../../../../dynamic-viscosity-split.md) $\mu_T$ is an effective flow-dependent transport coefficient, rather than a molecular material property. Large eddies carry [linear momentum](../../../../../momentum-split.md) between regions of different mean [velocity](../../../../../velocity.md).

There is a necessary qualification to the printed tensor equation (4). Taking its [trace](../../../../../matrix-trace.md) literally gives $0=-\rho\overline{u_i'u_i'}$, which would exclude nonzero [turbulence](../../../../../turbulence-split.md). A consistent [deviatoric eddy-viscosity closure](../../../../../deviatoric-eddy-viscosity-closure.md) in $d$ fluctuating dimensions is

$$
-\rho\overline{u_i'u_j'}=\mu_T(U_{i,j}+U_{j,i})
-\frac{2\rho e_t}{d}\delta_{ij},\qquad
 e_t=\frac12\overline{u_k'u_k'}.
$$

The isotropic term is absorbed into the effective [pressure](../../../../../pressure-split.md) $P_{\mathrm{eff}}=P+2\rho e_t/d$. Here $d=2$ for a strictly two-dimensional fluctuation model. The subsequent equations use $P$ for this effective [pressure](../../../../../pressure-split.md), or equivalently use (4) as a shear-stress closure. This preserves the intended thin-layer model without asserting an impossible full covariance identity.

For turbulent motions of scale $l$ and [velocity](../../../../../velocity.md) scale $u_l$, the estimate $\mu_T\sim\rho u_ll$ gives $\mu_T/\mu\sim u_ll/\nu$. It is much greater than one on energetic large scales and in the [inertial range](../../../../../inertial-range.md) well above the [Kolmogorov length scale](../../../../../kolmogorov-length-scale.md). At the molecular dissipation scales it is no longer large, and molecular transport also dominates very near a smooth solid wall.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the topics in fluid mechanics course of the University of Oxford](../../../../split.md)
6. [Topics in fluid mechanics course of the University of Oxford](../../../../../topics-in-fluid-mechanics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
