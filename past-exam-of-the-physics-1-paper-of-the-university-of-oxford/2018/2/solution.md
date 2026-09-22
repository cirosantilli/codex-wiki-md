<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Take the [rocket exhaust speed](../../../rocket-exhaust-speed.md) $u$ relative to the hovering ship, with exhaust directed vertically downward. If $\alpha=-\dot M>0$ is the [mass flow rate](../../../mass-flow-rate.md), the upward [rocket thrust](../../../rocket-thrust.md) is $u\alpha$. For example, over a short interval $dt$, the expelled mass $\alpha dt$ acquires downward [momentum](../../../momentum-split.md) $-u\alpha dt$, giving the opposite recoil to the ship. Balancing its weight requires

$$
u\alpha(t)=M(t)g,\qquad\frac{dM}{dt}=-\frac gu M.
$$

Solving this [differential equation](../../../differential-equation-split.md) with $M(0)=M_0$ yields the [hovering rocket mass flow](../../../hovering-rocket-mass-flow.md)

$$
\boxed{M(t)=M_0e^{-gt/u},\qquad
\alpha(t)=\frac{gM_0}{u}e^{-gt/u}.}
$$

The required [mass flow rate](../../../mass-flow-rate.md) decreases because the mass to support decreases. These expressions apply while fuel is available and $g,u$ remain constant. If the [rocket dry mass](../../../rocket-dry-mass.md) is $M_d>0$, hovering ends at $t=(u/g)\log(M_0/M_d)$; the mathematical limit $M\to0$ is not a model of an indefinitely fuelled physical ship.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2018](../../2018-split.md)
3. [Past exam of the physics 1 paper of the University of Oxford](../../split.md)
4. [Physics 1 paper of the University of Oxford](../../../physics-1-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
