<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [singular isothermal sphere](../../../../../../singular-isothermal-sphere.md) has one-dimensional [velocity dispersion](../../../../../../velocity-dispersion.md) $\sigma$, density $\rho_{\rm tot}(r)=\sigma^2/(2\pi Gr^2)$, and enclosed mass $M(<R)=2\sigma^2R/G$. The gas mass inside $R$ is therefore

$$
M_g(<R)=\frac{2f_{\rm gas}\sigma^2R}{G}.
$$

Taking the dynamical crossing time to be $t_{\rm dyn}\simeq R/\sigma$, the [dynamical upper bound on black-hole fuelling](../../../../../../dynamical-upper-bound-on-black-hole-fuelling.md) is

$$
\boxed{\dot M_{\rm dyn}\sim\frac{M_g(<R)}{t_{\rm dyn}}
=\frac{2f_{\rm gas}\sigma^3}{G}.}
$$

The cancellation of $R$ is special to the [singular isothermal sphere](../../../../../../singular-isothermal-sphere.md). At $\sigma=200\,\mathrm{km\,s^{-1}}$, this is approximately

$$
\dot M_{\rm dyn}\simeq3.8\times10^3f_{\rm gas}\,M_\odot\,\mathrm{yr^{-1}}
\simeq6.1\times10^2\left(\frac{f_{\rm gas}}{0.16}\right)M_\odot\,\mathrm{yr^{-1}}.
$$

Use the stated [M-sigma relation](../../../../../../m-sigma-relation.md) to set $M_{\rm BH}\simeq3\times10^8M_\odot$. Defining the [Eddington accretion rate](../../../../../../eddington-accretion-rate.md) with a reference [radiative efficiency of black-hole accretion](../../../../../../radiative-efficiency-of-black-hole-accretion.md) $\eta_0$,

$$
\dot M_{\rm Edd}=\frac{L_{\rm Edd,es}}{\eta_0c^2}
=\frac{4\pi GM_{\rm BH}}{\eta_0\kappa_{\rm es}c}
\simeq6.6\left(\frac{\eta_0}{0.1}\right)^{-1}
\left(\frac{\kappa_{\rm es}}{0.40\,\mathrm{cm^2\,g^{-1}}}\right)^{-1}
M_\odot\,\mathrm{yr^{-1}}.
$$

Combining this with $M_{\rm BH}\propto\sigma^4$ gives

$$
\boxed{\frac{\dot M_{\rm dyn}}{\dot M_{\rm Edd}}
\simeq92\left(\frac{f_{\rm gas}}{0.16}\right)
\left(\frac{\eta_0}{0.1}\right)
\left(\frac{\kappa_{\rm es}}{0.40\,\mathrm{cm^2\,g^{-1}}}\right)
\left(\frac{\sigma}{200\,\mathrm{km\,s^{-1}}}\right)^{-1}.}
$$

Thus a gas fraction of order $0.1$--$0.16$ and the usual $\eta_0=0.1$ give roughly $60$--$90$ times the [Eddington accretion rate](../../../../../../eddington-accretion-rate.md), below $100$ at the requested dispersion. Using a crossing time $R/(\sqrt2\sigma)$ instead changes the coefficient by $\sqrt2$, so this is an order-of-magnitude estimate rather than a sharp universal bound. The problem does not specify $f_{\rm gas}$ or the rate convention: without these choices, the numerical claim cannot be proved for every gas fraction. Defining the rate as $L_{\rm Edd}/c^2$ would make this ratio ten times larger.

This is extremely optimistic because it gives every gas element a direct path to the hole on a crossing time. In a real [galaxy](../../../../../../galaxy-split.md), gas must shed [angular momentum](../../../../../../angular-momentum.md), avoid conversion into stars through [star formation](../../../../../../star-formation.md), cool sufficiently to flow inward, and survive [active-galactic-nucleus feedback](../../../../../../active-galactic-nucleus-feedback.md). A rotating [accretion disk](../../../../../../accretion-disk.md) generally transports material on a [viscous timescale](../../../../../../viscous-timescale.md), much longer than the orbital crossing time. Most available gas need not reach the central hole. If the hole is supplied at approximately the [Eddington accretion rate](../../../../../../eddington-accretion-rate.md), only about one percent of this optimistic dynamical supply reaches it; the actual percentage depends on its luminosity and duty cycle, so the bound alone is not a measurement of the fuelling efficiency.

For the temperature jump, use [Bondi accretion](../../../../../../bondi-accretion.md) as the local hot-gas estimate:

$$
\dot M_B\propto\rho_\infty c_s^{-3}.
$$

Assuming the initial gas had $c_s\sim\sigma$, its density has not yet changed, and its polytropic coefficient remains comparable, heating to $c_{s,\rm feed}\sim10\sigma$ gives

$$
\boxed{\frac{\dot M_{B,\rm feed}}{\dot M_{B,\rm before}}\sim10^{-3}.}
$$

The capture radius $GM_{\rm BH}/c_s^2$ also shrinks by about $100$. Subsequent expansion can lower the density and suppress the [mass accretion rate](../../../../../../mass-accretion-rate.md) further. The result illustrates [thermal suppression of black-hole accretion](../../../../../../thermal-suppression-of-black-hole-accretion.md) and negative [active-galactic-nucleus feedback](../../../../../../active-galactic-nucleus-feedback.md): vigorous activity can shut off its own gas supply. The factor $10^{-3}$ is conditional on the fixed-density comparison; the previous dynamical upper bound is not itself an actual pre-heating Bondi rate.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 347](../../../paper-347-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
