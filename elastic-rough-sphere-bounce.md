# Elastic rough-sphere bounce

↑ **Parent:** [Rigid-body collision](rigid-body-collision.md)

An ideal [elastic collision](elastic-collision.md) between a sphere and a stationary plane reverses normal approach [velocity](velocity.md). On the fully rough, tangentially elastic branch, the tangential [contact-point velocity](contact-point-velocity.md) reverses too. If $K_t$ is the signed tangential [impulse](impulse.md), translation and spin obey $M\Delta v=K_t$ and $I\Delta\Omega=aK_t$, with positive spin anticlockwise. Restoring tangential translational plus rotational [kinetic energy](kinetic-energy.md) gives

$$
0=K_t(v+a\Omega)+\frac12K_t^2(M^{-1}+a^2/I).
$$

The nonzero root is the displayed [impulse](impulse.md); the other root is the smooth-contact branch. For $I=2Ma^2/5$, the map is $v'=(3v-4a\Omega)/7$ and $a\Omega'=-(10v+3a\Omega)/7$. It preserves [kinetic energy](kinetic-energy.md) and the [angular momentum](angular-momentum.md) about the contact point, $I\Omega-Mav$. An unspecified rough surface need not realize this idealization: finite [friction](friction.md) or a dissipative tangential contact law requires additional constitutive data. Setting the outgoing contact slip to zero instead loses $M(v+a\Omega)^2/7$ of [kinetic energy](kinetic-energy.md) for this uniform sphere.

## ↑ Ancestors (6)

1. [Rigid-body collision](rigid-body-collision.md)
2. [Rigid body dynamics](rigid-body-dynamics-split.md)
3. [Classical mechanics](classical-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-physics-1-paper-of-the-university-of-oxford/2017/8/d/solution.md)
