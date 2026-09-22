<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume a steady, locally plane-symmetric [galactic disk](../../../../../../galactic-disk.md), with negligible radial tilt term in the [vertical Jeans equation](../../../../../../vertical-jeans-equation.md). Write $\rho(z)$ for the stellar [mass density](../../../../../../density.md), and $K_z=\partial_z\Phi$ for the upward gradient of the [Newtonian gravitational potential](../../../../../../newtonian-gravitational-potential.md); the actual vertical [gravitational acceleration](../../../../../../gravitational-acceleration.md) is $-K_z$. Constant vertical [velocity dispersion](../../../../../../velocity-dispersion.md) gives

$$
\sigma^2\frac{d\rho}{dz}=-\rho K_z,\qquad
\rho(z)=\rho(0)\exp\left[-\frac{\Phi(z)-\Phi(0)}{\sigma^2}\right].
$$

Integrating the plane-parallel [Poisson equation for Newtonian gravity](../../../../../../poisson-equation-for-newtonian-gravity.md) from the symmetry plane gives $K_z(z)=4\pi G\int_0^z\rho(z')\,dz'$. Outside most of the mass, this tends to $2\pi G\Sigma$ for $z>0$, where the [surface density](../../../../../../surface-density-of-a-disk.md) includes both sides of the [galactic disk](../../../../../../galactic-disk.md). Treating this field as constant and integrating the [vertical Jeans equation](../../../../../../vertical-jeans-equation.md) yields

$$
\rho(z)\propto e^{-|z|/h},\qquad
\boxed{h=\frac{\sigma^2}{2\pi G\Sigma}}.
$$

**This exponential is the thin-sheet approximation or the outer tail, not the exact profile at every height.** To see the distinction without an additional assumption, set $\rho=\rho_0e^{-u}$ with $u=(\Phi-\Phi(0))/\sigma^2$. The [Poisson equation for Newtonian gravity](../../../../../../poisson-equation-for-newtonian-gravity.md) becomes $u''=(4\pi G\rho_0/\sigma^2)e^{-u}$, with $u(0)=u'(0)=0$, and is solved by

$$
u=2\log\cosh(z/z_0),\qquad
\rho=\rho_0\operatorname{sech}^2(z/z_0),\qquad
z_0^2=\frac{\sigma^2}{2\pi G\rho_0}.
$$

Since $\Sigma=2\rho_0z_0$, the exact [self-gravitating isothermal slab](../../../../../../self-gravitating-isothermal-slab.md) has $z_0=\sigma^2/(\pi G\Sigma)$. At large $|z|/z_0$, $\operatorname{sech}^2(z/z_0)\sim4e^{-2|z|/z_0}$, recovering precisely the boxed [scale height](../../../../../../scale-height.md); near the plane its slope vanishes, whereas an exponential has a cusp.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
