<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Since $L_z=J_\phi$, [Hamilton's equations](../../../../hamilton-s-equations.md) give

$$
\boxed{\dot L_z=-\frac{\partial H}{\partial\theta_\phi}=-\frac{\partial\delta\Phi}{\partial\theta_\phi}.}
$$

For the spherical unperturbed [Hamiltonian](../../../../hamiltonian.md), $H_0=H_0(J_r,L)$; in these particular [action-angle variables](../../../../action-angle-variables.md) the third component $\Omega_\phi=0$ describes the fixed orientation of the orbital plane. It should not be confused with the physical azimuthal [angular velocity](../../../../angular-velocity.md) of a particle around its orbit.

The conserved [normalization of a probability distribution](../../../../normalization-of-a-probability-distribution.md) $\int f\,d^3\theta\,d^3J=1$ makes the [expected value](../../../../expected-value-split.md) of specific [angular momentum](../../../../angular-momentum.md) equal to $\int L_zf\,d^3\theta\,d^3J$. Its time derivative is the [torque](../../../../torque.md) per unit halo [mass](../../../../mass.md):

$$
\boxed{\mathcal T(t)=-\int f(\boldsymbol\theta,\mathbf J,t)\frac{\partial\delta\Phi}{\partial\theta_\phi}\,d^3\theta\,d^3J.}
$$

This follows either by averaging the single-particle equation or by integrating the [Collisionless Boltzmann equation](../../../../collisionless-boltzmann-equation.md) against $L_z$, with vanishing boundary fluxes.

The term $f_0\partial_{\theta_\phi}\delta\Phi$ integrates to zero over the periodic [angle variable](../../../../angle-variable.md). Thus the first nonzero [torque](../../../../torque.md) is quadratic in the perturbation. Use the [Fourier series](../../../../fourier-series-split.md) expansions of [b](../b.md); the source's reference here to part (a) is a numbering slip. Integrating the product over all three [angle variables](../../../../angle-variable.md) yields

$$
\begin{aligned}
\mathcal T(t)
&=-(2\pi)^3\sum_{\mathbf k,\boldsymbol\ell}i\ell_\phi
\int\delta f_{\mathbf k}\delta\Phi_{\boldsymbol\ell}\,
\delta_{\mathbf k+\boldsymbol\ell,\mathbf0}\,d^3J\\
&=\boxed{i(2\pi)^3\sum_{\mathbf k}k_\phi\int\delta f_{\mathbf k}(\mathbf J,t)\delta\Phi_{\mathbf k}^*(\mathbf J,t)\,d^3J.}
\end{aligned}
$$

Reality of the [potential energy](../../../../potential-energy.md) per unit [mass](../../../../mass.md) gives $\delta\Phi_{-\mathbf k}=\delta\Phi_{\mathbf k}^*$; likewise $\delta f_{-\mathbf k}=\delta f_{\mathbf k}^*$. Conjugate harmonics make the total [torque](../../../../torque.md) real. The sum is over all integer vectors, so no extra factor of two should be inserted.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the kinetic theory course of the University of Oxford](../../../split.md)
5. [Kinetic theory course of the University of Oxford](../../../../kinetic-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
