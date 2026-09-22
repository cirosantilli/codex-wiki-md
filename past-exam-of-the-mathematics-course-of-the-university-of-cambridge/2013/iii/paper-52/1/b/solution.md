<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For this geometry $\nabla\cdot\mathbf u=0$, $\nabla\cdot\mathbf B=0$ and $\mathbf u\cdot\nabla=0$. Consequently constant [mass density](../../../../../../density.md) and [pressure](../../../../../../pressure.md) satisfy the full nonlinear continuity and adiabatic pressure equations. Write $\mathbf B_\perp=(B_x,B_y)$ and $\mathbf u_\perp=(u_x,u_y)$. The [ideal magnetohydrodynamic induction equation](../../../../../../ideal-magnetohydrodynamic-induction-equation.md) and the transverse [ideal magnetohydrodynamic momentum equation](../../../../../../ideal-magnetohydrodynamic-momentum-equation.md) become

$$
\partial_t\mathbf B_\perp=B_z\partial_z\mathbf u_\perp,\qquad
\rho\partial_t\mathbf u_\perp=\frac{B_z}{\mu_0}\partial_z\mathbf B_\perp.
$$

The longitudinal momentum equation is

$$
0=-\frac{1}{2\mu_0}\partial_z|\mathbf B_\perp|^2.
$$

Thus constant transverse magnetic magnitude eliminates the otherwise unavoidable [magnetic pressure](../../../../../../magnetic-pressure.md) acceleration. Differentiating the [ideal magnetohydrodynamic induction equation](../../../../../../ideal-magnetohydrodynamic-induction-equation.md) in time gives, for either transverse component,

$$
\boxed{\partial_t^2W=\frac{B_z^2}{\mu_0\rho}\partial_z^2W.}
$$

A constant-magnitude [nonlinear Alfvén wave](../../../../../../nonlinear-alfven-wave.md) is obtained by taking $B_z\ne0$ and

$$
B_x=A\cos F(z-ct),\qquad B_y=A\sin F(z-ct),\qquad
c=\pm\frac{B_z}{\sqrt{\mu_0\rho}},\qquad
\mathbf u_\perp=\mathbf U_0-\frac{c}{B_z}\mathbf B_\perp,
$$

where $A$ and $\mathbf U_0$ are constants and $F$ is any sufficiently differentiable real function. Both first-order equations hold, and $B_x^2+B_y^2=A^2$. **Taking $F(\zeta)=k\zeta$ gives an exact finite-amplitude circularly polarized wave.** More general traveling rotations also work; an arbitrary superposition of oppositely traveling solutions of the [wave equation](../../../../../../wave-equation-split.md) need not preserve transverse magnetic magnitude and hence need not solve the full nonlinear system. If $B_z=0$, the coupled first-order equations instead require time-independent transverse fields and velocities, with spatially constant transverse magnetic magnitude; there is no propagating [Alfvén wave](../../../../../../alfven-wave.md) in the $z$ direction.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 52](../../../paper-52-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
