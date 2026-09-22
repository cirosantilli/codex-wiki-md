<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the [Boussinesq approximation](../../../../../../boussinesq-approximation.md), subtract the resting background [buoyancy](../../../../../../buoyancy.md) $N^2z$ and denote its perturbation by $b$. With constant nonzero $f$ and constant $N>0$, the leading [geostrophic flow](../../../../../../geostrophic-flow.md) and hydrostatic balance define the [quasi-geostrophic streamfunction](../../../../../../quasi-geostrophic-streamfunction.md)

$$
p'=f\psi,\qquad\mathbf u_g=(-\psi_y,\psi_x),\qquad b=f\psi_z.
$$

The leading horizontal flow is nondivergent. At the next order, its relative vertical [vorticity](../../../../../../vorticity.md) $q_g=\nabla_H^2\psi$ is stretched by the small vertical [velocity](../../../../../../velocity.md), while the background [buoyancy](../../../../../../buoyancy.md) is advected vertically. Thus the curl and [buoyancy](../../../../../../buoyancy.md) equations give

$$
D_g\nabla_H^2\psi=f w_z,\qquad D_gb+N^2w=0,
\qquad D_g=\partial_t-\psi_y\partial_x+\psi_x\partial_y.
$$

These follow from $Dq_a/Dt=-q_a\nabla_H\cdot\mathbf u$ with $q_a\simeq f$ and $\nabla_H\cdot\mathbf u_a=-w_z$, retaining the geostrophic advection of the first-order anomalies. Vertical advection of those anomalies is of higher quasi-geostrophic order.

Differentiate the [buoyancy](../../../../../../buoyancy.md) equation in $z$. It is important not to assume without justification that $\partial_z$ commutes with $D_g$. Their commutator on $b$ is

$$
[\partial_z,D_g]b=\mathbf u_{g,z}\cdot\nabla_Hb
=\frac1f(-b_y,b_x)\cdot(b_x,b_y)=0,
$$

by hydrostatic balance and [thermal wind](../../../../../../thermal-wind.md). Hence $D_gb_z=-N^2w_z$. Adding $f/N^2$ times this equation to the [vorticity](../../../../../../vorticity.md) equation eliminates $w_z$, yielding

$$
\boxed{D_gQ=0,\qquad Q=f+\nabla_H^2\psi+\frac{f^2}{N^2}\psi_{zz}.}
$$

This is the [quasi-geostrophic potential-vorticity equation](../../../../../../quasi-geostrophic-potential-vorticity-equation.md) on an $f$-plane. The additive $f$ makes $Q$ equal to the first-order normalized Ertel PV of total [buoyancy](../../../../../../buoyancy.md) $N^2z+b$; using a PV anomaly instead removes that constant and does not change the dynamics.

For [stretched coordinates for quasi-geostrophic inversion](../../../../../../stretched-coordinates-for-quasi-geostrophic-inversion.md), put

$$
X=x,\qquad Y=y,\qquad Z=\frac N{|f|}z.
$$

Then $(f^2/N^2)\partial_z^2=\partial_Z^2$, and the potential-vorticity relation becomes

$$
\boxed{Q=f+\nabla_*^2\psi,\qquad\nabla_*^2=\partial_X^2+\partial_Y^2+\partial_Z^2.}
$$

Stable [stratification](../../../../../../density-stratification.md) makes this operator elliptic. Uniform $N$ and nonzero $f$ are essential to this simple constant-coefficient stretching.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 77](../../../paper-77-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
