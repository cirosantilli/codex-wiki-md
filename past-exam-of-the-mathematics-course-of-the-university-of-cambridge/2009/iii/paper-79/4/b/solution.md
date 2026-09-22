<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $q=\partial_z\bar\rho>0$ for the unstable, horizontally averaged [density gradient](../../../../../../density-gradient.md). A turbulent displacement over a [mixing length](../../../../../../mixing-length.md) of order $W$ encounters a density contrast $\Delta\rho\sim Wq$. Balancing its [buoyancy](../../../../../../buoyancy.md) acceleration with the inertial acceleration gives

$$
\frac{u_*^2}{W}\sim g\frac{Wq}{\bar\rho},\qquad \boxed{u_*\sim W\sqrt{\frac{gq}{\bar\rho}}.}
$$

A [turbulent diffusivity](../../../../../../eddy-diffusivity.md) for density is therefore $D_T=K u_*W=KW^2\sqrt{gq/\bar\rho}$, absorbing dimensionless factors into $K>0$. The upward density flux is $J_\rho=\langle w'\rho'\rangle=-D_Tq$: turbulent exchange carries denser water downwards and lighter water upwards. Defining $F_\rho=-J_\rho$ as the positive downward flux yields the [buoyancy-driven turbulent density diffusion](../../../../../../buoyancy-driven-turbulent-density-diffusion.md) law

$$
\boxed{F_\rho=KW^2\sqrt{\frac g{\bar\rho}}\left(\partial_z\bar\rho\right)^{3/2}.}
$$

This is a flux per unit horizontal area, with units of mass per area per time. The total density transport across a horizontal section is $W^2F_\rho$.

The assumptions are established high-[Reynolds number](../../../../../../reynolds-number.md) [turbulence](../../../../../../turbulence-split.md), width-limited eddies, an instantaneous local balance between [buoyancy](../../../../../../buoyancy.md) and inertia, approximately constant $K$, negligible molecular diffusion, and zero mean vertical volume flux. The last condition follows from [incompressibility](../../../../../../incompressible-flow.md) and impermeable sidewalls in a closed tube. Density variations and the eddy statistics must also vary slowly enough for a local [mixing-length closure](../../../../../../mixing-length-closure.md) to be meaningful.

Horizontal averaging of [mass conservation](../../../../../../mass-conservation.md), with upward $z$, gives $\bar\rho_t=-\partial_zJ_\rho=\partial_zF_\rho$. Differentiating once more supplies the requested evolution of the [density gradient](../../../../../../density-gradient.md):

$$
\boxed{\partial_tq=\partial_z^2\left[KW^2\sqrt{\frac g{\bar\rho}}\,q^{3/2}\right].}
$$

Under the [Boussinesq approximation](../../../../../../boussinesq-approximation.md), replace $\bar\rho$ in the inertial prefactor by the constant reference density $\rho_0$; retain the changing [density gradient](../../../../../../density-gradient.md) inside the flux.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
