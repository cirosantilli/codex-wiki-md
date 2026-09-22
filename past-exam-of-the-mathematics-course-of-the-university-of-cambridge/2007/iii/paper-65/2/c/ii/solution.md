<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the circular [MHD wave polarization](../../../../../../../magnetohydrodynamic-wave-polarization.md), $B_x^2+B_y^2=a^2B_0^2$ is constant. Choose any constant $\rho_0>0,p_0>0$, put $v_a=B_0/\sqrt{\mu_0\rho_0}$ and take

$$
\boxed{\mathbf u=-a v_a(\cos\zeta,\sin\zeta,0),\qquad
\rho=\rho_0,\qquad p=p_0,\qquad \zeta=k(z-v_at)}.
$$

This gives a [circularly polarized nonlinear Alfvén wave](../../../../../../../circularly-polarized-nonlinear-alfven-wave.md) of arbitrary amplitude. All fields depend only on $z,t$, and $u_z=0$, so $\mathbf u\cdot\nabla\mathbf u=0$ and $\nabla\cdot\mathbf u=0$. Constant [mass density](../../../../../../../density.md) and [pressure](../../../../../../../pressure.md) then satisfy continuity and the adiabatic [pressure](../../../../../../../pressure.md) equation, and $\nabla\cdot\mathbf B=0$ because $B_z$ is constant.

The remaining [ideal magnetohydrodynamic induction equation](../../../../../../../ideal-magnetohydrodynamic-induction-equation.md) and transverse [magnetohydrodynamic momentum equation](../../../../../../../magnetohydrodynamic-momentum-equation.md) are

$$
\partial_t\mathbf B_\perp=B_0\partial_z\mathbf u_\perp,\qquad
\rho_0\partial_t\mathbf u_\perp=\frac{B_0}{\mu_0}\partial_z\mathbf B_\perp.
$$

Since $\partial_t=-v_a\partial_z$ on the traveling profiles and $\mathbf u_\perp=-(v_a/B_0)\mathbf B_\perp$, both identities hold exactly when $v_a^2=B_0^2/(\mu_0\rho_0)$. The longitudinal [magnetohydrodynamic momentum equation](../../../../../../../magnetohydrodynamic-momentum-equation.md) holds because $p+|\mathbf B_\perp|^2/(2\mu_0)$ is constant. **The circularly polarized wave is therefore an exact nonlinear solution even though the fluid is compressible.** Compressibility permits [mass density](../../../../../../../density.md) changes; it does not require every possible motion to compress the gas.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 65](../../../../paper-65-split.md)
5. [Iii](../../../../split.md)
6. [2007](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
