<h1 id="section-i/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

For a [Killing vector field](../../../../../../killing-vector-field.md) $\xi$, set $K^{\mu\nu}=\nabla^\mu\xi^\nu=-K^{\nu\mu}$. Choose surface orientation conventions so that the [Komar charge](../../../../../../komar-charge.md), up to overall normalization, is

$$
Q_\xi(V)=\tfrac12\int_{\partial V}K^{\mu\nu}\,dS_{\mu\nu}=\int_VJ_\xi^\mu\,dS_\mu,\qquad J_\xi^\mu=\nabla_\nu K^{\mu\nu}.
$$

This is the [Komar current from trace-reversed stress-energy](../../../../../../komar-current-from-trace-reversed-stress-energy.md) construction. The equality is the spacetime [Stokes theorem](../../../../../../stokes-theorem.md). With $[\nabla_\mu,\nabla_\nu]V^\rho=R^\rho{}_{\sigma\mu\nu}V^\sigma$, the [Killing equation](../../../../../../killing-equation.md) and $\nabla_\nu\xi^\nu=0$ give $J_\xi^\mu=R^\mu{}_\nu\xi^\nu$. In four dimensions, at zero cosmological constant, the [Einstein field equations](../../../../../../einstein-field-equations.md) give **the current**

$$
\boxed{J_\xi^\mu=8\pi G\left(T^\mu{}_\nu-\tfrac12T\delta^\mu{}_\nu\right)\xi^\nu.}
$$

Reversing orientation changes the common overall sign, not conservation. The [contracted Bianchi identity](../../../../../../contracted-bianchi-identity.md) gives

$$
\nabla_\mu J_\xi^\mu=\tfrac12\xi^\nu\partial_\nu R+R^{\mu\nu}\nabla_\mu\xi_\nu=0.
$$

An isometry preserves [scalar curvature](../../../../../../scalar-curvature.md), and the second term contracts symmetric and antisymmetric tensors. Equivalently [stress-energy conservation](../../../../../../stress-energy-conservation.md), the [Killing equation](../../../../../../killing-equation.md), and $\mathcal L_\xi T=0$ cancel the matter expression; its trace derivative needs this last observation. **Hence $\boxed{\nabla_\mu J_\xi^\mu=0}$.** Nonzero cosmological constant adds $\Lambda\xi^\mu$ to the geometric current, also divergence-free.

## ↑ Ancestors (11)

1. [Vi](../vi.md)
2. [Section I](../../section-i.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
