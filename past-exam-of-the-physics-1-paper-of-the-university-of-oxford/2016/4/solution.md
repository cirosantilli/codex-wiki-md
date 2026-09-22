<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $u_e>0$ be the constant rearward [rocket exhaust speed](../../../rocket-exhaust-speed.md), and let $\mathcal M$ denote the rocket's instantaneous [mass](../../../mass.md). Apply [momentum conservation](../../../momentum-conservation.md) over a short ejection interval: the remaining rocket gains $\mathcal M\,dv$, while the expelled positive mass $-d\mathcal M$ carries backward relative momentum $u_e\,d\mathcal M$. To first order,

$$
\mathcal M\,dv=-u_e\,d\mathcal M.
$$

Integrating gives the [rocket equation](../../../rocket-equation.md)

$$
\boxed{\Delta v=u_e\ln\frac{M}{M-m}.}
$$

This is a [velocity](../../../velocity.md) increment, measured along the thrust direction, for motion in free space without external [forces](../../../force-split.md).

For the two-stage vehicle, take $M_1$ and $M_2$ to be the initial masses of the respective stages, each including its fuel $m$. The first burn changes the total mass from $M_1+M_2$ to $M_1+M_2-m$. Discarding the empty first-stage shell of mass $M_1-m$ leaves mass $M_2$; ideal jettison without a relative impulse does not change the [velocity](../../../velocity.md). The second burn then changes $M_2$ to $M_2-m$. Adding the two [rocket equation](../../../rocket-equation.md) increments gives

$$
\boxed{\Delta v_{\mathrm{two}}=u_e\ln\frac{M_1+M_2}{M_1+M_2-m}+u_e\ln\frac{M_2}{M_2-m}.}
$$

Here $M_1>m$ and $M_2>m$ leave positive dry masses. Different stage exhaust speeds would multiply their respective logarithms. A [multistage rocket](../../../multistage-rocket.md) gains its advantage by avoiding acceleration of the spent first-stage shell during the second burn.

## ↑ Ancestors (11)

1. [4](../4.md)
2. [2016](../../2016-split.md)
3. [Past exam of the physics 1 paper of the University of Oxford](../../split.md)
4. [Physics 1 paper of the University of Oxford](../../../physics-1-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
