<h1 id="1/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [Gaussian integral](../../../../../../gaussian-integral.md) over the full vertical [velocity](../../../../../../velocity.md) line is $\sqrt{2\pi}\sigma_z$. Thus the [mass density](../../../../../../density.md) of the [self-gravitating isothermal slab](../../../../../../self-gravitating-isothermal-slab.md) is

$$
\rho(z)=\int_{-\infty}^{\infty}f\,dv_z=\rho_0e^{-\Phi(z)/\sigma_z^2}.
$$

Neglecting radial derivatives makes the [Poisson equation for Newtonian gravity](../../../../../../poisson-equation-for-newtonian-gravity.md) $\Phi_{zz}=4\pi G\rho(z)$. Substituting $\Phi=\sigma_z^2\phi$ and $z=z_0\zeta$, with $z_0^2=\sigma_z^2/(8\pi G\rho_0)$, gives

$$
\boxed{2\phi''=e^{-\phi}.}
$$

Multiply by $\phi'$ and integrate. The central value and [symmetry](../../../../../../symmetry-physics.md) under $z\mapsto-z$ fix the [constant of integration](../../../../../../constant-of-integration.md):

$$
(\phi')^2=1-e^{-\phi}.
$$

On the positive-$\zeta$ side, [Newtonian gravity](../../../../../../gravitational-acceleration.md) makes $\phi'\geq0$. Put $y=e^{\phi/2}$; then $4(y')^2=y^2-1$ with $y(0)=1$. Integration gives $2\operatorname{arcosh}y=\zeta$, and even reflection supplies the other side. Therefore

$$
\boxed{\phi(\zeta)=2\log\cosh(\zeta/2),\qquad \rho(z)=\rho_0\operatorname{sech}^2\!\left(\frac{z}{2z_0}\right).}
$$

Direct [differentiation](../../../../../../differentiation.md) verifies both the equation and central conditions. Uniqueness of the smooth [initial value problem](../../../../../../initial-value-problem.md) rules out other branches meeting those conditions. The [surface density](../../../../../../surface-density-of-a-disk.md) is $4\rho_0z_0$, and the conventional slab [scale height](../../../../../../scale-height.md) is $2z_0$; the factor of two is only a definition of the length scale.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [1](../../1.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
