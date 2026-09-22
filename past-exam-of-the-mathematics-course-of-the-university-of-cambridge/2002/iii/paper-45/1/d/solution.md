<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

[Type Ia supernovae](../../../../../../type-ia-supernova.md) have similar peak luminosities that can be standardized using their light-curve width and color, rather than assumed to be identical without correction. Their redshifts and corrected [apparent magnitudes](../../../../../../apparent-magnitude.md) give a [distance modulus](../../../../../../distance-modulus.md),

$$
\mu=m-M=5\log_{10}\left(\frac{d_L}{10\,\mathrm{pc}}\right).
$$

Compare this [Hubble diagram](../../../../../../hubble-diagram.md) with the luminosity-distance prediction of a background cosmology. Restoring $c$, put $E(z)=H(z)/H_0$, $I(z)=\int_0^z dz'/E(z')$ and define $\mathcal S_{\Omega_k}(I)$ as $\sinh(\sqrt{\Omega_k}I)/\sqrt{\Omega_k}$ for $\Omega_k>0$, $I$ for $\Omega_k=0$, and $\sin(\sqrt{-\Omega_k}I)/\sqrt{-\Omega_k}$ for $\Omega_k<0$. Then

$$
d_L(z)=\frac{c(1+z)}{H_0}\mathcal S_{\Omega_k}(I(z)).
$$

Neglecting radiation at these redshifts, [Friedmann equations](../../../../../../friedmann-equations.md) and a separately conserved [dark energy](../../../../../../dark-energy.md) component with $w(z)=p/(\rho c^2)$ give

$$
E^2(z)=\Omega_{m0}(1+z)^3+\Omega_{k0}(1+z)^2
+\Omega_{{\rm de},0}\exp\left[3\int_0^z\frac{1+w(z')}{1+z'}\,dz'\right].
$$

For constant $w$, the last factor is $(1+z)^{3(1+w)}$; a [cosmological constant](../../../../../../cosmological-constant.md) has $w=-1$. Thus the redshift dependence of the measured distance constrains matter density, curvature and the dark-energy [equation of state](../../../../../../equation-of-state.md). At small redshift, $d_L=(cz/H_0)[1+(1-q_0)z/2+\cdots]$, showing how departures from the linear Hubble law probe the [deceleration parameter](../../../../../../deceleration-parameter.md).

The early distant-supernova analyses found larger distances than matter-only decelerating models predicted, providing evidence for accelerated expansion; see [the 1998 supernova analysis](https://arxiv.org/abs/astro-ph/9805201) and [the 1999 independent supernova analysis](https://arxiv.org/abs/astro-ph/9812133). This is a statement about the distance-redshift curve under the standardization and cosmological assumptions, not a direct measurement of a fluid pressure.

The [absolute magnitude–Hubble constant degeneracy](../../../../../../absolute-magnitude-hubble-constant-degeneracy.md) means uncalibrated supernovae constrain the shape of $d_L(z)$ without separately determining $H_0$ and the common absolute luminosity. The integral over $H(z)$ also makes different matter, curvature and $w(z)$ histories partly degenerate. Wide redshift coverage and independent [cosmic microwave background](../../../../../../cosmic-microwave-background.md) and [large-scale structure of the universe](../../../../../../large-scale-structure-of-the-universe-split.md) information help break these degeneracies. Dust extinction, source evolution, photometric calibration, sample selection and [K corrections](../../../../../../k-correction.md) must be modeled, and constraints on a time-dependent equation of state depend on how that function is parameterized. **Standardized supernovae test the expansion history; they do not by themselves uniquely determine every cosmological parameter.**

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
