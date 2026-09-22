<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use a one-layer, hydrostatic, homogeneous fluid with reference depth $H_0$, no forcing or friction, small [Rossby number](../../../../../../rossby-number.md) $\epsilon=U/(|f_0|L)\ll1$, slow evolution, and leading [geostrophic balance](../../../../../../geostrophic-balance.md). For the [beta plane](../../../../../../beta-plane.md), take $\beta L/|f_0|=O(\epsilon)$; the relative free-surface displacement is also small, $\eta/H_0=O(\epsilon)$, with the [Rossby deformation radius](../../../../../../rossby-deformation-radius.md) retained at the chosen horizontal scale. This excludes the equatorial limit. If a bottom elevation $h_b$ is included, additionally require $h_b/H_0=O(\epsilon)$ and stationary topography. Set $h_b=0$ for a flat bottom.

The [quasi-geostrophic streamfunction](../../../../../../quasi-geostrophic-streamfunction.md) satisfies $\psi=g\eta/f_0$, $u=-\psi_y$, $v=\psi_x$, so [relative vorticity](../../../../../../relative-vorticity.md) is $\zeta=\nabla_h^2\psi$. Expanding the [shallow-water potential vorticity](../../../../../../shallow-water-potential-vorticity.md) using actual depth $H_0+\eta-h_b$ gives

$$
q=\frac{f_0}{H_0}+\frac1{H_0}\left[\nabla_h^2\psi+\beta y-\frac{f_0\eta}{H_0}+\frac{f_0h_b}{H_0}\right]+O(\epsilon^2|f_0|/H_0).
$$

Consequently the depth-scaled anomaly, the [shallow-water quasi-geostrophic potential vorticity](../../../../../../shallow-water-quasi-geostrophic-potential-vorticity.md), is

$$
\boxed{Q=\nabla_h^2\psi-R_D^{-2}\psi+\beta y+\frac{f_0h_b}{H_0},\qquad R_D^2=\frac{gH_0}{f_0^2}.}
$$

The leading material derivative uses the [geostrophic flow](../../../../../../geostrophic-flow.md). Define $J(a,b)=a_xb_y-a_yb_x$; then conservation yields $Q_t+J(\psi,Q)=0$. The term $-\psi/R_D^2$ represents free-surface stretching, $\beta y$ the variation of planetary rotation, and $f_0h_b/H_0$ topographic stretching. Under a [rigid lid](../../../../../../rigid-lid-approximation.md) or at scales much smaller than the [Rossby deformation radius](../../../../../../rossby-deformation-radius.md), the free-surface term is absent or negligible and the flat-bottom [Barotropic Rossby wave](../../../../../../barotropic-rossby-wave.md) model has $Q=\nabla_h^2\psi+\beta y$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 333](../../../paper-333-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
