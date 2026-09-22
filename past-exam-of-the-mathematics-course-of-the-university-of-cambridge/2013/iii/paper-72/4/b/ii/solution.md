<h1 id="4/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Solar geometry must be included before multiplying by the summer duration. Let $\phi=71^\circ$, solar declination $\delta$, and hour angle $u$, measured from local noon. The cosine of solar zenith angle is

$$
\cos\zeta=\sin\phi\sin\delta+\cos\phi\cos\delta\cos u.
$$

Only positive values receive sunlight. Integrating through a day gives the [daily mean solar irradiance](../../../../../../../daily-mean-solar-irradiance.md) at the top of the atmosphere:

$$
\overline S=\frac{S_0}{\pi}
[H_0\sin\phi\sin\delta+\cos\phi\cos\delta\sin H_0],
\qquad H_0=\arccos(-\tan\phi\tan\delta),
$$

with $H_0$ clipped to $\pi$ for polar day and to zero for polar night. At the solstice, for example, polar-day averaging gives $\overline S=S_0\sin71^\circ\sin23.44^\circ\simeq514\,\mathrm{W\,m^{-2}}$. It would be wrong to apply $S_0$ continuously to a horizontal surface.

A simple seasonal approximation $\delta(n)=23.44^\circ\sin[2\pi(n-80)/365]$, with calendar day $n$, gives a June–August daily-mean average of about $427\,\mathrm{W\,m^{-2}}$. There are 92 days. With [surface albedo](../../../../../../../surface-albedo.md) $\alpha=0.1$, the no-atmosphere absorbed-solar ceiling is

$$
\boxed{Q_{\rm solar,TOA}
=(1-\alpha)\sum_{n=152}^{243}\overline S(n)(86400)
\simeq3.06\times10^9\,\mathrm{J\,m^{-2}}.}
$$

This calculation neglects the small seasonal change in Earth-Sun distance. The ceiling is larger than the $1.80\,\mathrm{GJ\,m^{-2}}$ required in part (i), so geometry alone does not make a uniform $7^\circ\mathrm C$ column impossible.

A reasonable conditional estimate includes an effective atmospheric short-wave transmission $\tau$ and net non-solar loss $\overline L$:

$$
Q_{\rm stored}\simeq\tau Q_{\rm solar,TOA}
-\overline L(92)(86400),
$$

before adding advection or subtracting ice melting. The parameters are scenario assumptions, not measurements supplied by the question. For example, $\tau=0.6$ gives $1.83\,\mathrm{GJ\,m^{-2}}$ before other losses, barely enough; with a modest mean loss of $50\,\mathrm{W\,m^{-2}}$, the retained amount is only $1.44\,\mathrm{GJ\,m^{-2}}$. That would raise a uniform 50 m column from freezing by about $7.0\,\mathrm K$, reaching roughly $5.2^\circ\mathrm C$. With no other losses the transmission required for $7^\circ\mathrm C$ is $1.804/3.058\simeq0.590$; with that illustrative loss it rises to about $0.720$. Clouds, emitted thermal radiation, evaporation, transfer to colder water and melting all affect the balance.

**The satellite surface temperature is insufficient evidence for a $7^\circ\mathrm C$ seabed.** A warm, shallow [ocean mixed layer](../../../../../../../ocean-mixed-layer.md) can overlie colder water because meltwater and salinity maintain [stable density stratification](../../../../../../../stable-density-stratification.md). Heating only the upper 10 m through $8.8\,\mathrm K$ costs $0.361\,\mathrm{GJ\,m^{-2}}$, much less than heating all 50 m. Warm Pacific-water advection can also raise surface temperature or supply additional heat. If measured net solar input were too small for full-depth warming, shallow surface heating would be the natural alternative; if mixing and additional heat supply were strong enough, full-depth warming remains possible. The missing transmission, loss, mixing and inflow information prevents a unique yes-or-no conclusion from the supplied surface observation.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 72](../../../../paper-72-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
