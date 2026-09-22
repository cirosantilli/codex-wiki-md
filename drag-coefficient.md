# Drag coefficient

↑ **Parent:** [Drag (physics)](drag-physics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Drag_coefficient)

The [drag coefficient](drag-coefficient.md) measures a [drag force](drag-physics.md) against a specified scale of [force](force.md). Let $\mathbf U=\mathbf v_{\rm body}-\mathbf u_\infty$ be the body's [velocity](velocity.md) relative to the distant, undisturbed [fluid](fluid.md), and let $U=|\mathbf U|>0$ be its relative [speed](speed.md). For [fluid](fluid.md) [density](density.md) $\rho$, [drag force](drag-physics.md) magnitude $F_D$ and reference [area](surface-area.md) $A>0$, define

$$
C_D=\frac{F_D}{\tfrac12\rho U^2A},\qquad F_D=\tfrac12\rho U^2AC_D.
$$

The [drag coefficient](drag-coefficient.md) is a [dimensionless quantity](dimensionless-quantity.md): the denominator has units of [force](force.md). The reference [area](surface-area.md) must be reported with it. For a [sphere](sphere.md) of radius $a$, the usual choice is the frontal [area](surface-area.md) $A=\pi a^2$. Choosing its entire surface [area](surface-area.md) $4\pi a^2$ instead divides the reported [drag coefficient](drag-coefficient.md) by four for the same physical [drag force](drag-physics.md). Comparing coefficients without comparing their reference [areas](surface-area.md) can therefore be misleading. [NASA Glenn Research Center, Drag Coefficient, definition and Determining Value for Drag Coefficient](https://www1.grc.nasa.gov/beginners-guide-to-aeronautics/drag-coefficient/)

For a rigid [sphere](sphere.md) in [steady flow](steady-flow.md) through an unbounded [Newtonian fluid](newtonian-fluid.md) with constant [dynamic viscosity](dynamic-viscosity.md) $\mu$, [incompressible flow](incompressible-flow.md) and the [no-slip boundary condition](no-slip-boundary-condition.md), the creeping-flow limit requires the diameter-based [particle Reynolds number](particle-reynolds-number.md) $\mathrm{Re}_d=2a\rho U/\mu\ll1$. The [Stokes drag law](stokes-s-law.md) gives $F_D=6\pi\mu aU$. Substitution into the definition with $A=\pi a^2$ gives the short derivation

$$
C_D=\frac{6\pi\mu aU}{\tfrac12\rho U^2\pi a^2}=\frac{12\mu}{\rho aU}=\frac{24}{\mathrm{Re}_d}.
$$

Thus the [drag coefficient](drag-coefficient.md) is neither necessarily constant nor bounded above by one. The formula containing $U^2$ still describes [linear drag](linear-drag.md) here, because the [drag coefficient](drag-coefficient.md) varies as $1/U$. The relation $C_D=24/\mathrm{Re}_d$ is the leading small-[Reynolds number](reynolds-number.md) approximation, not a measured curve valid at every [Reynolds number](reynolds-number.md). [Richard Fitzpatrick, Axisymmetric Stokes Flow Around a Solid Sphere, equations 10.126 and 10.129](https://farside.ph.utexas.edu/teaching/336L/Fluid/node142.html)

For a worked example, stipulate [dynamic viscosity](dynamic-viscosity.md) $\mu=0.10\,\mathrm{Pa\,s}$, [density](density.md) $\rho=1000\,\mathrm{kg\,m^{-3}}$, radius $a=10^{-4}\,\mathrm m$ and relative [speed](speed.md) $U=10^{-3}\,\mathrm{m\,s^{-1}}$. Within the stated [Stokes drag law](stokes-s-law.md) assumptions,

$$
\mathrm{Re}_d=0.002,\qquad C_D=12000,\qquad F_D=6\pi\times10^{-8}\,\mathrm N\approx1.88495559\times10^{-7}\,\mathrm N.
$$

Doubling the relative [speed](speed.md) with all other parameters fixed gives $\mathrm{Re}_d=0.004$ and $C_D=6000$: the predicted [drag force](drag-physics.md) doubles to $3.76991118\times10^{-7}\,\mathrm N$. Falsely holding the [drag coefficient](drag-coefficient.md) at $12000$ would instead quadruple the [drag force](drag-physics.md). Both [particle Reynolds numbers](particle-reynolds-number.md) remain small, so the comparison is within the creeping-flow approximation.

<a id="image-sphere-drag-coefficient-in-the-creeping-flow-approximation"></a>
![](sphere-drag-coefficient-stokes-limit.png)

**[Figure 11](#image-sphere-drag-coefficient-in-the-creeping-flow-approximation). Sphere drag coefficient in the creeping-flow approximation**. The mathematical approximation $C_D=24/\mathrm{Re}_d$ is plotted only for small diameter-based [particle Reynolds number](particle-reynolds-number.md), using frontal reference [area](surface-area.md) $A=\pi a^2$. The two dots mark the worked example and its doubled relative [speed](speed.md). This is a creeping-limit curve, not empirical data or an extension of the [Stokes drag law](stokes-s-law.md) to all [Reynolds numbers](reynolds-number.md).

The useful idea is to separate the [force](force.md) scale from the dependence on geometry and flow conditions. A [drag coefficient](drag-coefficient.md) can help compare experiments, but changing [Reynolds number](reynolds-number.md) can change the coefficient itself; NASA Glenn explicitly stresses matching the relevant flow conditions. The elegant cancellation above also exposes a common mistake: a [drag coefficient](drag-coefficient.md) definition does not by itself impose a [quadratic drag](quadratic-drag.md) law.

## ↑ Ancestors (5)

1. [Drag (physics)](drag-physics.md)
2. [Fluid mechanics](fluid-mechanics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (15)

- [Drag coefficient](drag-coefficient.md)
- [Dynamic pressure](dynamic-pressure.md)
- [Linear friction coefficient](linear-friction-coefficient.md)
- [Particle Reynolds number](particle-reynolds-number.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-83/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-89/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-65/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-61/2/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-74/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-345/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-345/4/b/solution.md)
- [Quadratic drag](quadratic-drag.md)
- [Sediment entrainment threshold](sediment-entrainment-threshold.md)
- [Settling-velocity radius scaling](settling-velocity-radius-scaling.md)
- [Shields parameter](shields-parameter.md)
