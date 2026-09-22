# Torsion stress function for a simply connected bar

↑ **Parent:** [Linear elasticity](linear-elasticity.md)

For uniform twist $\Omega$ and displacement $(-\Omega yz,\Omega xz,w(x,y))$, [linear elasticity](linear-elasticity.md) gives $\tau_{xz}=\mu(w_x-\Omega y)$ and $\tau_{yz}=\mu(w_y+\Omega x)$. Their planar divergence vanishes by axial equilibrium. On a simply connected section there is therefore a stress function $\phi$ with $\tau_{xz}=\phi_y$ and $\tau_{yz}=-\phi_x$.

The mixed derivatives of $w$ imply $\Delta\phi=-2\mu\Omega$. The lateral axial traction is the tangential derivative of $\phi$, so a traction-free connected boundary makes $\phi$ constant; choose it to be zero. Finally the torque is $M=\int_D(x\tau_{yz}-y\tau_{xz})\,dA=-\int_D(x\phi_x+y\phi_y)\,dA=2\int_D\phi\,dA$, since its boundary term vanishes. Thus one scalar [Poisson equation](poisson-s-equation.md) determines both the shear field and torsional stiffness. Multiply connected sections require additional constants and compatibility conditions on the separate boundary components.

**Table of contents**

- [Torsional warping](torsional-warping.md)
- [Elliptical-bar torsion and first yield](elliptical-bar-torsion-and-first-yield.md)

## ↑ Ancestors (6)

1. [Linear elasticity](linear-elasticity.md)
2. [Elasticity (physics)](elasticity-physics-split.md)
3. [Continuum mechanics](continuum-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Elliptical-bar torsion and first yield](elliptical-bar-torsion-and-first-yield.md)
- [Solution](past-exam-of-the-elasticity-and-plasticity-course-of-the-university-of-oxford/2008/2/solution.md)
- [Torsional warping](torsional-warping.md)
