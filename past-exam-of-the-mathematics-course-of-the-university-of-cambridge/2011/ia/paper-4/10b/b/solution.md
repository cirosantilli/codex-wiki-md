<h1 id="10b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Neglect the [centrifugal acceleration](../../../../../../centrifugal-acceleration.md), which is of order $\omega^2$, and use the local flat-surface approximation. To zeroth order in $\omega$, the height above $P$ and flight time are

$$
z_0(t)=vt-\frac12gt^2,\qquad \dot z_0=v-gt,\qquad T_0=\frac{2v}{g}.
$$

Inserting this vertical [velocity](../../../../../../velocity.md) into the [Coriolis acceleration](../../../../../../coriolis-acceleration.md) gives the eastward component

$$
\ddot x=-2\omega\sin\theta\,(v-gt)+O(\omega^2).
$$

With $x(0)=\dot x(0)=0$, two integrations yield

$$
\dot x=-2\omega\sin\theta\left(vt-\frac12gt^2\right),\qquad
x=-\omega\sin\theta\left(vt^2-\frac13gt^3\right)
$$

to first order. Horizontal [velocity](../../../../../../velocity.md) is already of order $\omega$, so its effect on vertical acceleration is of order $\omega^2$. Thus the flight time remains $T_0$ at this order. The [Coriolis deflection of a vertical projectile](../../../../../../coriolis-deflection-of-a-vertical-projectile.md) at landing is

$$
\boxed{x(T_0)=-\frac{4\omega v^3}{3g^2}\sin\theta.}
$$

The displacement is **westward**, and its magnitude is $4\omega v^3\sin\theta/(3g^2)$. The horizontal speed remains westward during the flight: $\dot x=-2\omega\sin\theta\,z_0(t)$. This explains why the eastward acceleration on descent does not cancel the earlier displacement.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [10B](../../10b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
