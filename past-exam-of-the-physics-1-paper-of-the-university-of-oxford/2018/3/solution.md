<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $\theta$ be the displacement from the upward vertical and $v$ the [speed](../../../speed.md) of the ball's [centre of mass](../../../center-of-mass.md). Its centre follows a circle of radius $R+r$. The [rolling without slipping](../../../rolling-without-slipping.md) constraint is $v=r\omega$, with $\omega$ the ball's spin [angular velocity](../../../angular-velocity.md). The static contact [friction](../../../friction.md) does no work on the ball because the instantaneous contact point is stationary. Thus [conservation of energy](../../../conservation-of-energy.md) gives

$$
Mg(R+r)(1-\cos\theta)
=\frac12Mv^2+\frac12\left(\frac25Mr^2\right)\frac{v^2}{r^2}
=\frac7{10}Mv^2.
$$

Project [Newton's second law](../../../newton-s-second-law.md) toward the hemisphere's centre. The inward component of gravity is $Mg\cos\theta$ and the [normal force](../../../normal-force.md) $N$ points outward, so

$$
Mg\cos\theta-N=\frac{Mv^2}{R+r}.
$$

At contact loss $N=0$. Eliminating $v$ gives the ideal [sphere rolling off a hemisphere](../../../sphere-rolling-off-a-hemisphere.md) result

$$
\frac{10}{7}(1-\cos\theta_d)=\cos\theta_d,
\qquad
\boxed{\cos\theta_d=\frac{10}{17},\quad\theta_d\simeq53.97^\circ.}
$$

The radius cancels, so replacing $R+r$ by $R$ under the stated small-ball approximation leaves the same answer.

**Finite-friction qualification.** This is an ideal rolling-constraint result. It does not describe uninterrupted pure rolling to detachment with any finite [coefficient of static friction](../../../coefficient-of-static-friction.md). The tangential [force](../../../force-split.md) and [torque](../../../torque.md) equations give

$$
M\dot v=Mg\sin\theta-f,\qquad
fr=\frac25Mr^2\frac{\dot v}{r},
$$

so $f=(2/7)Mg\sin\theta$ acts uphill, whereas

$$
N=\frac{Mg}{7}(17\cos\theta-10).
$$

Consequently the required ratio is

$$
\boxed{\frac fN=\frac{2\sin\theta}{17\cos\theta-10}\longrightarrow\infty
\quad\text{as }\theta\to\theta_d^-.}
$$

For a concrete example, a [coefficient of static friction](../../../coefficient-of-static-friction.md) of one allows rolling only up to about $47.54^\circ$, where $17\cos\theta-10=2\sin\theta$, before sliding begins. A subsequent physical contact-loss angle needs a sliding-friction model. The boxed $53.97^\circ$ answers the source's expressly imposed no-slip idealization.

## ↑ Ancestors (11)

1. [3](../3.md)
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
