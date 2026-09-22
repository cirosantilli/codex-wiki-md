<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $\mu$ be the instantaneous total [mass](../../../mass.md) of the rocket, including its remaining [rocket propellant](../../../rocket-propellant.md). During a short ejection it changes by $d\mu<0$. The expelled [mass](../../../mass.md) $-d\mu$ has [velocity](../../../velocity.md) $v-v_0$ to first order in a fixed [inertial frame](../../../inertial-frame.md). With no external [force](../../../force-split.md), [momentum conservation](../../../momentum-conservation.md) reads

$$
\mu v=(\mu+d\mu)(v+dv)+(-d\mu)(v-v_0).
$$

Discarding the second-order product gives $\mu\,dv=-v_0\,d\mu$. Integrate from initial total [mass](../../../mass.md) $m_0+M$ to [rocket dry mass](../../../rocket-dry-mass.md) $m_0$:

$$
v_f=-v_0\int_{m_0+M}^{m_0}\frac{d\mu}{\mu},
\qquad\boxed{v_f=v_0\ln\left(1+\frac M{m_0}\right).}
$$

For constant [mass flow rate](../../../mass-flow-rate.md) $\alpha=-\dot\mu>0$, the same [rocket equation](../../../rocket-equation.md) gives $\mu(t)=m_0+M-\alpha t$ and $v(t)=v_0\ln[(m_0+M)/\mu(t)]$ until $t=M/\alpha$. The final result depends on the [rocket mass ratio](../../../rocket-mass-ratio.md), not on how rapidly the fuel is ejected. These are Newtonian [velocities](../../../velocity.md); a very large [rocket mass ratio](../../../rocket-mass-ratio.md) would require a relativistic treatment even if the exhaust is slow in the instantaneous rocket frame.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [2017](../../2017-split.md)
3. [Past exam of the physics 1 paper of the University of Oxford](../../split.md)
4. [Physics 1 paper of the University of Oxford](../../../physics-1-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
