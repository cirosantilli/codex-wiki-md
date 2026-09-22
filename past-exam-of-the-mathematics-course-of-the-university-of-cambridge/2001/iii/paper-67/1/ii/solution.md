<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

An isotropic source's [bolometric luminosity](../../../../../../luminosity.md) is distributed over a wavefront of physical area $4\pi a_0^2r^2$. Each [photon](../../../../../../photon.md) loses an [energy](../../../../../../energy.md) factor $(1+z)^{-1}$ through [cosmological redshift](../../../../../../cosmological-redshift.md), and successive [photons](../../../../../../photon.md) arrive with a further rate factor $(1+z)^{-1}$ through [cosmological time dilation](../../../../../../cosmological-time-dilation.md). Therefore the [radiative flux](../../../../../../radiative-flux.md) and [luminosity distance](../../../../../../luminosity-distance.md) are

$$
F=\frac{L}{4\pi a_0^2r^2(1+z)^2},
\qquad d_L=a_0r(1+z),\qquad 1+z=\frac{a_0}{a(t)}.
$$

These are bolometric formulas; a fixed observed [frequency](../../../../../../frequency.md) would require the shifted emission spectrum as well.

Normalize the [scale factor](../../../../../../scale-factor-cosmology.md) by $a_0=1$. Summing the [radiative flux](../../../../../../radiative-flux.md) over the [source counts on an FLRW past light cone](../../../../../../source-counts-on-an-flrw-past-light-cone.md) makes the transverse shell-area factors cancel:

$$
d\mathcal F_0=F\,dN=L n(t)a(t)^4dt,\qquad
\boxed{\mathcal F_0=L\int_0^{t_0}n(t)a(t)^4dt.}
$$

Thus $\mathcal F_0$ is power per effective detector area, summed over the whole sky; an all-sky detector of effective area $A_{\rm det}$ receives $A_{\rm det}\mathcal F_0$. The corresponding intensity per [solid angle](../../../../../../solid-angle.md) is $\mathcal F_0/(4\pi)$. Restoring the speed of light multiplies these flux integrals by $c$.

Spatially uniform $n(t)$ by itself does not specify its time evolution. For a persistent population comoving with the expansion, with neither creation nor destruction, the [cosmological continuity equation](../../../../../../cosmological-continuity-equation.md) for source number is $\dot n+3Hn=0$. Its conserved [comoving number density](../../../../../../comoving-number-density.md) is $n_0=a^3n$, so the [cosmological bolometric background from conserved sources](../../../../../../cosmological-bolometric-background-from-conserved-sources.md) becomes $Ln_0\int a\,dt$. For the [Einstein-de Sitter universe](../../../../../../einstein-de-sitter-universe.md),

$$
\boxed{\mathcal F_{\rm flat}
=Ln_0\int_0^{t_0}\left(\frac{t}{t_0}\right)^{2/3}dt
=\frac35Ln_0t_0=\frac{2Ln_0}{5H_0}.}
$$

The last equality uses $H_0=2/(3t_0)$. The early-time [improper integral](../../../../../../improper-integral.md) converges despite the diverging physical source density. If instead the proper [number density](../../../../../../number-density.md) were maintained at a constant value $n_0$ by continuous source creation, the same geometry would give $3Ln_0t_0/11$. For a completely unspecified source history the general integral above is the determined answer; constancy of individual [luminosity](../../../../../../luminosity.md) alone does not imply number conservation.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
