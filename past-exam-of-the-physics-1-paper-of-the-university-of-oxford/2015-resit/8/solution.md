<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

**Descent equation.** Take downward [velocity](../../../velocity.md) $v$ and underwater depth $z$ as positive, with $z=0$ at the lake surface. For a [sphere](../../../sphere.md) of radius $r$, the pebble [mass](../../../mass.md) is $m=4\pi r^3\rho_p/3$ and the frontal [area](../../../surface-area.md) is $A=\pi r^2$. [Newton's second law](../../../newton-s-second-law.md) includes downward [gravitational weight](../../../weight-physics.md), upward [buoyancy](../../../buoyancy.md) and upward [quadratic drag](../../../quadratic-drag.md):

$$
m\dot v=mg-\rho_w\frac{4\pi r^3}{3}g-\frac12C\rho_w\pi r^2v^2
\qquad(v\geq0).
$$

Thus

$$
\boxed{\dot v=g\left(1-\frac{\rho_w}{\rho_p}\right)-bv^2,\qquad \dot z=v,\qquad b=\frac{3C\rho_w}{8\rho_pr}.}
$$

Here $b$ has units of inverse [length](../../../length.md). For arbitrary signed [velocity](../../../velocity.md), the last term is $-bv|v|$, so [drag](../../../drag-physics.md) always opposes motion. The displayed downward form suffices for this trajectory.

**Limiting speed.** At [terminal velocity](../../../terminal-velocity.md), the net [force](../../../force-split.md) and $\dot v$ vanish. For $\rho_p>\rho_w$,

$$
\boxed{v_t=\sqrt{\frac{8rg(\rho_p-\rho_w)}{3C\rho_w}}.}
$$

Use $\rho_p=2500\,\mathrm{kg\,m^{-3}}$, $\rho_w=1000\,\mathrm{kg\,m^{-3}}$, $r=0.020\,\mathrm m$, $C=0.7$ and $g=9.81\,\mathrm{m\,s^{-2}}$. Then

$$
b=5.25\,\mathrm{m^{-1}},\qquad g_{\mathrm{eff}}=g(1-\rho_w/\rho_p)=5.886\,\mathrm{m\,s^{-2}},
\qquad\boxed{v_t\simeq1.059\,\mathrm{m\,s^{-1}}.}
$$

The $\rho_p-\rho_w$ factor is essential: omitting [buoyancy](../../../buoyancy.md) would overestimate the limiting [speed](../../../speed.md).

For the numerical descent, assume the pebble is released from rest, neglect air [drag](../../../drag-physics.md), take $g$ and the water [mass density](../../../density.md) as constant, and apply the given constant [drag coefficient](../../../drag-coefficient.md) once it is submerged. Neglect the finite entry interval, entry energy losses and [added mass](../../../added-mass.md), so its initial underwater [speed](../../../speed.md) is

$$
u=\sqrt{2gH_a}=\sqrt{2g\times5\,\mathrm m}\simeq9.905\,\mathrm{m\,s^{-1}}>v_t.
$$

It consequently slows down towards [terminal velocity](../../../terminal-velocity.md); a rest-starting underwater trajectory would describe a different initial condition.

## ↑ Ancestors (11)

1. [8](../8.md)
2. [2015 resit](../../2015-resit-split.md)
3. [Past exam of the physics 1 paper of the University of Oxford](../../split.md)
4. [Physics 1 paper of the University of Oxford](../../../physics-1-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
