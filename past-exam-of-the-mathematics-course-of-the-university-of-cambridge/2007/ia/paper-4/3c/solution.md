<h1 id="3c/solution">Solution</h1>

↑ **Parent:** [3C](../3c.md)

Take upward [velocity](../../../../../velocity.md) as positive, and consider the closed material system consisting of the rocket and the fuel it ejects during a short interval $dt$. Initially its mass and [momentum](../../../../../momentum.md) are $m$ and $mv$. Let $\delta m>0$ be the ejected mass, so the rocket's mass change is $dm=-\delta m$. At the end its [velocity](../../../../../velocity.md) is $v+dv$, while the ejected gas has inertial [velocity](../../../../../velocity.md) $v-u$ to first order; its downward relative [velocity](../../../../../velocity.md) need not be downward in the inertial frame.

The final total [momentum](../../../../../momentum.md), to first order, is

$$
(m-\delta m)(v+dv)+\delta m(v-u)=mv+m\,dv-u\,\delta m.
$$

Neglect air resistance and take the gravitational [acceleration](../../../../../acceleration.md) $g$ constant. The external gravitational impulse on this material system is $-mg\,dt$ to first order. [Newton's second law](../../../../../newton-s-second-law.md) therefore gives $m\,dv-u\,\delta m=-mg\,dt$, or

$$
\boxed{m\frac{dv}{dt}=-u\frac{dm}{dt}-gm.}
$$

The positive thrust is $-u\dot m$ because fuel loss makes $\dot m<0$. Applying $d(mv)/dt$ to the rocket alone without accounting for the escaping [momentum](../../../../../momentum.md) would give the wrong equation.

For constant $u$ and positive mass, divide by $m$ and integrate from release at $t=0$:

$$
v(t)=-u\ln\frac{m(t)}{m_0}-gt.
$$

Thus the gravity-corrected [rocket equation](../../../../../rocket-equation.md) is equivalent to

$$
\boxed{m(t)=m_0\exp\left[-\frac{gt+v(t)}u\right].}
$$

## ↑ Ancestors (10)

1. [3C](../3c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
