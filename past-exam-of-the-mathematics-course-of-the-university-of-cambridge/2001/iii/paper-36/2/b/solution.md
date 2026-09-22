<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An explicit example avoids an unspecified [correlation time](../../../../../../correlation-time.md). For each coordinate axis $\mathbf e_j$, choose transverse unit vectors $\mathbf a_j,\mathbf b_j$ with $\mathbf e_j\times\mathbf a_j=\mathbf b_j$, and take the three real [circular polarizations](../../../../../../circular-polarization.md)

$$
\mathbf u_j=U(\mathbf a_j\cos\phi_j-\sigma\mathbf b_j\sin\phi_j),\qquad \phi_j=kx_j-\Omega t,\qquad \sigma=\pm1.
$$

The propagation directions are mutually perpendicular and all three waves have the same handedness. Direct differentiation gives

$$
\nabla\times\mathbf u_j=\sigma k\mathbf u_j,\qquad \nabla^2\mathbf u_j=-k^2\mathbf u_j,\qquad \mathbf u_j\times\partial_{\phi_j}\mathbf u_j=-\sigma U^2\mathbf e_j.
$$

A spatial average over the periodic cell removes cross terms between different waves. Hence the mean [kinetic helicity](../../../../../../hydrodynamical-helicity.md) of their sum is

$$
\mathcal H=\langle\mathbf u\cdot\nabla\times\mathbf u\rangle=3\sigma kU^2.
$$

The sum has isotropic second moments, $\langle u_i u_j\rangle=U^2\delta_{ij}$.

For a locally uniform test [magnetic field](../../../../../../magnetic-field.md) $\overline{\mathbf B}$, the periodic [first-order smoothing](../../../../../../first-order-smoothing-approximation.md) response obeys

$$
(\partial_t-\eta\nabla^2)\mathbf b_j=k\overline B_j\partial_{\phi_j}\mathbf u_j.
$$

Set $a=\eta k^2>0$. Since $\partial_t=-\Omega\partial_\phi$ and $\partial_\phi^2\mathbf u_j=-\mathbf u_j$, direct substitution gives the response after transients decay:

$$
\mathbf b_j=\frac{k\overline B_j}{a^2+\Omega^2}(a\partial_{\phi_j}\mathbf u_j-\Omega\mathbf u_j).
$$

The term proportional to $\mathbf u_j$ contributes no [cross product](../../../../../../cross-product.md) with that same wave. Cross terms between distinct waves average to zero. Therefore

$$
\boldsymbol{\mathcal E}=\sum_j\langle\mathbf u_j\times\mathbf b_j\rangle=-\frac{\sigma kU^2a}{a^2+\Omega^2}\overline{\mathbf B},
$$

and the [isotropic alpha effect of three helical traveling waves](../../../../../../isotropic-alpha-effect-of-three-helical-traveling-waves.md) is

$$
\boxed{\alpha=-\frac{a}{3(a^2+\Omega^2)}\mathcal H,\qquad a=\eta k^2.}
$$

This is the alpha-helicity relation with the exact response time $\tau_{\rm eff}=a/(a^2+\Omega^2)$ for these monochromatic waves. In the quasistatic limit $\Omega=0$, $\alpha=-\mathcal H/(3\eta k^2)$. A single wave would give an anisotropic response along its propagation direction; the three equal waves make the response tensor a scalar multiple of the identity. The calculation retains the validity assumptions of [first-order smoothing](../../../../../../first-order-smoothing-approximation.md), rather than extrapolating the formula to arbitrary fluctuation amplitude.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
