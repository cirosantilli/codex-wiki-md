<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The retained [mass](../../../mass.md) at time $t$ is $M(t)=M_0+kt$. Incoming rain has zero horizontal [momentum](../../../momentum-split.md) in the ground [reference frame](../../../reference-frame.md). During $dt$, horizontal [momentum conservation](../../../momentum-conservation.md) for the carriage and the rain about to enter gives

$$
M(t)u(t)=[M(t)+k\,dt][u(t)+du]+O(dt^2),
$$

so

$$
M\dot u+ku=0,\qquad
\boxed{u(t)=\frac{M_0u_0}{M_0+kt}.}
$$

This is a [variable-mass system](../../../variable-mass-system.md): the entering [mass](../../../mass.md) must be accelerated horizontally, even though no external horizontal [force](../../../force-split.md) acts on the carriage-plus-rain system. Integrating the [velocity](../../../velocity.md),

$$
\boxed{x(t)-x(0)=\int_0^t\frac{M_0u_0}{M_0+ks}\,ds
=\frac{M_0u_0}{k}\ln\left(1+\frac{kt}{M_0}\right).}
$$

For $u_0\ge0$ this is also the distance travelled. Its $k\to0$ limit is $u_0t$. Vertical impact can dissipate [kinetic energy](../../../kinetic-energy.md); horizontal [momentum conservation](../../../momentum-conservation.md) does not require [kinetic energy](../../../kinetic-energy.md) conservation.

## ↑ Ancestors (11)

1. [5](../5.md)
2. [2019 resit](../../2019-resit-split.md)
3. [Past exam of the physics 1 paper of the University of Oxford](../../split.md)
4. [Physics 1 paper of the University of Oxford](../../../physics-1-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
