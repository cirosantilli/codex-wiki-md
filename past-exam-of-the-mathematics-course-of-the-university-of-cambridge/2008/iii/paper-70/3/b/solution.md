<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Outside the thin burning shell, the enclosed mass and luminosity are approximately $M_c$ and $L$. Divide the [hydrostatic pressure support equation](../../../../../../hydrostatic-pressure-support-equation.md) by [radiative diffusion in a star](../../../../../../radiative-diffusion-in-a-star.md) with constant opacity:

$$
\frac{dP}{dT}=\frac{16\pi acGM_c}{3\kappa_0L}T^3.
$$

In the [constant-opacity radiative-zero giant envelope](../../../../../../constant-opacity-radiative-zero-giant-envelope.md) approximation, the outer pressure and temperature constants are negligible. Integration gives

$$
\boxed{P=\Lambda T^4,\qquad
\Lambda=\frac{4\pi acGM_c}{3\kappa_0L}.}
$$

The [radiation pressure](../../../../../../radiation-pressure.md) is $aT^4/3$, so the [gas pressure](../../../../../../gas-pressure.md) fraction $\beta$ is constant and satisfies $(1-\beta)\Lambda=a/3$. Thus also

$$
\boxed{\Lambda=\frac{a}{3(1-\beta)},\qquad
\beta=1-\frac{\kappa_0L}{4\pi cGM_c}.}
$$

The physical branch has positive gas pressure, hence $L<4\pi cGM_c/\kappa_0$, the constant-opacity [Eddington luminosity](../../../../../../eddington-luminosity.md) for the core mass.

Using the gas part of the [equation of state](../../../../../../equation-of-state.md), define $H=\mu\beta\Lambda/\mathcal R$, so $\rho=HT^3$. Substitution into hydrostatic balance gives

$$
4\Lambda T^3\frac{dT}{dr}
=-\frac{GM_c}{r^2}\frac{\mu\beta\Lambda}{\mathcal R}T^3,
\qquad
\frac{dT}{dr}=-\frac{\mu\beta GM_c}{4\mathcal Rr^2}.
$$

Consequently, in the same deep-envelope radiative-zero approximation,

$$
\boxed{T(r)=\frac{\mu\beta GM_c}{4\mathcal Rr}.}
$$

Precisely, a finite outer matching point $(R_s,T_s)$ gives $T=T_s+\mu\beta GM_c(1/r-1/R_s)/(4\mathcal R)$. The displayed $1/r$ profile neglects that additive outer-boundary constant; it is appropriate near a compact core when the envelope extends to much smaller temperatures.

To estimate the thin-shell luminosity, write $K_T=\mu\beta GM_c/(4\mathcal R)$, so $T=K_T/r$. The hydrogen-layer heating law gives

$$
\frac{dL_r}{dr}=4\pi r^2\rho\epsilon
=4\pi\epsilon_0H^2r^2T^{22}
=4\pi\epsilon_0H^2K_T^{22}r^{-20}.
$$

This steep radial dependence strongly concentrates the emission near $R_c$. Continuing the outer profile across the thin emitting layer and taking a distant upper limit gives

$$
L\simeq\frac{4\pi\epsilon_0}{19}H^2K_T^{22}R_c^{-19}.
$$

The same radiative coefficient implies $H=16\pi acK_T/(3\kappa_0L)$. Hence the [high-power shell burning in a constant-opacity giant envelope](../../../../../../high-power-shell-burning-in-a-constant-opacity-giant-envelope.md) satisfies

$$
L^3=\frac{4\pi\epsilon_0}{19}
\left(\frac{16\pi ac}{3\kappa_0}\right)^2K_T^{24}R_c^{-19}.
$$

Taking the cube root gives the requested form,

$$
\boxed{L=C\frac{(\mu\beta M_c)^8}{R_c^{19/3}},\qquad
C=\left(\frac G{4\mathcal R}\right)^8
\left[\frac{4\pi\epsilon_0}{19}
\left(\frac{16\pi ac}{3\kappa_0}\right)^2\right]^{1/3}.}
$$

Thus $C$ contains only the specified opacity and heating normalizations and physical constants. The explicit coefficient uses the outer radiative profile as a thin-shell estimate; resolving the variation of $L_r$ within the emitting layer can change that coefficient. Also $\beta$ depends on $L$, so the radiation-pressure-inclusive relation is implicit, not a pure explicit eighth-power core-mass law with independently fixed $\beta$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
