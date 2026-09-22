<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the [two-zone cloudy annulus transmission model](../../../../../../two-zone-cloudy-annulus-transmission-model.md), assume a uniform stellar disc, an opaque planet below $R_p$, $0\leq H_c\leq H$, and constant total slant [optical depth](../../../../../../optical-depth.md) within each radial zone. Neglect scattered light entering the beam and the planet's own emission. A ray transmits the fraction $e^{-\tau}$, so each zone blocks its projected area multiplied by $1-e^{-\tau}$.

The opaque disc, cloudy annulus and clear annulus have areas $\pi R_p^2$, $\pi[(R_p+H_c)^2-R_p^2]$ and $\pi[(R_p+H)^2-(R_p+H_c)^2]$, respectively. Thus the [exoplanet transmission spectrum](../../../../../../exoplanet-transmission-spectrum.md), expressed as total transit depth, is

$$
\boxed{\begin{aligned}
\delta_\lambda=1-\frac{F_{\rm in,\lambda}}{F_{\rm out,\lambda}}
={}&\frac{R_p^2}{R_s^2}
+\frac{(R_p+H_c)^2-R_p^2}{R_s^2}(1-e^{-\tau_{\lambda,c}})\\
&+\frac{(R_p+H)^2-(R_p+H_c)^2}{R_s^2}(1-e^{-\tau_\lambda}).
\end{aligned}}
$$

Here $\tau_{\lambda,c}$ means the total [optical depth](../../../../../../optical-depth.md) on rays assigned to the cloudy zone. If it denotes cloud extinction alone, its exponent must instead contain the sum of cloud and gas [optical depths](../../../../../../optical-depth.md). For a geometrically thin [exoplanet atmosphere](../../../../../../exoplanet-atmosphere.md), the two atmospheric prefactors become $2R_pH_c/R_s^2$ and $2R_p(H-H_c)/R_s^2$.

An opaque [exoplanet cloud deck](../../../../../../exoplanet-cloud-deck.md) gives the simpler expression

$$
\delta_\lambda=\frac{(R_p+H_c)^2}{R_s^2}+\frac{(R_p+H)^2-(R_p+H_c)^2}{R_s^2}(1-e^{-\tau_\lambda}).
$$

The [exoplanet cloud deck](../../../../../../exoplanet-cloud-deck.md) raises the wavelength-independent occulting radius and suppresses the clear atmospheric contribution. If $H_c=H$, the spectrum is flat at $(R_p+H)^2/R_s^2$; if $H_c=0$, the ordinary [annulus model for transmission spectroscopy](../../../../../../annulus-model-for-transmission-spectroscopy.md) is recovered. Stellar limb darkening and varying tangent-ray [optical depth](../../../../../../optical-depth.md) would require an intensity-weighted radial integral rather than this constant-depth model.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 315](../../../paper-315-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
