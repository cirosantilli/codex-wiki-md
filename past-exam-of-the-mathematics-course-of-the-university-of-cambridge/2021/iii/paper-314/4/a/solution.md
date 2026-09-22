<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The divergence-free poloidal field can be represented by the [poloidal magnetic flux function](../../../../../../poloidal-magnetic-flux-function.md)

$$
\mathbf B_p=\nabla\psi\times\nabla\phi
=-\frac1r\mathbf e_\phi\times\nabla\psi.
$$

In a steady axisymmetric [ideal magnetohydrodynamics](../../../../../../ideal-magnetohydrodynamics.md) flow, the azimuthal component of $\nabla\times(\mathbf u\times\mathbf B)=0$ makes $\mathbf u_p$ parallel to $\mathbf B_p$. Write

$$
\boxed{\rho\mathbf u_p=k\mathbf B_p}.
$$

Mass conservation and $\nabla\cdot\mathbf B=0$ then imply $\mathbf B\cdot\nabla k=0$, so the [magnetohydrodynamic mass loading](../../../../../../magnetohydrodynamic-mass-loading.md) $k=k(\psi)$ is constant along each magnetic line.

The poloidal part of $\mathbf u\times\mathbf B$ is

$$
\mathbf u\times\mathbf B
=\frac1r\left(u_\phi-\frac{kB_\phi}{\rho}\right)\nabla\psi.
$$

Its curl vanishes only if its coefficient is a flux function, giving the [field-line angular velocity](../../../../../../field-line-angular-velocity.md)

$$
\boxed{\frac{u_\phi}{r}-\frac{kB_\phi}{r\rho}=\omega(\psi)}.
$$

The azimuthal component of momentum conservation is a divergence of matter and magnetic angular-momentum flux. Dividing its field-line constant by the mass loading yields the [magnetohydrodynamic angular-momentum invariant](../../../../../../magnetohydrodynamic-angular-momentum-invariant.md)

$$
\boxed{ru_\phi-\frac{rB_\phi}{\mu_0k}=\ell(\psi)}.
$$

The conservative total-energy equation similarly gives the [magnetohydrodynamic Bernoulli invariant](../../../../../../magnetohydrodynamic-bernoulli-invariant.md)

$$
\boxed{\frac12|\mathbf u|^2+\Phi+h
-\frac{r\omega B_\phi}{\mu_0k}=\epsilon(\psi)}.
$$

Finally, the [entropy advection equation](../../../../../../entropy-advection-equation.md) and $\mathbf u_p\parallel\mathbf B_p$ imply $s=s(\psi)$. Thus $k,\omega,\ell,\epsilon$, and $s$ are constant along each magnetic field line.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 314](../../../paper-314-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
