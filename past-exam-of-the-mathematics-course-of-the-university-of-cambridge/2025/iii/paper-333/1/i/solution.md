<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $\mathbf u=(u,v)$ and let the layer thickness be $H=H_0+\eta$. The inviscid [shallow water equations](../../../../../../shallow-water-equations.md) are

$$
\frac{D\mathbf u}{Dt}+f\widehat{\mathbf z}\times\mathbf u
=-g\nabla(\eta-h_b),
\qquad
H_t+\nabla\mathbin\cdot(H\mathbf u)=0.
$$

They follow from a homogeneous incompressible fluid with small aspect ratio, [hydrostatic pressure](../../../../../../hydrostatic-pressure.md), negligible vertical acceleration, horizontal velocity nearly uniform through the depth, a material free surface, and a rigid stationary bottom. Rotation may be represented by an [f-plane](../../../../../../f-plane.md) or [beta plane](../../../../../../beta-plane.md). The model is useful because many atmospheric and oceanic motions are horizontally much broader than their depth, while the free surface or an internal density interface still supports waves and [potential vorticity](../../../../../../potential-vorticity.md) dynamics.

Let $\zeta=v_x-u_y$. Taking the vertical curl of momentum gives

$$
\frac{D(\zeta+f)}{Dt}=-(\zeta+f)\nabla\mathbin\cdot\mathbf u,
$$

where $Df/Dt=\beta v$ supplies the planetary-vorticity term when $f$ varies. Continuity gives $DH/Dt=-H\nabla\cdot\mathbf u$. Combining the two equations yields material conservation of [shallow-water potential vorticity](../../../../../../shallow-water-potential-vorticity.md):

$$
\boxed{q=\frac{\zeta+f}{H},
\qquad \frac{Dq}{Dt}=0.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 333](../../../paper-333-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
