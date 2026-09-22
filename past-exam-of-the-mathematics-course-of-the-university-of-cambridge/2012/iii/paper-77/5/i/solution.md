<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the same length, thermal-time, velocity and temperature scales as in thermal convection. Write the imposed [magnetic field](../../../../../../magnetic-field.md) as $B_0\hat{\mathbf z}$ and measure its perturbation in units of $B_0$. The physical linear [magnetohydrodynamic momentum equation](../../../../../../magnetohydrodynamic-momentum-equation.md) contains magnetic tension $(B_0^2/\mu_0)\partial_z\mathbf b$; the gradient part of the [Lorentz force density](../../../../../../lorentz-force-density.md) is absorbed into [magnetohydrodynamic total pressure](../../../../../../magnetohydrodynamic-total-pressure.md).

Divide the momentum equation by the viscous force scale $\rho_0\nu\kappa/d^3$. Its acceleration coefficient is $\kappa/\nu=1/\sigma$ and its magnetic coefficient is

$$
\frac{B_0^2d^2}{\mu_0\rho_0\nu\kappa}=Q\zeta,\qquad \zeta=\frac\eta\kappa,\qquad Q=\frac{B_0^2d^2}{\mu_0\rho_0\eta\nu}.
$$

Here $Q$ is the [Chandrasekhar number](../../../../../../chandrasekhar-number.md), comparing magnetic and viscous-diffusive effects, and $\zeta$ is the ratio of [magnetic diffusivity](../../../../../../magnetic-diffusivity.md) to [thermal diffusivity](../../../../../../thermal-diffusivity.md). The induction scale is $B_0\kappa/d^2$, so linearization gives

$$
\boxed{\frac1\sigma\dot{\mathbf u}=-\nabla P+Q\zeta\partial_z\mathbf b+R\theta\hat{\mathbf z}+\nabla^2\mathbf u,\qquad \dot{\mathbf b}=\partial_z\mathbf u+\zeta\nabla^2\mathbf b.}
$$

Complete the linear system with $\dot\theta=w+\nabla^2\theta$, $\nabla\cdot\mathbf u=0$ and the [solenoidal magnetic-field constraint](../../../../../../solenoidal-magnetic-field-constraint.md) $\nabla\cdot\mathbf b=0$. The omitted advective and perturbed-field tension terms are quadratic in the disturbances. Magnetic tension resists bending of the vertical field, while diffusion allows that bending to relax.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [5](../../5.md)
3. [Section III](../../section-iii.md)
4. [Paper 77](../../../paper-77-split.md)
5. [Iii](../../../split.md)
6. [2012](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
