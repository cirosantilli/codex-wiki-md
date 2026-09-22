# Axisymmetry of the inertia tensor

↑ **Parent:** [Inertia tensor](inertia-tensor.md)

If a [rigid body](rigid-body-dynamics-split.md)'s [mass density](density.md) is invariant under every [rotation](rotation-mathematics.md) about an axis through its [centre of mass](center-of-mass.md), its [inertia tensor](inertia-tensor.md) in any [orthonormal basis](orthonormal-basis.md) with third vector on that axis has the displayed form. In particular all transverse directions are [principal axes](principal-axis.md) with equal [principal moments of inertia](principal-moment-of-inertia.md).

For a proof, let that axis be $z$. In the defining integrals for the [inertia tensor](inertia-tensor.md), a half-turn $(x,y,z)\mapsto(-x,-y,z)$ makes the $xz$ and $yz$ products change sign, so their integrals vanish. A quarter-turn $(x,y,z)\mapsto(-y,x,z)$ makes the $xy$ integral vanish and equates the integrals of $x^2$ and $y^2$. Therefore all off-diagonal components vanish and $I_{11}=I_{22}$. The values are $I_\perp=\int\rho[(x^2+y^2)/2+z^2]\,d^3r$ and $I_\parallel=\int\rho(x^2+y^2)\,d^3r$. No reflection symmetry in $z$ is needed.

## ↑ Ancestors (7)

1. [Inertia tensor](inertia-tensor.md)
2. [Moment of inertia](moment-of-inertia.md)
3. [Rigid body dynamics](rigid-body-dynamics-split.md)
4. [Classical mechanics](classical-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-classical-mechanics-course-of-the-university-of-oxford/2023/2/a/ii/solution.md)
