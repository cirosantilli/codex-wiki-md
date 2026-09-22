<h1 id="15e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A fixed [comoving volume](../../../../../../comoving-volume.md) $d^3q$ labels a fixed collection of cold dark matter particles. Their background mass is $a^3\bar\rho\,d^3q$, which is constant by [mass conservation](../../../../../../mass-conservation.md). At the perturbed positions it is $\rho\,d^3r$. The [Jacobian determinant](../../../../../../jacobian-determinant.md) of the [Zeldovich approximation](../../../../../../zeldovich-approximation.md) map is

$$
\det\frac{\partial r_i}{\partial q_j}=a^3\det(I+\partial_j\psi_i)=a^3[1+\nabla_q\cdot\boldsymbol\psi]+O(\psi^2).
$$

Taking its reciprocal and using mass conservation gives

$$
\boxed{d^3q=a^{-3}[1-\nabla_q\cdot\boldsymbol\psi]d^3r+O(\psi^2),\qquad \delta=-\nabla_q\cdot\boldsymbol\psi.}
$$

For the perturbed field the [Poisson equation](../../../../../../poisson-equation.md) must be $\nabla_r^2\Phi=4\pi G\rho=4\pi G\bar\rho(1+\delta)$. The displayed background-only right-hand side in the PDF would give no clumping force; it is the background equation, not the full perturbed equation.

Write $\Phi=\Phi_b+\varphi$, where $\nabla_r\Phi_b=(4\pi G/3)\bar\rho\,\mathbf r$. To linear order,

$$
\nabla_q^2\varphi=4\pi G\bar\rho a^2\delta=-4\pi G\bar\rho a^2\nabla_q\cdot\boldsymbol\psi.
$$

For the longitudinal, curl-free displacement used in the growing Zel'dovich mode, this integrates to $\nabla_q\varphi=-4\pi G\bar\rho a^2\boldsymbol\psi$, after removing external homogeneous harmonic fields. More generally the force involves only the longitudinal part $\boldsymbol\psi_\parallel$, which has the same divergence as $\boldsymbol\psi$.

Differentiate $\mathbf r=a(\mathbf q+\boldsymbol\psi)$ twice at fixed $\mathbf q$ and substitute $\ddot{\mathbf r}=-\nabla_r\Phi$. The terms proportional to $\mathbf q+\boldsymbol\psi$ cancel using $\ddot a=-(4\pi G/3)\bar\rho a$, leaving

$$
\ddot{\boldsymbol\psi}+2\frac{\dot a}{a}\dot{\boldsymbol\psi}=4\pi G\bar\rho\boldsymbol\psi_\parallel.
$$

For a longitudinal displacement the right side is $4\pi G\bar\rho\boldsymbol\psi$. Taking minus the comoving divergence gives the general scalar [density contrast](../../../../../../density-contrast.md) equation

$$
\boxed{\ddot\delta+2\frac{\dot a}{a}\dot\delta-4\pi G\bar\rho\delta=0.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [15E](../../15e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
