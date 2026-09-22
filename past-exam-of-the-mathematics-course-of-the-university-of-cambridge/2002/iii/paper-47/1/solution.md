<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the [Unscaled Papkovich–Neuber representation](../../../../../unscaled-papkovich-neuber-representation.md)

$$
\mathbf u=\nabla(\mathbf x\cdot\boldsymbol\Phi+\chi)-2\boldsymbol\Phi,\qquad p=2\mu\nabla\cdot\boldsymbol\Phi,
$$

with [harmonic](../../../../../harmonic-function.md) [vector](../../../../../vector.md) and [scalar](../../../../../scalar.md) potentials. For a torque-driven [sphere](../../../../../sphere.md) choose

$$
\boldsymbol\Phi=\frac{\mathbf G\times\nabla(1/r)}{16\pi\mu},\qquad\chi=0.
$$

Its components are [harmonic](../../../../../harmonic-function.md) for $r>a$, and both $\mathbf x\cdot\boldsymbol\Phi$ and $\nabla\cdot\boldsymbol\Phi$ vanish. Hence

$$
\boxed{\mathbf u_G=\frac{\mathbf G\times\mathbf x}{8\pi\mu r^3},\quad p_G=0,\quad\boldsymbol\Omega_G=\frac{\mathbf G}{8\pi\mu a^3}.}
$$

The last equality follows from the [no-slip boundary condition](../../../../../no-slip-boundary-condition.md) at $r=a$. To check that $\mathbf G$ is indeed the applied [couple](../../../../../couple-mechanics.md), the [traction](../../../../../traction.md) on the [sphere](../../../../../sphere.md), with $\mathbf n=\mathbf x/a$ directed into the fluid, is $\boldsymbol\sigma_G\mathbf n=-3\mu\boldsymbol\Omega_G\times\mathbf n$. Its [hydrodynamic torque](../../../../../hydrodynamic-torque.md) is

$$
a\int_{r=a}\mathbf n\times(-3\mu\boldsymbol\Omega_G\times\mathbf n)dS=-8\pi\mu a^3\boldsymbol\Omega_G=-\mathbf G.
$$

Here $\int\mathbf n\mathbf n\,dS=(4\pi a^2/3)I$. The applied [couple](../../../../../couple-mechanics.md) balances this resisting [torque](../../../../../torque.md). The resulting field is the [rotlet](../../../../../rotlet.md) of a [rotating sphere in Stokes flow](../../../../../rotating-sphere-in-stokes-flow.md).

For the [Lorentz reciprocal theorem for Stokes flow](../../../../../lorentz-reciprocal-theorem-for-stokes-flow.md), let $\mathbf n_D$ point out of the fluid domain $D$ and take the same [viscosity](../../../../../dynamic-viscosity.md) in both flows. With $\nabla\cdot\boldsymbol\sigma_i+\mathbf f_i=0$, the theorem is

$$
\boxed{\int_{\partial D}(\mathbf u_1\cdot\boldsymbol\sigma_2\mathbf n_D-\mathbf u_2\cdot\boldsymbol\sigma_1\mathbf n_D)dS=\int_D(\mathbf u_2\cdot\mathbf f_1-\mathbf u_1\cdot\mathbf f_2)dV.}
$$

It follows by taking the [divergence](../../../../../divergence.md) of the boundary integrand: [incompressibility](../../../../../incompressible-flow.md) removes pressure-work terms, the two Newtonian strain contractions are equal, and the remaining [stress](../../../../../stress.md) [divergences](../../../../../divergence.md) give the displayed body-force terms. This convention matters: on the inner boundary of an exterior domain, $\mathbf n_D=-\mathbf n$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 47](../../paper-47-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
