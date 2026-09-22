# Quadratic drag

↑ **Parent:** [Drag (physics)](drag-physics.md)

Quadratic drag has magnitude proportional to the square of the relative speed and points opposite to the relative velocity.

For an [isotropic](isotropy.md) model of a body of fixed shape, let $\mathbf U=\mathbf v_{\rm body}-\mathbf u_\infty$ denote its [relative velocity](relative-velocity.md) through the distant [fluid](fluid.md), with $U=|\mathbf U|$. A constant positive resistance $k$ gives

$$
\mathbf F_D=-k|\mathbf U|\mathbf U,\qquad F_D=kU^2,\qquad k=\tfrac12\rho AC_D.
$$

Here [density](density.md) $\rho$, reference [area](surface-area.md) $A$ and [drag coefficient](drag-coefficient.md) $C_D$ are held fixed over the modeled range of relative [speeds](speed.md). The vector formula makes the direction explicit: the [drag force](drag-physics.md) on the body opposes its motion relative to the [fluid](fluid.md), and vanishes at $U=0$. For a general body, orientation and other flow conditions can affect the [drag coefficient](drag-coefficient.md); treating it as a constant requires a regime in which that is an adequate approximation. [NASA Glenn Research Center, Drag Coefficient, Air Viscosity and Compressibility Effects](https://www1.grc.nasa.gov/beginners-guide-to-aeronautics/drag-coefficient/)

Compare two distinct models at a chosen relative [speed](speed.md) $U_0>0$. A [linear drag](linear-drag.md) model has $F_D(U)/F_D(U_0)=U/U_0$, while a constant-coefficient [quadratic drag](quadratic-drag.md) model has $F_D(U)/F_D(U_0)=(U/U_0)^2$. At $U=2U_0$ their [drag force](drag-physics.md) ratios are two and four respectively.

<a id="image-normalized-linear-and-quadratic-drag-models-doubling-speed-gives-force-ratios-two-and-four"></a>
![](linear-versus-quadratic-drag-scaling.png)

**[Figure 12](#image-normalized-linear-and-quadratic-drag-models-doubling-speed-gives-force-ratios-two-and-four). Normalized linear and quadratic drag models: doubling speed gives force ratios two and four**. Each model is divided by its own [drag force](drag-physics.md) at $U_0$. The [linear drag](linear-drag.md) curve applies, for example, to a rigid [sphere](sphere.md) under the [Stokes drag law](stokes-s-law.md) assumptions while its [particle Reynolds number](particle-reynolds-number.md) remains small. The [quadratic drag](quadratic-drag.md) curve assumes constant [density](density.md), reference [area](surface-area.md) and [drag coefficient](drag-coefficient.md) over its modeled range. The comparison specifies neither an exact transition nor a single set of physical parameters that realizes both laws throughout the plotted range.

This distinction matters when estimating [terminal velocity](terminal-velocity.md) or trajectories such as [descent from rest under quadratic drag](descent-from-rest-under-quadratic-drag.md): doubling relative [speed](speed.md) increases the resistance much more strongly in the [quadratic drag](quadratic-drag.md) model. An approximately constant [drag coefficient](drag-coefficient.md) can occur in another [Reynolds number](reynolds-number.md) regime; its use must be justified there. Conversely, substituting the creeping-flow [sphere](sphere.md) coefficient $C_D=24/\mathrm{Re}_d$ into $F_D=\tfrac12\rho U^2AC_D$ recovers [linear drag](linear-drag.md), so writing this general formula does not make the resistance quadratic. Neither approximation should be extended across all [Reynolds numbers](reynolds-number.md).

The distinction already appears in the original investigation underlying the [Stokes drag law](stokes-s-law.md), read on 9 December 1850: article 42 identifies resistance proportional to relative [speed](speed.md) and distinguishes it from a contribution proportional to the square of relative [speed](speed.md). [George Gabriel Stokes, On the Effect of the Internal Friction of Fluids on the Motion of Pendulums, article 42, collected-paper reprint](https://mural.uv.es/daroig/documentos/stokes1850.pdf)

**Table of contents**

- [Descent from rest under quadratic drag](descent-from-rest-under-quadratic-drag.md)
- [Quadratic-drag turning angle](quadratic-drag-turning-angle.md)
  - [Mass per drag area](mass-per-drag-area.md)
- [Quadratic damping](quadratic-damping.md)

## ↑ Ancestors (5)

1. [Drag (physics)](drag-physics.md)
2. [Fluid mechanics](fluid-mechanics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (21)

- [Accreting raindrop with quadratic drag](accreting-raindrop-with-quadratic-drag.md)
- [Constant mass-loss propulsion with quadratic drag](constant-mass-loss-propulsion-with-quadratic-drag.md)
- [Damped pendulum](damped-pendulum.md)
- [Damping measurement from free decay](damping-measurement-from-free-decay.md)
- [Descent from rest under quadratic drag](descent-from-rest-under-quadratic-drag.md)
- [Drag coefficient](drag-coefficient.md)
- [Particle Reynolds number](particle-reynolds-number.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ia/paper-4/12c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-79/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-4/9b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-89/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-80/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-74/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-345/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ia/paper-4/4a/solution.md)
- [Quadratic drag](quadratic-drag.md)
- [Quadratic-drag turning angle](quadratic-drag-turning-angle.md)
- [Sediment entrainment threshold](sediment-entrainment-threshold.md)
- [Settling-velocity radius scaling](settling-velocity-radius-scaling.md)
- [Terminal velocity](terminal-velocity.md)
- [Viscous damping](viscous-damping.md)
