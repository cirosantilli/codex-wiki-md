<h1 id="11c/solution">Solution</h1>

↑ **Parent:** [11C](../11c.md)

Label the initially left-hand rod $A$ and the right-hand rod $B$. At impact their centres are $(0,\ell)$ and $(0,-\ell)$, and their contact points are both the origin. Each rod has total mass $2m$ and [moment of inertia](../../../../../moment-of-inertia.md)

$$
I=m\ell^2+m\ell^2=2m\ell^2.
$$

Let the [impulse](../../../../../impulse.md) on $B$ be $+J\mathbf e_x$, so the [impulse](../../../../../impulse.md) on $A$ is $-J\mathbf e_x$. The impulsive form of [Newton's second law](../../../../../newton-s-second-law.md) gives

$$
\mathbf v_A=\left(V-\frac{J}{2m},0\right),\qquad
\mathbf v_B=\left(-V+\frac{J}{2m},0\right).
$$

The contact lever arms from the centres are $(0,-\ell)$ for $A$ and $(0,+\ell)$ for $B$. Both angular [impulses](../../../../../impulse.md) are $-\ell J\mathbf e_z$. Thus, taking counterclockwise rotation as positive,

$$
\omega_A=\omega_B=-\frac{\ell J}{I}=-\frac{J}{2m\ell}.
$$

Equal and opposite linear [impulses](../../../../../impulse.md) therefore produce equal clockwise rotations, not opposite rotations.

The restitution law uses the velocities of the contacting endpoints, including the rotational terms. For $A$ that velocity is

$$
u_A=V-\frac{J}{2m}+\ell\omega_A=V-\frac Jm,
$$

and for $B$ it is $u_B=-V+J/m$. The approach speed before impact is $2V$. The [coefficient of restitution](../../../../../coefficient-of-restitution.md) $e$ therefore gives

$$
u_B-u_A=-2V+\frac{2J}{m}=2eV,\qquad J=mV(1+e).
$$

Substituting into the centre and [angular velocities](../../../../../angular-velocity.md) yields the [endpoint collision of two freely rotating equal rods](../../../../../endpoint-collision-of-two-freely-rotating-equal-rods.md):

$$
\boxed{\mathbf v_A=\left(\frac{1-e}{2}V,0\right),\qquad
\mathbf v_B=\left(-\frac{1-e}{2}V,0\right),\qquad
\omega_A=\omega_B=-\frac{1+e}{2\ell}V.}
$$

For the first, perfectly elastic case, $e=1$, so

$$
\boxed{\mathbf v_A=\mathbf v_B=(0,0),\qquad
\omega_A=\omega_B=-\frac V\ell.}
$$

All initial translational energy has become rotational energy. Indeed the total initial [kinetic energy](../../../../../kinetic-energy.md) is $2mV^2$, while the final energy for general $e$ is

$$
K_{\mathrm{final}}
=2\left(m\frac{(1-e)^2V^2}{4}
+m\ell^2\frac{(1+e)^2V^2}{4\ell^2}\right)
=mV^2(1+e^2).
$$

The loss is $mV^2(1-e^2)$, zero for an [elastic collision](../../../../../elastic-collision.md). Conservation of total [angular momentum](../../../../../angular-momentum.md) about the origin provides another check: initially it is $-4m\ell V$; after collision the centre-motion contribution is $-2m\ell V(1-e)$ and the spins contribute $-2m\ell V(1+e)$, with the same total. The initial distance $d$ determines when the collision occurs but does not enter the impulsive velocities.

## ↑ Ancestors (10)

1. [11C](../11c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
