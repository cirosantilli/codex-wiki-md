<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose the amplitude $U$ real and positive locally, absorbing its phase into $\Theta$, and work away from vortex cores or other density zeros. Put $\rho=U^2$ and $\theta=\Theta/\epsilon$. Direct separation of the real and imaginary parts of the [Gross–Pitaevskii equation](../../../../../../gross-pitaevskii-equation.md) gives the exact [Madelung equations](../../../../../../madelung-equations.md)

$$
\rho_t+\nabla\cdot(\rho\mathbf v_s)=0,\qquad \mathbf v_s=\nabla\theta,
$$



$$
\theta_t+\frac12|\mathbf v_s|^2=1-\rho+\frac{\nabla^2U}{2U}-\zeta D_n\rho,
\qquad D_n=\partial_t+\mathbf v_n\cdot\nabla.
$$

For example, the imaginary part is $-U_t=\nabla U\cdot\nabla\theta+(U/2)\nabla^2\theta$, which proves the density equation after multiplication by $2U$. The real damping coefficient affects the phase balance rather than adding a particle source.

Using this [continuity equation](../../../../../../continuity-equation.md) and $\nabla\cdot\mathbf v_n=0$,

$$
D_n\rho=-\nabla\cdot(\rho\mathbf v_s)+\mathbf v_n\cdot\nabla\rho
=-\nabla\cdot[\rho(\mathbf v_s-\mathbf v_n)].
$$

Taking a [gradient](../../../../../../gradient.md) of the phase equation gives the exact [velocity](../../../../../../velocity.md) equation

$$
\partial_t\mathbf v_s+\frac12\nabla|\mathbf v_s|^2
=-\nabla(\rho-1)+\frac12\nabla\left(\frac{\nabla^2U}U\right)
+\zeta\nabla\nabla\cdot[\rho(\mathbf v_s-\mathbf v_n)].
$$

Now $\nabla_x=\epsilon\nabla_X$, $\partial_t=\epsilon\partial_T$, and $\mathbf v_s=\nabla_X\Theta$ is order one. The inertial and chemical-potential gradients are $O(\epsilon)$; the double-gradient bulk term is $O(\epsilon^2)$; and the [quantum potential](../../../../../../quantum-potential.md) force contains three slow derivatives and is $O(\epsilon^3)$, provided $U$ stays bounded away from zero. Through order $\epsilon^2$ this proves the requested [bulk-viscous limit of a material-density-damped condensate](../../../../../../bulk-viscous-limit-of-a-material-density-damped-condensate.md) with

$$
\boxed{\rho_s=U^2,\qquad\mathbf v_s=\nabla_X\Theta,\qquad\mu=U^2-1,\qquad\xi=\zeta.}
$$

Adding a spatially constant value to $\mu$ does not affect the equation, so $\mu=U^2$ is an equivalent convention. The density and viscosity coefficients are in the equation's dimensionless units. The [bulk viscosity](../../../../../../volume-viscosity.md) term is the [gradient](../../../../../../gradient.md) of the divergence of the relative mass flux, not a shear-viscosity term. At density zeros the slow-amplitude expansion and the division by $U$ fail; there one must retain the original field equation.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 83](../../../paper-83-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
