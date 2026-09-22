<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In the rotating [shearing sheet](../../../../../../shearing-sheet.md), write the background orbital shear as $\mathbf U_0=-q\Omega x\mathbf e_y$. The rotating momentum equation contains [Coriolis acceleration](../../../../../../coriolis-acceleration.md) $2\boldsymbol\Omega\times\mathbf u$ and the [shearing-sheet tidal potential](../../../../../../shearing-sheet-tidal-potential.md); the background shear balances the radial tidal acceleration.

Set

$$
\mathbf u=\mathbf U_0+(v_x(z,t),v_y(z,t),0),\qquad
\mathbf B=(B_x(z,t),B_y(z,t),B_z).
$$

[Gauss's law for magnetism](../../../../../../gauss-s-law-for-magnetism.md) gives $\partial_zB_z=0$, and the vertical [ideal magnetohydrodynamic induction equation](../../../../../../ideal-magnetohydrodynamic-induction-equation.md) gives $\partial_tB_z=0$. Horizontal invariance and $v_z=0$ remove the nonlinear horizontal advection. The remaining background-shear term is $(\mathbf v\mathbin\cdot\nabla)\mathbf U_0=-q\Omega v_x\mathbf e_y$. The horizontal [magnetic tension](../../../../../../magnetic-tension.md) is $B_z\partial_z\mathbf B_h/\mu_0$, while horizontal pressure gradients vanish. Subtracting background balance yields

$$
\boxed{\partial_tv_x-2\Omega v_y=\frac{B_z}{\mu_0\rho}\partial_zB_x},\qquad
\boxed{\partial_tv_y+(2-q)\Omega v_x=\frac{B_z}{\mu_0\rho}\partial_zB_y}.
$$

For [ideal magnetohydrodynamics](../../../../../../ideal-magnetohydrodynamics.md), the [ideal magnetohydrodynamic induction equation](../../../../../../ideal-magnetohydrodynamic-induction-equation.md) is $\partial_t\mathbf B+\mathbf u\mathbin\cdot\nabla\mathbf B=\mathbf B\mathbin\cdot\nabla\mathbf u$. Its horizontal components give

$$
\boxed{\partial_tB_x=B_z\partial_zv_x},\qquad
\boxed{\partial_tB_y+q\Omega B_x=B_z\partial_zv_y}.
$$

These [horizontally invariant magnetized shearing-sheet equations](../../../../../../horizontally-invariant-magnetized-shearing-sheet-equations.md) are exact within the stated local, incompressible ansatz, even for finite horizontal amplitudes. The vertical equation determines the pressure needed to balance vertical gravity and [magnetic pressure](../../../../../../magnetic-pressure.md); it does not add another horizontal evolution equation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 321](../../../paper-321-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
