# Simple-shear traction angle for a Mooney-Rivlin solid

↑ **Parent:** [Mooney-Rivlin solid](mooney-rivlin-solid.md)

For incompressible [simple shear](simple-shear.md) $F=I+\gamma\mathbf e_1\otimes\mathbf e_2$ with Mooney-Rivlin energy $\alpha(I_1-3)+\beta(I_2-3)$, zero traction on the third-coordinate faces fixes the pressure reaction. The remaining Cauchy stress has $T_{11}=2\alpha\gamma^2$, $T_{22}=-2\beta\gamma^2$ and $T_{12}=2(\alpha+\beta)\gamma$. The material face $x_1=\text{constant}$ has current unit normal $\mathbf n=(1,-\gamma,0)/\sqrt{1+\gamma^2}$ and tangent $\mathbf m=(\gamma,1,0)/\sqrt{1+\gamma^2}$. Resolving $T\mathbf n$ gives $N=-2\gamma^2(\alpha+2\beta+\beta\gamma^2)/(1+\gamma^2)$ and $S=2\gamma(\alpha+\beta)/(1+\gamma^2)$. Since $N<0$, the traction-normal angle satisfies $\tan(\theta-\pi/2)=-N/|S|$, proving the displayed formula. Consequently its two-sided small-shear slope is $(\alpha+2\beta)/(\alpha+\beta)$. The reference normal cannot replace the transformed normal in this calculation.

## ↑ Ancestors (8)

1. [Mooney-Rivlin solid](mooney-rivlin-solid.md)
2. [Hyperelastic material](hyperelastic-material.md)
3. [Finite elasticity](finite-elasticity.md)
4. [Elasticity (physics)](elasticity-physics-split.md)
5. [Continuum mechanics](continuum-mechanics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-solid-mechanics-course-of-the-university-of-oxford/2009/2/solution.md)
