<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use [relative energy](../../../../../../relative-energy.md) $E=\psi-v^2/2$, with $\psi=-\phi$. If the [galactic distribution function](../../../../../../galactic-distribution-function.md) depends on $E$ alone, rotations and sign reversals in [velocity](../../../../../../velocity.md) space leave it unchanged. Thus all mean [velocities](../../../../../../velocity.md) vanish, and the three component second moments are equal. The anisotropy term in the [Spherical Jeans equation](../../../../../../spherical-jeans-equation.md) cancels. With constant radial [velocity dispersion](../../../../../../velocity-dispersion.md) $\sigma_0$, it reduces to

$$
\sigma_0^2\frac{d\rho}{dr}=-\rho\frac{d\phi}{dr}=\rho\frac{d\psi}{dr}.
$$

Integration gives the [isothermal collisionless tracer](../../../../../../isothermal-collisionless-tracer.md) density

$$
\boxed{\rho(r)=\rho_0\exp\!\left(\frac{\psi(r)}{\sigma_0^2}\right).}
$$

The constant $\rho_0$ changes if a constant is added to the potential; this has no effect on the [velocity](../../../../../../velocity.md) distribution.

Apply the given [untruncated Eddington inversion](../../../../../../untruncated-eddington-inversion.md), retaining its lower limit $-\infty$. Define its integral before differentiation by $I(E)$. With $\psi=E-\sigma_0^2s^2$, the [Gaussian integral](../../../../../../gaussian-integral.md) gives

$$
\begin{aligned}
I(E)&=\int_{-\infty}^E\frac{d\rho}{d\psi}\frac{d\psi}{\sqrt{E-\psi}}\\
&=\frac{2\rho_0}{\sigma_0}e^{E/\sigma_0^2}\int_0^\infty e^{-s^2}\,ds
=\frac{\rho_0\sqrt\pi}{\sigma_0}e^{E/\sigma_0^2}.
\end{aligned}
$$

Differentiating and multiplying by $1/(\sqrt8\,\pi^2)$ yields

$$
\boxed{f(E)=\frac{\rho_0}{(2\pi\sigma_0^2)^{3/2}}e^{E/\sigma_0^2}.}
$$

Indeed, at a fixed position this is

$$
f(\boldsymbol r,\boldsymbol v)=\frac{\rho(\boldsymbol r)}{(2\pi\sigma_0^2)^{3/2}}
\exp\!\left(-\frac{v^2}{2\sigma_0^2}\right),
$$

whose integral over all [velocities](../../../../../../velocity.md) is $\rho$ and whose component second moments are $\sigma_0^2$. This checks both the normalization and the [velocity dispersion](../../../../../../velocity-dispersion.md).

Let $w$ be the [line of sight](../../../../../../line-of-sight.md) component of [velocity](../../../../../../velocity.md). Integrate this [Maxwell-Boltzmann velocity distribution](../../../../../../maxwell-boltzmann-velocity-distribution.md) over the two transverse components:

$$
\int_{\mathbb R^2} f(\boldsymbol r,\boldsymbol v)\,d^2v_\perp
=\frac{\rho(\boldsymbol r)}{\sqrt{2\pi}\sigma_0}e^{-w^2/(2\sigma_0^2)}.
$$

At projected radius $R$, integrating along the [line of sight](../../../../../../line-of-sight.md) simply replaces $\rho$ by the projected [surface density](../../../../../../surface-density-of-a-disk.md) $\Sigma(R)$. Dividing by $\Sigma(R)$ gives the spectroscopist's normalized [Gaussian line-of-sight velocity distribution](../../../../../../gaussian-line-of-sight-velocity-distribution.md):

$$
\boxed{p(w\mid R)=\frac1{\sqrt{2\pi}\sigma_0}e^{-w^2/(2\sigma_0^2)}.}
$$

It is a zero-mean [normal distribution](../../../../../../normal-distribution.md) with width $\sigma_0$, independent of projected radius. This is the untruncated model specified by the lower limit in the inversion formula: no escape-energy cutoff has been imposed. A population restricted to positive binding energy would have truncated velocity tails and would not obey this exact Gaussian density law in a finite escape potential.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
