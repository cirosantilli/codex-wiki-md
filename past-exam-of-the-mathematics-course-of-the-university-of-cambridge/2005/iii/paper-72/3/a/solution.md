<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Interpret the barred [velocities](../../../../../../velocity.md) as [second moments](../../../../../../second-moment.md) of a steady nonstreaming [collisionless stellar system](../../../../../../collisionless-stellar-system.md), and write $\sigma_r^2=\overline{v_r^2}$. In an isotropic model the three component dispersions agree, so the [Spherical Jeans equation](../../../../../../spherical-jeans-equation.md) becomes

$$
\frac{d(\rho\sigma_r^2)}{dr}=-\frac{\rho GM(r)}{r^2}.
$$

Put $A=\rho_0r_0^k$, so $\rho=Ar^{-k}$. If this density supplies all of the [Newtonian gravity](../../../../../../gravitational-acceleration.md) and there is no central point [mass](../../../../../../mass.md), finite enclosed [mass](../../../../../../mass.md) requires $k<3$ and

$$
M(r)=\frac{4\pi A}{3-k}r^{3-k}.
$$

Integrate to an outer radius $b$ at which the pressure is $P_b=\rho(b)\sigma_r^2(b)$. The exact Jeans-moment solution within the power-law region is

$$
\rho\sigma_r^2=P_b+\frac{4\pi GA^2}{3-k}\int_r^b s^{1-2k}\,ds,
$$

and, for $k\ne1$,

$$
\boxed{\sigma_r^2(r)=\frac{P_b}{A}r^k+\frac{2\pi GA}{(3-k)(1-k)}r^k\left(b^{2-2k}-r^{2-2k}\right).}
$$

For $k<1$ and $r\ll b$, the integral is dominated by outer radii. Therefore

$$
\boxed{\sigma_r^2\sim Cr^k,\quad C=\frac{P_b}{A}+\frac{2\pi GA}{(3-k)(1-k)}b^{2-2k}.}
$$

The coefficient cannot be determined from the local density cusp alone. Extending the power law to infinity gives a divergent pressure integral when $k<1$, so an outer scale or boundary condition is essential. For the usual shallow cusp $0<k<1$, the central [velocity dispersion](../../../../../../velocity-dispersion.md) tends to zero even though the density diverges.

For $1<k<3$, inner radii dominate as $r/b\to0$; equivalently one can send $b\to\infty$ with vanishing boundary pressure to obtain

$$
\boxed{\sigma_r^2\sim\frac{2\pi G\rho_0r_0^k}{(3-k)(k-1)}r^{2-k}=\frac{V_c^2(r)}{2(k-1)}.}
$$

Thus the central [velocity dispersion](../../../../../../velocity-dispersion.md) decreases for $1<k<2$, is constant at $k=2$, and diverges for $2<k<3$. At the omitted threshold $k=1$, $\sigma_r^2=(P_b/A)r+2\pi GA r\ln(b/r)$. For $k\geq3$ the assumed central density law has infinite enclosed [mass](../../../../../../mass.md), so the same unmodified model cannot determine a finite [velocity dispersion](../../../../../../velocity-dispersion.md). These boundary and domain restrictions are the [boundary dependence of an isotropic self-gravitating cusp](../../../../../../boundary-dependence-of-an-isotropic-self-gravitating-cusp.md); specifying density without them does not specify a physical finite [galaxy](../../../../../../galaxy-split.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
