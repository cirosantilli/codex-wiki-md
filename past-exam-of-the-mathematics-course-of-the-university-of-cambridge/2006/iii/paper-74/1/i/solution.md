<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $D_t=\partial_t+\mathbf u\cdot\nabla$ for the [material derivative](../../../../../../material-derivative.md). The [resistive induction equation](../../../../../../resistive-induction-equation.md), together with the [solenoidal](../../../../../../solenoidal-vector-field.md) conditions on both fields, is

$$
D_t\mathbf B=(\mathbf B\cdot\nabla)\mathbf u+\eta\Delta\mathbf B,\qquad \nabla\cdot\mathbf B=\nabla\cdot\mathbf u=0.
$$

Since $D_t\mathbf x=\mathbf u$, the [product rule](../../../../../../product-rule.md) gives

$$
D_tP=\mathbf x\cdot D_t\mathbf B+\mathbf B\cdot\mathbf u,\qquad
\mathbf B\cdot\nabla Q=\mathbf x\cdot[(\mathbf B\cdot\nabla)\mathbf u]+\mathbf B\cdot\mathbf u.
$$

Also $\Delta P=\mathbf x\cdot\Delta\mathbf B+2\nabla\cdot\mathbf B=\mathbf x\cdot\Delta\mathbf B$. Substitution proves the [radial magnetic induction scalar](../../../../../../radial-magnetic-induction-scalar.md) equation:

$$
\boxed{\partial_tP+\mathbf u\cdot\nabla P=\mathbf B\cdot\nabla Q+\eta\Delta P\quad(r<a).}
$$

In the insulating exterior the quasistatic [magnetic field](../../../../../../magnetic-field.md) is current-free, so $\nabla\times\mathbf B=0$ and $\nabla\cdot\mathbf B=0$. Thus $\Delta\mathbf B=0$ and **$\Delta P=0$ for $r>a$**, with decay at infinity for an isolated field. This is an instantaneous exterior [Laplace equation](../../../../../../laplace-equation.md), rather than a diffusion equation with the interior value of $\eta$.

Use the usual nonmagnetic-interface assumptions: equal [magnetic permeability](../../../../../../permeability-electromagnetism.md) on both sides and no surface current. The [electromagnetic boundary conditions](../../../../../../electromagnetic-boundary-condition.md) then make $B_r$ and the tangential [magnetic field](../../../../../../magnetic-field.md) continuous. Hence $P=rB_r$ is continuous. In spherical coordinates, the [solenoidal magnetic-field constraint](../../../../../../solenoidal-magnetic-field-constraint.md) reads

$$
\partial_rP=-B_r-\operatorname{div}_{S^2}\mathbf B_{\mathrm{tan}},
$$

where the last term is the angular [divergence](../../../../../../divergence.md) on the unit sphere. Its right-hand side is also continuous, giving the [insulating boundary condition for the radial magnetic scalar](../../../../../../insulating-boundary-condition-for-the-radial-magnetic-scalar.md):

$$
\boxed{[P]_{r=a}=0,\qquad[\partial_rP]_{r=a}=0.}
$$

Equivalently, the decaying exterior degree-$l$ [spherical harmonic](../../../../../../spherical-harmonic.md) is proportional to $r^{-(l+1)}$, so its boundary amplitude satisfies $\partial_rP_{lm}(a)=-(l+1)P_{lm}(a)/a$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
