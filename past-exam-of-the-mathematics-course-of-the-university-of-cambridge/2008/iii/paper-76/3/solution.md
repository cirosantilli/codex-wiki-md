<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Put $\lambda=(r/a)^2$, so the inverted observation point is $\overline{\mathbf r}=\mathbf r/\lambda$ and $\overline r=r/\lambda$. Let $\mathbf R=\overline{\mathbf r}-\mathbf r_0$. The [Kelvin transform](../../../../../kelvin-transform.md) correction in the first bracket is transformed using

$$
\mathbf R=\lambda^{-1}(\mathbf r-\lambda\mathbf r_0),
\qquad R=\lambda^{-1}|\mathbf r-\lambda\mathbf r_0|,
\qquad \frac{\overline r}{a}=\lambda^{-1/2}.
$$

Thus its dipole contribution is exactly

$$
\frac{1}{4\pi\sigma}\mathbf Q\cdot
\frac{\overline r}{a}\frac{\mathbf R}{R^3}
=\lambda^{3/2}\Psi(\mathbf r;\lambda\mathbf r_0).
$$

For the remaining correction use the [dipole line-integral identity](../../../../../dipole-line-integral-identity.md). Writing $\mathbf P_c=\mathbf r-c\mathbf r_0$ and $P_c=|\mathbf P_c|$, it is

$$
\int_0^c\frac{\mathbf r-t\mathbf r_0}{|\mathbf r-t\mathbf r_0|^3}\,dt
=\frac{c(P_c\mathbf r+r\mathbf P_c)}{rP_c(rP_c+\mathbf r\cdot\mathbf P_c)}.
$$

It can be proved by differentiating the right side with respect to $c$ and checking its zero value at $c=0$. Alternatively resolve into directions parallel and perpendicular to $\mathbf r_0=b\mathbf e$: if $\mathbf r=\rho\mathbf e_\rho+z\mathbf e$, the two integrals are $(z/r-(z-bc)/P_c)/(b\rho)$ and $(1/P_c-1/r)/b$, respectively, which combine to the displayed expression. The limiting cases follow by continuity.

Set $c=\lambda$. Then $\mathbf P_c=\lambda\mathbf R$, $P_c=\lambda R$, $\mathbf r=\lambda\overline{\mathbf r}$ and $r=\lambda\overline r$. Substitution gives

$$
\sqrt\lambda\int_0^\lambda
\frac{\mathbf r-t\mathbf r_0}{|\mathbf r-t\mathbf r_0|^3}\,dt
=\frac{R\overline{\mathbf r}+\overline r\mathbf R}
{aR(\overline rR+\overline{\mathbf r}\cdot\mathbf R)}.
$$

Dotting with $\mathbf Q/(4\pi\sigma)$ reproduces the second correction. Including the primary dipole therefore proves the [Spherical Neumann dipole images](../../../../../spherical-neumann-dipole-images.md) representation,

$$
\boxed{u^-(\mathbf r)=\Psi(\mathbf r;\mathbf r_0)
+\left(\frac ra\right)^3\Psi\!\left(\mathbf r;\left(\frac ra\right)^2\mathbf r_0\right)
+\frac ra\int_0^{(r/a)^2}\Psi(\mathbf r;t\mathbf r_0)\,dt.}
$$

The upper limit is $(r/a)^2$ in the PDF; extracting the small stacked fraction as text can incorrectly invert it. The extra terms are one scaled dipole and a continuous dipole line in this parametrized [method of images](../../../../../method-of-images.md). Their positions and strengths depend on the observation radius, so they should not be treated as a fixed set of independent physical sources. For an interior point $r<a$, the entire image segment satisfies $t|\mathbf r_0|\leq(r/a)^2|\mathbf r_0|<r$, so it introduces no new interior singularity. The only physical interior dipole singularity remains at $\mathbf r_0$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 76](../../paper-76-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
