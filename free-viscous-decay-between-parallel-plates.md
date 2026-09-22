# Free viscous decay between parallel plates

↑ **Parent:** [Plane Poiseuille flow](plane-poiseuille-flow.md)

For a unidirectional [incompressible flow](incompressible-flow.md) between stationary plates a distance $H>0$ apart, removing the driving [pressure gradient](pressure-gradient.md) leaves $u_t=\nu u_{yy}$ when the [kinematic viscosity](kinematic-viscosity.md) $\nu>0$ is constant. The [no-slip boundary condition](no-slip-boundary-condition.md) gives $u(0,t)=u(H,t)=0$. For an initial profile $g$ in [L2 space](l2-space-is-a-hilbert-space.md), [separation of variables](separation-of-variables.md) and the [Fourier sine series](fourier-sine-series.md) give the displayed solution, with

$$
b_n=\frac2H\int_0^H g(y)\sin\frac{n\pi y}{H}\,dy.
$$

Each [normal mode](normal-mode.md) decays at a rate proportional to $n^2$. The lowest mode present dominates at late times; when $b_1\ne0$, its [time constant](time-constant.md) is $H^2/(\nu\pi^2)$, consistent with the [viscous diffusion time](viscous-diffusion-time.md). The solution approaches the initial data in [L2 space](l2-space-is-a-hilbert-space.md); compatible smooth profiles also give the familiar pointwise initial condition. This is a [heat equation](heat-equation.md) for momentum diffusion, rather than temperature.

## ↑ Ancestors (6)

1. [Plane Poiseuille flow](plane-poiseuille-flow.md)
2. [Viscous fluid flow](viscous-fluid-flow-split.md)
3. [Fluid mechanics](fluid-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-2/section-b/10/solution.md)
