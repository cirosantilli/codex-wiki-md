<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Begin with the [Boussinesq approximation](../../../../../../boussinesq-approximation.md) primitive equations on a [beta plane](../../../../../../beta-plane.md), decompose every field into a zonal mean and a disturbance, and average over longitude. The zonal momentum equation then contains the divergence of the eddy momentum flux $\overline{u'v'}$, while the mean density equation contains the divergence of the eddy density flux $\overline{\rho'v'}$. At small [Rossby number](../../../../../../rossby-number.md), use [geostrophic balance](../../../../../../geostrophic-balance.md), [hydrostatic pressure](../../../../../../hydrostatic-pressure.md), [thermal-wind balance](../../../../../../thermal-wind.md), and the leading eddy equations to combine those fluxes.

Define

$$
A=\frac{\overline{\rho'v'}}{d\rho_s/dz}
$$

and introduce the [residual mean circulation](../../../../../../residual-mean-circulation.md)

$$
\boxed{
\overline v_a^*=\overline v_a-A_z,
\qquad
\overline w_a^*=\overline w_a+A_y}.
$$

The added eddy-induced velocity is nondivergent, so

$$
\overline v_{a,y}^*+\overline w_{a,z}^*=0.
$$

It absorbs the eddy density-flux divergence into advection by the transformed circulation, giving

$$
\overline\rho_t+overline w_a^*\frac{d\rho_s}{dz}=0.
$$

The mean zonal momentum equation becomes

$$
\overline u_t-f_0\overline v_a^*
=\nabla\mathbin\cdot\overline{\mathbf F},
$$

where the zonally averaged [Eliassen–Palm flux](../../../../../../eliassen-palm-flux.md) in the meridional-vertical plane is

$$
\boxed{
\overline F^{(y)}=-\overline{u'v'},
\qquad
\overline F^{(z)}
=f_0\frac{\overline{\rho'v'}}{d\rho_s/dz}}.
$$

**Thus the [transformed Eulerian mean](../../../../../../transformed-eulerian-mean.md) gathers the wave forcing into one flux divergence and makes density evolve under one residual circulation.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 333](../../../paper-333-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
