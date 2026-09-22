<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Interpret $h$ as the vertical drop of the cylinder's [centre of mass](../../../center-of-mass.md), and initially take the suspended rod to be vertical. The [moment of inertia of a uniform solid cylinder](../../../moment-of-inertia-of-a-uniform-solid-cylinder.md) is $I=mr^2/2$. Before impact, [rolling without slipping](../../../rolling-without-slipping.md) gives $\omega=u/r$, so [conservation of mechanical energy](../../../conservation-of-mechanical-energy.md) gives

$$
mgh=\frac12mu^2+\frac12I\frac{u^2}{r^2}=\frac34mu^2,
\qquad u=\sqrt{\frac{4gh}{3}}.
$$

Use the usual instantaneous smooth [elastic collision](../../../elastic-collision.md) model: the horizontal impact [impulse](../../../impulse.md) passes through the cylinder's [centre of mass](../../../center-of-mass.md), and the floor supplies negligible tangential [impulse](../../../impulse.md) during impact. The cylinder's [angular velocity](../../../angular-velocity.md) is then unchanged during impact; its [rotational kinetic energy](../../../rotational-kinetic-energy.md) does not transfer to the bob. The rod supplies no horizontal [impulse](../../../impulse.md) when vertical. If $v$ and $V$ are the signed cylinder and bob [velocities](../../../velocity.md) immediately afterwards, [conservation of momentum](../../../momentum-conservation.md) and the unit [coefficient of restitution](../../../coefficient-of-restitution.md) give

$$
mu=mv+2mV,\qquad V-v=u,
\qquad v=-\frac u3,\quad V=\frac{2u}{3}.
$$

During the subsequent [simple pendulum](../../../simple-pendulum-split.md) swing, [conservation of mechanical energy](../../../conservation-of-mechanical-energy.md) gives

$$
\frac12(2m)V^2=2mgh(1-\cos\theta_{\max}),
\qquad
\boxed{\cos\theta_{\max}=\frac{19}{27},\quad
\theta_{\max}=\cos^{-1}\frac{19}{27}\simeq45.28^\circ.}
$$

The cylinder generally slips immediately after this impact, which is consistent with imposing [rolling without slipping](../../../rolling-without-slipping.md) only on the descent.

**Impact convention matters.** The [floor-impulse dependence of a rolling-cylinder collision](../../../floor-impulse-dependence-of-a-rolling-cylinder-collision.md) gives a different answer if a different constraint is imposed. If instead the floor enforces [rolling without slipping](../../../rolling-without-slipping.md) throughout the impulsive [collision](../../../collision.md), it supplies a nonzero horizontal [impulse](../../../impulse.md). The cylinder's effective translational [mass](../../../mass.md) is then $m+I/r^2=3m/2$. Writing $J$ for the [impulse](../../../impulse.md) delivered to the bob gives $(3m/2)(v-u)=-J$, $2mV=J$ and $V-v=u$. Hence $V=6u/7$ and $\cos\theta_{\max}=25/49$, giving $59.32^\circ$. The original wording specifies the descent constraint but does not specify an impulsive floor-friction law; the first boxed value uses the smooth-impact convention.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2021 resit](../../2021-resit-split.md)
3. [Past exam of the physics 1 paper of the University of Oxford](../../split.md)
4. [Physics 1 paper of the University of Oxford](../../../physics-1-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
