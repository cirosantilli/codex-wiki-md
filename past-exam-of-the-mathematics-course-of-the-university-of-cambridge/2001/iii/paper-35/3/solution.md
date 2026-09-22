<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [spherical harmonic](../../../../../spherical-harmonic.md) of angular degree $\ell$ has horizontal [wavenumber](../../../../../wavenumber.md) $k_h=L/r$, with $L=\sqrt{\ell(\ell+1)}$. The local acoustic [dispersion relation](../../../../../dispersion-relation.md) therefore gives the radial [wavenumber](../../../../../wavenumber.md)

$$
k_r^2=\omega^2/c^2-L^2/r^2.
$$

In the high-order regime a travelling [stellar acoustic mode](../../../../../stellar-acoustic-mode.md) accumulates phase $\int k_r\,dr$ across its radial cavity. Reflection at the inner turning point and at the near-surface boundary fixes additional phases. A round trip must return the same complex amplitude, so [WKB quantization](../../../../../wkb-quantization-condition.md) gives

$$
\boxed{\int_{r_t}^{r_o}\sqrt{\omega^2/c^2-L^2/r^2}\,dr=(n+\alpha)\pi.}
$$

Here $n$ counts radial oscillations, up to the choice of origin for radial order, and $\alpha$ incorporates both reflection phases. The outer acoustic reflection need not coincide exactly with the geometric stellar radius; replacing it by $R$ and absorbing its correction in $\alpha$ is the leading asymptotic approximation. The model neglects [buoyancy](../../../../../buoyancy.md), perturbations of self-gravity and rapid background variations on a wavelength.

Resolved observations of the [Sun](../../../../../sun.md) measure line-of-sight surface [velocity](../../../../../velocity.md) through the [Doppler effect](../../../../../doppler-effect.md), or brightness fluctuations. Projection on [spherical harmonics](../../../../../spherical-harmonic.md) identifies $\ell$ and azimuthal order $m$; a temporal [Fourier transform](../../../../../fourier-transform.md) identifies the mode [angular frequencies](../../../../../angular-frequency.md) $\omega$. The sequences of peaks of successive radial order form ridges in the frequency-degree diagram. Their ordering and comparison with a reference [stellar oscillation](../../../../../stellar-oscillation.md) model identify $n$; the surface image alone does not count inaccessible radial nodes. Fit the residual phase of the radial quantization relation across the observed mode set to estimate $\alpha$. A simultaneous fit with the sound-speed profile, or a calibrated reference model, is needed: $\alpha$ is not determined independently by one mode, and an integer shift of the numbering of $n$ shifts $\alpha$ oppositely. In a more accurate fit the surface phase depends on [frequency](../../../../../frequency.md). These steps constitute [helioseismology](../../../../../helioseismology.md).

Set $a(r)=c(r)/r$ and $w=\omega/L$. Assume $a$ decreases outwards in the region to be inverted. With the surface approximation above, the [Duvall law](../../../../../duvall-law.md) is

$$
F(w)=\frac{(n+\alpha)\pi}{\omega}
=\int_{r_t(w)}^R\sqrt{1-a(r)^2/w^2}\,\frac{dr}{c(r)}.
$$

Thus a suitably scaled mode set samples one function of $w$. Smooth the measured values before differentiating; inversion amplifies observational noise. At a finite outer reference point $r_s$, the already known contribution exterior to $r_s$ must be subtracted. For the remaining cavity, let $w_s=a(r_s)$ and $h(b)=-d\ln r/db$. Changing integration variable from radius to $b=a(r)$ gives

$$
F(w)=\int_{w_s}^{w}\frac{h(b)}{b}\sqrt{1-b^2/w^2}\,db,\qquad
F'(w)=\int_{w_s}^{w}\frac{h(b)b}{w^2\sqrt{w^2-b^2}}\,db.
$$

The boundary term vanishes because the square root vanishes at $b=w$. Now multiply the derivative by $w/\sqrt{a^2-w^2}$ and interchange the [integrals](../../../../../integral.md). The kernel identity

$$
\int_b^a\frac{dw}{w\sqrt{w^2-b^2}\sqrt{a^2-w^2}}=\frac{\pi}{2ab}
$$

follows by setting $w^2=b^2+(a^2-b^2)\sin^2\theta$ and then integrating $1/[b^2\cos^2\theta+a^2\sin^2\theta]$. It yields the [Abel inversion of stellar acoustic travel times](../../../../../abel-inversion-of-stellar-acoustic-travel-times.md):

