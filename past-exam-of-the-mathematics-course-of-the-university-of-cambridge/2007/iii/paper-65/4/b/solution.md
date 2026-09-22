<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

To distinguish [Eulerian and Lagrangian fluid perturbations](../../../../../../eulerian-and-lagrangian-fluid-perturbations.md), use $\boldsymbol\xi=(\xi_x,\xi_y,\xi_z)$ for the [fluid displacement](../../../../../../lagrangian-displacement-fluid-mechanics.md), $\phi=\Phi'$ for the Eulerian potential perturbation, and $\delta\rho$ for the Eulerian [mass density](../../../../../../density.md) perturbation. The equilibrium [mass density](../../../../../../density.md) $\rho(z)$ is the profile from part (a); subscript $z$ below denotes differentiation. Linearized [mass conservation](../../../../../../mass-conservation.md) and the [isothermal equation of state](../../../../../../globally-isothermal-equation-of-state.md) give

$$
\delta\rho=-ik\rho\xi_x-(\rho\xi_z)_z,\qquad
\delta p=c_s^2\delta\rho.
$$

The [velocity](../../../../../../velocity.md) perturbation is $-i\omega\boldsymbol\xi$. Linearized momentum initially has the form

$$
-\omega^2\rho\boldsymbol\xi=-\nabla\delta p-\delta\rho\nabla\Phi_0-\rho\nabla\phi.
$$

Since $\nabla\Phi_0=-c_s^2\nabla\ln\rho$, the [pressure](../../../../../../pressure.md) and perturbed [mass density](../../../../../../density.md) gravity terms combine into $-\rho\nabla(c_s^2\delta\rho/\rho)$. Define $W=c_s^2\delta\rho/\rho+\phi$. The closed linearized system is

$$
\boxed{\omega^2\xi_x=ikW,\qquad \omega^2\xi_z=W_z,\qquad
\omega^2\xi_y=0,\qquad
\phi_{zz}-k^2\phi=4\pi G\delta\rho,\qquad
\delta\rho=-ik\rho\xi_x-(\rho\xi_z)_z}.
$$

The $y$ component is a neutral transverse sector; it vanishes for nonzero-frequency modes.

To prove reality rather than assume it, multiply momentum by $\rho\boldsymbol\xi^*$ and integrate over $z$. With $I=\int\rho|\boldsymbol\xi|^2dz>0$, [integration by parts](../../../../../../integration-by-parts.md) and the conjugate [continuity equation](../../../../../../continuity-equation.md) give

$$
\omega^2I=\left[\rho\xi_z^*W\right]_{-\infty}^{\infty}
+c_s^2\int\frac{|\delta\rho|^2}{\rho}\,dz+\int\delta\rho^*\phi\,dz.
$$

Using the conjugate [Poisson equation for Newtonian gravity](../../../../../../poisson-equation-for-newtonian-gravity.md) in the last integral gives

$$
\int\delta\rho^*\phi\,dz
=\frac1{4\pi G}\left[\phi\phi_z^*\right]_{-\infty}^{\infty}
-\frac1{4\pi G}\int(|\phi_z|^2+k^2|\phi|^2)\,dz.
$$

Take disturbances with finite $I$, finite [pressure](../../../../../../pressure.md) and gravitational integrals, and vanishing [pressure](../../../../../../pressure.md) work and gravitational boundary terms. For $k\ne0$, require the potential to decay at both infinities and the [fluid displacement](../../../../../../lagrangian-displacement-fluid-mechanics.md) to make $\rho\xi_z^*W\to0$ as well. In a source-free outer region the decaying potential is proportional to $e^{-|k||z|}$. The [isothermal displacement energy of a self-gravitating slab](../../../../../../isothermal-displacement-energy-of-a-self-gravitating-slab.md) then gives

$$
\boxed{\omega^2 I=c_s^2\int\frac{|\delta\rho|^2}{\rho}\,dz
-\frac1{4\pi G}\int(|\phi_z|^2+k^2|\phi|^2)\,dz\in\mathbb R}.
$$

Since $I$ is strictly positive for a nonzero displacement, **$\omega^2$ is real**. Positive values describe oscillations; negative values give pure growth and decay. The result is the [energy](../../../../../../energy.md) identity for the pressure-gravity displacement operator, a [self-adjoint operator](../../../../../../self-adjoint-operator.md) in the [mass density](../../../../../../density.md)-weighted [inner product](../../../../../../inner-product.md). The identity excludes an oscillatory growing eigenmode under these [boundary conditions](../../../../../../boundary-condition.md). At $k=0$ the same identity applies when its boundary terms vanish and its integrals remain finite, with the gravitational integral involving only $|\phi_z|^2$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
