<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [luminosity distance](../../../../../../luminosity-distance.md) is defined operationally by the bolometric relation $F=L/(4\pi d_L^2)$ for an isotropic source. It incorporates geometric spreading, reduced photon energy and dilated photon arrival times. If $D_M$ is the transverse comoving distance with the present scale factor included, then $d_L=(1+z)D_M$ in a spacetime with an [FLRW metric](../../../../../../friedmann-lemaitre-robertson-walker-metric.md) with photon number conserved.

Let $\nu_e=(1+z)\nu_o$ be the emitted frequency. A narrow emitted band carries energy $P(\nu_e)\,d\nu_e\,dt_e\,d\Omega$. At the observer the energy is smaller by $1+z$, the time interval is $dt_o=(1+z)dt_e$, the frequency interval is $d\nu_o=d\nu_e/(1+z)$, and the illuminated area is $D_M^2d\Omega$. Hence the spectral [spectral flux density](../../../../../../spectral-flux-density.md) per unit observed frequency is

$$
S(\nu_o)=\frac{P((1+z)\nu_o)}{(1+z)D_M^2}
=\frac{(1+z)P((1+z)\nu_o)}{d_L^2}.
$$

For the specified power law, $P((1+z)\nu_o)=(1+z)^{-\alpha}P(\nu_o)$, so the [power-law spectral K correction](../../../../../../power-law-spectral-k-correction.md) is

$$
\boxed{S(\nu_o)=P(\nu_o)(1+z)^{1-\alpha}d_L^{-2}.}
$$

There is no extra $4\pi$ because $P$ is power per steradian. For total spectral luminosity $L_\nu=4\pi P_\nu$, that factor would instead appear in the denominator. The frequency-band factor is essential: bolometric flux has two redshift-dimming factors, but spectral flux has one of them compensated by the bandwidth change.

## ↑ Ancestors (11)

1. [C](../c.md)
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
