<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Integrate the reduced vertical [phase-space distribution function](../../../../../phase-space-distribution-function.md) over $v_z$. The Gaussian velocity integral cancels its normalization, giving

$$
\rho(z)=\rho_0 e^{-\Phi(z)/\sigma_z^2}.
$$

Here the constant vertical [velocity dispersion](../../../../../velocity-dispersion.md) is $\sigma_z$, and $\Phi(0)=0$ fixes the potential reference. Neglecting the radial derivatives in the [Poisson equation for Newtonian gravity](../../../../../poisson-equation-for-newtonian-gravity.md) leaves

$$
\frac{d^2\Phi}{dz^2}=4\pi G\rho_0e^{-\Phi/\sigma_z^2}.
$$

With $\phi=\Phi/\sigma_z^2$, $\zeta=z/z_0$ and $z_0^2=\sigma_z^2/(8\pi G\rho_0)$, this becomes

$$
\frac{d^2\phi}{d\zeta^2}=\frac12e^{-\phi}.
$$

Thus the stated dimensionless equation follows with its factor of two.

For a direct solution, multiply by $2\phi'$ and integrate from the midplane. The initial conditions give

$$
(\phi')^2=1-e^{-\phi}.
$$

For $\zeta>0$ take the increasing branch and put $u=e^{\phi/2}$. Then $4(u')^2=u^2-1$, whose smoothly increasing solution consistent with the second-order equation is $u=\cosh(\zeta/2)$. Reflection about the midplane supplies the negative-$\zeta$ branch. Therefore

$$
\boxed{\phi(\zeta)=2\log\cosh(\zeta/2),\qquad
\rho(z)=\rho_0\operatorname{sech}^2\!\left(\frac{z}{2z_0}\right).}
$$

Substitution verifies $2\phi''=\operatorname{sech}^2(\zeta/2)=e^{-\phi}$ and both boundary conditions. The smooth second-order equation has a unique solution for those initial data, so no extra constant branch from the first-integral square root is admissible.

This is the [self-gravitating isothermal slab](../../../../../self-gravitating-isothermal-slab.md). Its scale convention matters: if its profile is instead written $\rho=\rho_0\operatorname{sech}^2(z/H)$, then $H=2z_0=\sigma_z/\sqrt{2\pi G\rho_0}$. Its [surface density](../../../../../surface-density-of-a-disk.md) is $\Sigma=4\rho_0z_0$. The force approaches $|\Phi'|=\sigma_z^2/z_0=2\pi G\Sigma$, consistent with the field of a plane sheet. These checks fix both the scale-height and Poisson factors.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 44](../../paper-44-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
