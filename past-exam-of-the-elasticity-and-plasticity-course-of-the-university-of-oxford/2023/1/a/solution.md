<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For [antiplane shear](../../../../antiplane-shear.md), the [displacement field](../../../../displacement-field-mechanics.md) is $\mathbf u=(0,0,w(x,y,t))$, independent of $z$. Its [divergence](../../../../divergence.md) is zero. Consequently the only possibly nonzero components of the [stress tensor](../../../../cauchy-stress-tensor.md) are the [shear stresses](../../../../shear-stress.md)

$$
\tau_{xz}=\tau_{zx}=\mu w_x,\qquad
\tau_{yz}=\tau_{zy}=\mu w_y.
$$

The $x$ and $y$ components of the [Navier-Cauchy equation](../../../../navier-cauchy-equation.md) vanish identically. Its $z$ component gives $\rho w_{tt}=\partial_x(\mu w_x)+\partial_y(\mu w_y)$. Each material has constant [shear modulus](../../../../shear-modulus.md) and [mass density](../../../../density.md), so the required [wave equation](../../../../wave-equation-split.md) and [wave speeds](../../../../wave-speed.md) are

$$
\boxed{w_{j,tt}=c_j^2(w_{j,xx}+w_{j,yy}),\qquad
c_j=\sqrt{\frac{\mu_j}{\rho_j}},\quad j=1,2.}
$$

At a [perfectly bonded elastic interface](../../../../perfectly-bonded-elastic-interface.md), both the [displacement field](../../../../displacement-field-mechanics.md) and the [traction](../../../../traction.md) are continuous. Using the same normal $\mathbf e_y$ on both sides, the only nonzero [traction](../../../../traction.md) component is $\tau_{zy}$. Thus the interface [boundary conditions](../../../../boundary-condition.md) are

$$
\boxed{w_1(x,h,t)=w_2(x,h,t),\qquad
\mu_1w_{1,y}(x,h,t)=\mu_2w_{2,y}(x,h,t).}
$$

[Continuity](../../../../continuous-function.md) of “stress” here means [continuity](../../../../continuous-function.md) of [traction](../../../../traction.md); it does not require equality of the full [stress tensors](../../../../cauchy-stress-tensor.md). The rigid plate supplies the remaining [boundary condition](../../../../boundary-condition.md) $w_1(x,0,t)=0$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the elasticity and plasticity course of the University of Oxford](../../../split.md)
5. [Elasticity and plasticity course of the University of Oxford](../../../../elasticity-and-plasticity-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
