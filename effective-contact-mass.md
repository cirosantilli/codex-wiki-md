# Effective contact mass

↑ **Parent:** [Rigid-body collision](rigid-body-collision.md)

A normal [impulse](impulse.md) $j$ on a free planar [rigid body](rigid-body-dynamics-split.md) of [mass](mass.md) $M$ and [moment of inertia](moment-of-inertia.md) $I$, at perpendicular lever arm $b$, changes the contact point's normal [velocity](velocity.md) by $j(1/M+b^2/I)$. Its effective mass in that direction is therefore $(1/M+b^2/I)^{-1}$. This follows by adding the translational change $j/M$ to the rotational contribution $b(jb/I)$.

For an incoming [point mass](point-mass.md) $m$, the inverse reduced contact mass is $1/m+1/M+b^2/I$. A smooth [elastic collision](elastic-collision.md) with initial relative approach speed $u$ has impulse $2u/(1/m+1/M+b^2/I)$, since the relative normal velocity reverses. This separates effective inertia at a contact from the body's total mass and explains the lever-arm dependence in an [equal-speed elastic impact on a free rod](equal-speed-elastic-impact-on-a-free-rod.md).

## ↑ Ancestors (6)

1. [Rigid-body collision](rigid-body-collision.md)
2. [Rigid body dynamics](rigid-body-dynamics-split.md)
3. [Classical mechanics](classical-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-physics-1-paper-of-the-university-of-oxford/2019/4/solution.md)
