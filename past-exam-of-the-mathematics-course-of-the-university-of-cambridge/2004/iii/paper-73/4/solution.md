<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $R=\overline{u'v'}$ be the eddy [momentum flux](../../../../../momentum-flux.md), $F=\overline{\rho'v'}$ the eddy [density](../../../../../density.md) flux, and $S=d\rho_s/dz<0$. The PDF's hydrostatic equation is $g\overline\rho=-\overline p_z$; the converted TeX mistakenly replaces the [pressure](../../../../../pressure.md) derivative by a [density](../../../../../density.md) derivative. With $N_0^2=-gS/\rho_0$, define

$$
A=F/S,\qquad v^*=\overline v_a-A_z,\qquad w^*=\overline w_a+A_y.
$$

The [residual mean circulation](../../../../../residual-mean-circulation.md) is nondivergent because $v_y^*+w_z^*=\overline v_{ay}+\overline w_{az}$. Substituting in the original mean momentum and [density](../../../../../density.md) equations gives the [transformed Eulerian mean](../../../../../transformed-eulerian-mean.md) equations

$$
\boxed{\overline u_t-f_0v^*=-R_y+f_0A_z=\partial_y\mathsf F_y+\partial_z\mathsf F_z,}
\qquad
\boxed{\overline\rho_t+Sw^*=0,\quad v_y^*+w_z^*=0,}
$$

with the unchanged geostrophic and hydrostatic balances. Here the [Eliassen–Palm flux](../../../../../eliassen-palm-flux.md) components are

$$
\mathsf F_y=-R,\qquad \mathsf F_z=f_0A
=\frac{f_0\overline{v'b'}}{N_0^2},\qquad b'=-g\rho'/\rho_0.
$$

The [eddy buoyancy flux](../../../../../eddy-buoyancy-flux.md) has been absorbed into the residual transport, while both types of wave forcing enter the momentum equation through the [Eliassen–Palm flux](../../../../../eliassen-palm-flux.md) divergence.

For geostrophic disturbances, the [Taylor identity for quasi-geostrophic flux](../../../../../taylor-identity-for-quasi-geostrophic-flux.md) gives

$$
\nabla\cdot\boldsymbol{\mathsf F}=\overline{v'q'}.
$$

For example, zonal averaging removes $\overline{\psi'_x\psi'_{xx}}$ and converts the remaining horizontal and vertical terms in $\overline{\psi'_xq'}$ into derivatives of $\overline{\psi'_x\psi'_y}$ and $(f_0^2/N_0^2)\overline{\psi'_x\psi'_z}$, giving precisely the displayed fluxes.

Locally, for a basic flow with nonzero meridional PV gradient $Q_y$, the [quasi-geostrophic wave pseudomomentum](../../../../../quasi-geostrophic-wave-pseudomomentum.md) is $\mathcal A=\overline{q'^2}/(2Q_y)$. Multiplying the linear perturbation PV equation by $q'/Q_y$ gives

$$
\mathcal A_t+\nabla\cdot\boldsymbol{\mathsf F}=\frac{\overline{q'\mathcal D}}{Q_y},
$$

where $\mathcal D$ is a PV source or sink. In a locally uniform conservative [Rossby wave](../../../../../rossby-wave.md) packet, $\boldsymbol{\mathsf F}=\mathcal A\mathbf c_g$. Thus the flux tracks [group velocity](../../../../../group-velocity.md) rather than the generally different [phase velocity](../../../../../phase-velocity.md), with a signed [wave activity](../../../../../wave-activity.md) if $Q_y<0$.

The [non-acceleration theorem for quasi-geostrophic waves](../../../../../non-acceleration-theorem-for-quasi-geostrophic-waves.md) states that statistically steady conservative waves, with no wave-activity sources, sinks or independent boundary forcing, produce no balanced mean acceleration. Their flux divergence vanishes. In the present stable, impermeable mean-flow problem the homogeneous residual-circulation equation then has the zero solution, so $v^*=w^*=0$ and $\overline u_t=0$. The [Eulerian mean flow](../../../../../eulerian-mean-flow.md) can still circulate because its eddy-induced correction need not vanish. Dissipation, absorption at a critical layer, time-dependent [wave activity](../../../../../wave-activity.md) or boundary forcing produces a nonzero flux divergence and invalidates the non-acceleration conclusion.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 73](../../paper-73-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
