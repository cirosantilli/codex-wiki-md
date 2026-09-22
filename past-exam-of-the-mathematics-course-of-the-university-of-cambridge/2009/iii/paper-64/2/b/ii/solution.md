<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the aligned poloidal flow from part (i), and define the [magnetohydrodynamic mass loading](../../../../../../../magnetohydrodynamic-mass-loading.md) $\eta=\rho\alpha$, so $\rho\mathbf u_p=\eta\mathbf B_p$. Axisymmetric [mass conservation](../../../../../../../mass-conservation.md) and $\nabla\cdot\mathbf B_p=0$ give $\mathbf B_p\cdot\nabla\eta=0$. Introduce the [poloidal magnetic flux function](../../../../../../../poloidal-magnetic-flux-function.md) $\Psi$ by $\mathbf B_p=R^{-1}\nabla\Psi\times\mathbf e_\phi$, and write $u_\phi=R\Omega$. Then

$$
\mathbf u\times\mathbf B=(u_\phi-\alpha B_\phi)\mathbf e_\phi\times\mathbf B_p=\left(\Omega-\frac{\eta B_\phi}{\rho R}\right)\nabla\Psi.
$$

The steady induction equation says the curl of this expression is zero. Hence $\nabla\Omega_F\times\nabla\Psi=0$, where

$$
\Omega_F=\Omega-\frac{\eta B_\phi}{\rho R};
$$

the [field-line angular velocity](../../../../../../../field-line-angular-velocity.md) $\Omega_F$ is constant on each connected magnetic surface and along its field lines.

To control the difference between matter rotation and field-line rotation, use the azimuthal component of the [ideal magnetohydrodynamic momentum equation](../../../../../../../ideal-magnetohydrodynamic-momentum-equation.md). The inertial and magnetic terms are respectively $\rho R^{-1}\mathbf u_p\cdot\nabla(Ru_\phi)$ and $(\mu_0R)^{-1}\mathbf B_p\cdot\nabla(RB_\phi)$; [pressure](../../../../../../../pressure.md) and gravity have no azimuthal derivative. Multiplying by $R$ and using constant mass loading gives

$$
\mathbf B_p\cdot\nabla\left(R^2\Omega-\frac{RB_\phi}{\mu_0\eta}\right)=0.
$$

Thus the [magnetohydrodynamic angular-momentum invariant](../../../../../../../magnetohydrodynamic-angular-momentum-invariant.md) $L=R^2\Omega-RB_\phi/(\mu_0\eta)$ is constant along the line when $\eta\ne0$. Let $v_{Ap}=|\mathbf B_p|/\sqrt{\mu_0\rho}$ and define $M_{Ap}^2=|\mathbf u_p|^2/v_{Ap}^2=\mu_0\eta^2/\rho$. Eliminating $B_\phi$ between the two invariants gives

$$
\boxed{\Omega=\frac{\Omega_F-M_{Ap}^2L/R^2}{1-M_{Ap}^2},\qquad \Omega-\Omega_F=\frac{M_{Ap}^2}{1-M_{Ap}^2}\left(\Omega_F-\frac{L}{R^2}\right).}
$$

For a highly sub-Alfvénic poloidal flow, $M_{Ap}^2\ll1$, this is $\Omega\simeq\Omega_F$ along a nonsingular field-line segment. This proves [sub-Alfvénic isorotation in a steady axisymmetric wind](../../../../../../../sub-alfvenic-isorotation-in-a-steady-axisymmetric-wind.md), with the correction explicitly displayed. If the poloidal flow is exactly zero, the induction equation directly gives $\mathbf B_p\cdot\nabla\Omega=0$, namely [Ferraro's law of isorotation](../../../../../../../ferraro-s-law-of-isorotation.md). The approximate claim presumes regular invariants: small $M_{Ap}$ alone is not a uniform relative bound if $L/R^2$ is allowed to become arbitrarily large.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 64](../../../../paper-64-split.md)
5. [Iii](../../../../split.md)
6. [2009](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
