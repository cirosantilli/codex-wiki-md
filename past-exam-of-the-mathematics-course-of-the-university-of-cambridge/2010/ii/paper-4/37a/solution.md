<h1 id="37a/solution">Solution</h1>

↑ **Parent:** [37A](../37a.md)

For axisymmetric incompressible flow without swirl, the [Stokes streamfunction](../../../../../stokes-streamfunction.md) satisfies

$$
\boxed{u_R=\frac{\Psi_\theta}{R^2\sin\theta},\qquad
u_\theta=-\frac{\Psi_R}{R\sin\theta}.}
$$

Substitution into the divergence in spherical coordinates makes [incompressibility](../../../../../incompressible-flow.md) an identity. Its only [vorticity](../../../../../vorticity.md) component is

$$
\omega_\phi=\frac1R[\partial_R(Ru_\theta)-\partial_\theta u_R]
=-\frac{\mathcal D^2\Psi}{R\sin\theta}.
$$

Taking the curl of the [Stokes equation](../../../../../stokes-equation.md) eliminates pressure and gives $\nabla^2\boldsymbol\omega=0$. For an axisymmetric azimuthal vector, its scalar component obeys $(\Delta-1/(R^2\sin^2\theta))\omega_\phi=0$. Direct differentiation verifies

$$
\left(\Delta-\frac1{R^2\sin^2\theta}\right)
\frac{h}{R\sin\theta}
=\frac{\mathcal D^2h}{R\sin\theta}.
$$

Apply this to $h=\mathcal D^2\Psi$ to obtain

$$
\boxed{\mathcal D^2(\mathcal D^2\Psi)=0.}
$$

## ↑ Ancestors (10)

1. [37A](../37a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
