<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $p(r)=\rho(r)\sigma_r^2(r)$ and use the [velocity-anisotropy parameter](../../../../../../velocity-anisotropy-parameter.md) $\beta=1-\sigma_\theta^2/\sigma_r^2$, with $\sigma_\theta^2=\sigma_\phi^2$. Here the tangential variance is per component; a definition using the sum of both tangential variances instead has an extra factor of two. The original PDF has this correct per-component ratio, which the TeX corrupts.

At a point along the [line of sight](../../../../../../line-of-sight.md), $r^2=R^2+z^2$. The radial direction makes an angle with the sightline satisfying $\sin^2\chi=R^2/r^2$. [Spherical symmetry](../../../../../../spherical-symmetry.md) eliminates mixed moments, and projection gives

$$
\overline{v_{\rm los}^2}=\sigma_r^2\cos^2\chi+\sigma_\theta^2\sin^2\chi=\sigma_r^2\left(1-\beta\frac{R^2}{r^2}\right).
$$

Using both sides of the [galaxy](../../../../../../galaxy-split.md) and $dz=r\,dr/\sqrt{r^2-R^2}$,

$$
I(R)\sigma_p^2(R)=2\int_R^\infty\left(1-\beta\frac{R^2}{r^2}\right)p(r)\frac{r\,dr}{\sqrt{r^2-R^2}}.
$$

For this formula use $I$ as the projected density of the same tracer represented by $\rho$. If $\rho$ is a [mass density](../../../../../../density.md) and $I$ an observed [surface brightness](../../../../../../surface-brightness.md), a constant [mass-to-light ratio](../../../../../../mass-to-light-ratio.md) rescales $I$ by that factor; otherwise replace $\rho$ by the [luminosity density](../../../../../../luminosity-density.md) throughout the tracer equation. The gravitating $M(r)$ remains the total [mass](../../../../../../mass.md), not necessarily the tracer's [mass](../../../../../../mass.md).

The [Spherical Jeans equation](../../../../../../spherical-jeans-equation.md) is $p'+2\beta p/r=-\rho GM/r^2$. Eliminate $\beta p=-r[p'+\rho GM/r^2]/2$ from the projected integrand:

$$
2\left(1-\beta\frac{R^2}{r^2}\right)p=2p+\frac{R^2}{r}p'+\frac{R^2\rho GM}{r^3}.
$$

Rearranging proves

$$
\boxed{I\sigma_p^2-R^2\int_R^\infty\frac{\rho GM(r)}{r^2\sqrt{r^2-R^2}}\,dr=\int_R^\infty\left(2p+\frac{R^2}{r}p'\right)\frac{r\,dr}{\sqrt{r^2-R^2}}.}
$$

No constancy of $\beta$ was needed. Convergence of the projected moments and the steady spherical assumptions are required. This is the integral form of the [projected spherical Jeans residual](../../../../../../projected-spherical-jeans-residual.md).

Although $\beta$ has disappeared explicitly, the unknown radial pressure $p$ still carries the orbital information. Thus the identity does not remove the [mass--anisotropy--density degeneracy](../../../../../../mass-anisotropy-density-degeneracy.md): projected brightness and one projected [second moment](../../../../../../second-moment.md) do not uniquely determine both $M(r)$ and the radial/tangential partition. A central rise in [velocity dispersion](../../../../../../velocity-dispersion.md) can reflect a compact central [mass](../../../../../../mass.md), radial orbital bias, or a changing [mass-to-light ratio](../../../../../../mass-to-light-ratio.md); flattening and departures from equilibrium add further ambiguities.

For example, within a point-mass-dominated region with tracer $\rho\propto r^{-k}$ and constant $\beta$, direct solution gives $\sigma_r^2=GM_\bullet/[(k+1-2\beta)r]$. For $k>1$ the [projected velocity dispersion of a Keplerian cusp](../../../../../../projected-velocity-dispersion-of-a-keplerian-cusp.md) is

$$
\sigma_p^2(R)=\frac{GM_\bullet}{(k+1-2\beta)R}\frac{B(k/2,1/2)}{B((k-1)/2,1/2)}\left(1-\frac{\beta k}{k+1}\right).
$$

The [beta function](../../../../../../beta-function.md) factors come from setting $r=R\sec\chi$ in the integrals along the [line of sight](../../../../../../line-of-sight.md). Different allowed $\beta$ generally change the [mass](../../../../../../mass.md) needed to fit the same normalization; $k=2$ is a special cancellation, not the general case. Resolving the central [black-hole sphere of influence](../../../../../../black-hole-sphere-of-influence.md) and constraining orbital structure with higher [velocity](../../../../../../velocity.md) moments or additional kinematic directions strengthens a compact-mass inference. **Brightness and [velocity dispersion](../../../../../../velocity-dispersion.md) profiles alone do not establish a unique central black-hole [mass](../../../../../../mass.md), still less an [event horizon](../../../../../../event-horizon.md).**

## ↑ Ancestors (11)

1. [B](../b.md)
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
