# Rigid rotation minimizes kinetic energy at fixed angular momentum

↑ **Parent:** [Kinetic energy](kinetic-energy.md)

For rotational motion about a fixed axis, let $r$ be cylindrical radius, $v$ the signed tangential [velocity](velocity.md), and $dm$ the mass measure. Define the [kinetic energy](kinetic-energy.md), axial [angular momentum](angular-momentum.md), and [moment of inertia](moment-of-inertia.md) by

$$
K=\frac12\int v^2\,dm,\qquad L=\int rv\,dm,\qquad I=\int r^2\,dm>0.
$$

The [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) gives $L^2\leq(\int v^2dm)(\int r^2dm)=2KI$. More precisely, direct expansion gives the nonnegative energy gap

$$
K-\frac{L^2}{2I}=\frac12\int\left(v-\frac LI r\right)^2dm.
$$

Thus the minimum at fixed $L$ and fixed mass distribution occurs exactly when $v=(L/I)r$ almost everywhere with respect to $dm$. This means constant [angular velocity](angular-velocity.md) $\Omega=L/I$, or [solid-body rotation](solid-body-rotation.md). If the profile is continuous, the equality holds at every point in the mass support.

For a uniform unit-density [cylinder](cylinder-geometry.md) of radius $a$, height $h$, and [volume](volume.md) $V=\pi a^2h$, the [moment of inertia](moment-of-inertia.md) is $I=Va^2/2$. Therefore $K\geq L^2/(Va^2)$, with equality for $\omega(r)=2L/(Va^2)$. Multiplying by a uniform nonunit [density](density.md) changes the mass measure and $I$ consistently.

## ↑ Ancestors (6)

1. [Kinetic energy](kinetic-energy.md)
2. [Energy](energy-split.md)
3. [Classical mechanics](classical-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