$$
\boxed{\ln\frac{r_s}{r(a)}=\frac{2a}{\pi}\int_{w_s}^{a}\frac{wF'(w)}{\sqrt{a^2-w^2}}\,dw
=\frac{2a^2}{\pi}\int_{w_s/a}^1\frac{xF'(ax)}{\sqrt{1-x^2}}\,dx.}
$$

Knowing the monotone relation $r(a)$ then gives $c=ar$. Observed turning points delimit the region recoverable without extrapolation; an unknown surface contribution or nonmonotone $a$ prevents this simple unique inversion.

There are genuine inconsistencies in the printed numerical example. Since $w$ and $w_0$ have dimensions of angular frequency, $F$ must have dimensions of time, but the displayed empirical right-hand side is dimensionless. Moreover its derivative supplies a factor $1/w_0$, whereas the requested inversion supplies $1/w_0^2$. The dimensionally repaired relation that produces the requested inversion integral is

$$
F_c(w)=\frac{w}{w_0^2}\left(1-\frac{3w^2}{2\pi w_0^2}\right),\qquad
F_c'(w)=\frac{1}{w_0^2}\left(1-\frac{9w^2}{2\pi w_0^2}\right).
$$

Substitution in the boxed [Abel transform](../../../../../abel-transform.md) inversion gives precisely the exponent coefficient $2a^2/(\pi w_0^2)$, with the square-root denominator inside the integral. This repairs the first normalization but does not repair the later algebra.

Indeed, put $x_s=w_s/a$ and $b=\sqrt{1-x_s^2}$. The required elementary [integrals](../../../../../integral.md) evaluate to

$$
\int_{x_s}^1\frac{x\,dx}{\sqrt{1-x^2}}=b,\qquad
\int_{x_s}^1\frac{x^3\,dx}{\sqrt{1-x^2}}=b-\frac{b^3}{3}.
$$

The finite-reference-point answer following from $F_c$ is therefore

$$
\boxed{\ln\frac{r_s}{r}=\frac{2a^2}{\pi w_0^2}
\left[b-\frac{9a^2}{2\pi w_0^2}\left(b-\frac{b^3}{3}\right)\right].}
$$

It still depends on $w_s$. The later printed profile suppresses that dependence, which requires the additional surface limit $w_s\to0$, $r_s\to R$. Even in that limit it is not the result of this integral. To see this exactly, write $\mathcal L=\ln(R/r)$ and $y=a^2/(\pi w_0^2)$. The integral gives

$$
\mathcal L=2y-6y^2,\qquad
\boxed{c(r)=r w_0\sqrt{\frac{\pi}{6}\left(1-\sqrt{1-6\ln(R/r)}\right)}.}
$$

The minus branch is selected by $a\to0$ at the surface. Its decreasing-radius branch extends only to $\ln(R/r)=1/6$, where $a^2=\pi w_0^2/6$; it cannot describe $r=R/e$. The stated lower bound on the largest sampled $w$ does not fix this algebraic obstruction. In contrast, squaring and rearranging the printed closed profile would require $\mathcal L=18y-81y^2$. This differs identically from $2y-6y^2$, so the two printed steps cannot both follow from the same data.

The surface [polytrope](../../../../../polytrope.md) test can nevertheless be performed exactly, and clarifies the final discrepancy. For a plane-parallel [polytropic atmosphere](../../../../../polytropic-atmosphere.md) of index $m=3$, take $g=GM/R^2$ constant and $z=R-r$. The [stellar hydrostatic equation](../../../../../hydrostatic-pressure-support-equation.md) and $p=K\rho^{4/3}$ give $4p/\rho=gz$, hence the [surface sound speed of a polytropic star](../../../../../surface-sound-speed-of-a-polytropic-star.md) is

$$
\boxed{c^2\simeq\frac{\gamma GM}{4R^2}z,\qquad c_0=\sqrt{\frac{\gamma GM}{4R^2}}.}
$$

The exponent in the equilibrium [polytropic equation of state](../../../../../polytropic-equation-of-state.md) need not equal the perturbation [adiabatic exponent](../../../../../heat-capacity-ratio.md) $\gamma$. For the corrected inversion above, expansion at $z/R\ll1$ gives $c^2\simeq\pi w_0^2Rz/2$, so matching the surface [polytrope](../../../../../polytrope.md) fixes $w_0^2=\gamma GM/(2\pi R^3)$.

Alternatively, if the later printed closed profile is adopted as a separate imposed model, its surface expansion gives $c^2\simeq\pi w_0^2Rz/18$. It also has the correct square-root depth dependence, but requires

$$
\boxed{w_0^2=\frac{9\gamma GM}{2\pi R^3}\quad\text{for the printed closed profile}.}
$$

At $r=R/e$ that imposed profile then gives

$$
\boxed{c(R/e)=\frac1e\sqrt{\frac{\gamma GM}{2R}}.}
$$

The claimed coefficient $\pi/3$ is inconsistent with this substitution; $1/e\ne\pi/3$. Thus the surface scaling is demonstrable, but the empirical normalization, the requested closed inversion and the final numerical coefficient cannot all be asserted as printed. These discrepancies are visible in the original PDF, not introduced by its TeX conversion.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
