<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

[Inertia](../../../inertia.md) is resistance to a change of motion. Translational [inertia](../../../inertia.md) is measured by [mass](../../../mass.md) in [Newton's second law](../../../newton-s-second-law.md); rotational [inertia](../../../inertia.md) about a specified fixed axis is measured by the [moment of inertia](../../../moment-of-inertia.md)

$$
I=\int r_\perp^2\,dm,
$$

where $r_\perp$ is perpendicular [distance](../../../distance.md) from that axis. For a thin uniform rod, take axes perpendicular to the rod. With [linear mass density](../../../linear-mass-density.md) $\lambda=m/l$,

$$
I_{\rm CM}=\frac ml\int_{-l/2}^{l/2}x^2\,dx=\frac{ml^2}{12},\qquad
\boxed{I_{\rm end}=I_{\rm CM}+m\left(\frac l2\right)^2=\frac{ml^2}{3}.}
$$

The second result uses the [parallel axis theorem](../../../parallel-axis-theorem.md); direct [integration](../../../integral-split.md) over $0\leq x\leq l$ gives the same value. The axis specification is essential: an ideal thin rod has zero [moment of inertia](../../../moment-of-inertia.md) about its own longitudinal axis.

During the short [elastic collision](../../../elastic-collision.md), neglect the [impulse](../../../impulse.md) from gravity. The pivot can exert an external [impulse](../../../impulse.md), so total linear [momentum](../../../momentum-split.md) of rod plus particle need not be conserved. Its [torque](../../../torque.md) about the pivot is zero, so [conservation of angular momentum](../../../conservation-of-angular-momentum.md) about that point applies. Let $w$ be the particle's signed outgoing horizontal [velocity](../../../velocity.md), and $\omega$ the rod's outgoing [angular velocity](../../../angular-velocity.md), positive towards the incident motion. Then

$$
mlv_0=mlw+I_{\rm end}\omega,\qquad
\frac12mv_0^2=\frac12mw^2+\frac12I_{\rm end}\omega^2.
$$

Substituting $\omega=3(v_0-w)/l$ into the [kinetic energy](../../../kinetic-energy.md) equation gives

$$
v_0^2=w^2+3(v_0-w)^2,
\qquad (v_0-w)(v_0-2w)=0.
$$

Discarding the zero-[impulse](../../../impulse.md) branch $w=v_0$, the actual [collision](../../../collision.md) gives

$$
\boxed{w=\frac{v_0}{2}\quad\text{forward},\qquad
\omega=\frac{3v_0}{2l}.}
$$

The rod's lower end initially moves forward at $l\omega=3v_0/2$, so the bodies separate. Afterwards the free particle undergoes [projectile motion](../../../projectile-motion.md). With the pivot as origin and $z$ downward, its [trajectory](../../../trajectory.md) is $x=(v_0/2)t$, $z=l+gt^2/2$, where $t=0$ at the [collision](../../../collision.md). The rod instead swings about the fixed pivot in a vertical plane as a [physical pendulum](../../../physical-pendulum.md).

The rod's initial rotational [kinetic energy](../../../kinetic-energy.md) is $I_{\rm end}\omega^2/2=3mv_0^2/8$. Reaching the horizontal raises its [centre of mass](../../../center-of-mass.md) by $l/2$, increasing [gravitational potential energy](../../../gravitational-energy.md) by $mgl/2$. Consequently,

$$
\boxed{v_0^2\geq\frac{4gl}{3}\ \text{to reach the horizontal},\qquad
v_0=\sqrt{\frac{4gl}{3}}\ \text{to just reach it at rest}.}
$$

For the threshold case, measure the rod's [angle](../../../angle.md) $\theta$ from the downward vertical and reset $t=0$ at its first horizontal [turning point](../../../turning-point.md), so $\theta(0)=\pi/2$ and $\dot\theta(0)=0$. The restoring [torque](../../../torque.md) about the pivot gives the exact [equation of motion](../../../equation-of-motion.md)

$$
\boxed{\ddot\theta+\frac{3g}{2l}\sin\theta=0.}
$$

At the horizontal, $\ddot\theta=-3g/(2l)$, so the rod immediately swings back. [Conservation of mechanical energy](../../../conservation-of-mechanical-energy.md) yields

$$
\frac12\frac{ml^2}{3}\dot\theta^2+\frac{mgl}{2}(1-\cos\theta)=\frac{mgl}{2},
\qquad
\dot\theta^2=\frac{3g}{l}\cos\theta.
$$

On the initial descent its explicit time dependence is specified by the [definite integral](../../../definite-integral.md)

$$
\boxed{t=\sqrt{\frac{l}{3g}}\int_{\theta(t)}^{\pi/2}\frac{d\alpha}{\sqrt{\cos\alpha}}.}
$$

It continues through the vertical to $-\pi/2$, reverses, and repeats without damping. An alternative expression valid throughout the oscillation uses the [Jacobi elliptic sine](../../../jacobi-elliptic-sine.md). Put $k=1/\sqrt2$, $\omega_r=\sqrt{3g/(2l)}$, and let $K(k)$ denote the [complete elliptic integral of the first kind](../../../complete-elliptic-integral-of-the-first-kind.md). Then

$$
\boxed{\theta(t)=2\arcsin\!\left[k\,\operatorname{sn}\!\left(K(k)-\omega_rt,k\right)\right],\qquad
T_r=4\sqrt{\frac{2l}{3g}}\,K\!\left(\frac1{\sqrt2}\right).}
$$

This is not [simple harmonic motion](../../../simple-harmonic-motion.md) at an [amplitude](../../../wave-amplitude.md) of $\pi/2$. Its [oscillation period](../../../period-of-an-oscillation.md) exceeds its own small-[amplitude](../../../wave-amplitude.md) value $2\pi\sqrt{2l/(3g)}$ by the factor $2K(1/\sqrt2)/\pi\simeq1.18034$.

A [simple pendulum](../../../simple-pendulum-split.md) of [length](../../../length.md) $l/2$ obeys $\ddot\theta+(2g/l)\sin\theta=0$. At the same [amplitude](../../../wave-amplitude.md) $\pi/2$, its [oscillation period](../../../period-of-an-oscillation.md) is $T_p=4\sqrt{l/(2g)}K(1/\sqrt2)$, so

$$
\boxed{\frac{T_r}{T_p}=\frac{2}{\sqrt3}>1.}
$$

The rod swings more slowly. Its equivalent [simple pendulum](../../../simple-pendulum-split.md) [length](../../../length.md) is $I_{\rm end}/[m(l/2)]=2l/3$, not the [distance](../../../distance.md) $l/2$ to its [centre of mass](../../../center-of-mass.md). The same [oscillation period](../../../period-of-an-oscillation.md) ratio holds in the common small-[amplitude](../../../wave-amplitude.md) limit, but replacing the actual 90-degree motion by that limit would underestimate both [oscillation periods](../../../period-of-an-oscillation.md).

## ↑ Ancestors (11)

1. [7](../7.md)
2. [2021](../../2021-split.md)
3. [Past exam of the physics 1 paper of the University of Oxford](../../split.md)
4. [Physics 1 paper of the University of Oxford](../../../physics-1-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
