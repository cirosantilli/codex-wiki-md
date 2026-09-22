# Collision contact geometry is not determined by incoming velocities

↑ **Parent:** [Oblique collision](oblique-collision.md)

In a smooth [oblique collision](oblique-collision.md), the [impulse](impulse.md) is parallel to the contact normal $\mathbf n$, while tangential [velocity](velocity.md) components remain unchanged. Incoming [velocities](velocity.md), [masses](mass.md), and a [coefficient of restitution](coefficient-of-restitution.md) do not determine the outgoing [velocities](velocity.md) until that contact normal, or equivalent scattering data, is specified. For an [elastic collision](elastic-collision.md) of [masses](mass.md) $3m,m$, incoming [velocities](velocity.md) $(-u,0)$ and $(\sqrt3w/2,w/2)$, and outgoing first [velocity](velocity.md) $(0,h)$, [conservation of momentum](momentum-conservation.md) and conservation of [kinetic energy](kinetic-energy.md) give $w(\sqrt3u+h)=2u^2+4h^2$. Thus specifying only the first outgoing $x$ component leaves a family: $h=0$ gives $w=2u/\sqrt3$, while $h=u/\sqrt3$ gives $w=5\sqrt3u/6$.

## ↑ Ancestors (7)

1. [Oblique collision](oblique-collision.md)
2. [Collision mechanics](collision-mechanics.md)
3. [Particle dynamics](particle-dynamics.md)
4. [Classical mechanics](classical-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
