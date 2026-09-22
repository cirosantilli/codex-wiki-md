<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

**[virial pressure-radius curve with uniform-sphere binding energy](../../../../virial-pressure-radius-curve-with-uniform-sphere-binding-energy.md).** Put $c_s^2=k_BT/\mu$. Isothermality makes $\int(p/\rho)dM=c_s^2M_0$, so the [virial theorem](../../../../virial-theorem.md) gives

$$
\boxed{p_0=\frac{A}{r_0^3}-\frac{B}{r_0^4},\qquad
A=\frac{3c_s^2M_0}{4\pi},\quad B=\frac{3GM_0^2}{20\pi}}.
$$

The curve crosses zero at $r_z=B/A=GM_0/(5c_s^2)$, rises to its maximum at

$$
\boxed{r_c=\frac{4B}{3A}=\frac{4GM_0}{15c_s^2}},
$$

then decreases toward zero at large radius. Since $p_0'=(4B-3Ar_0)/r_0^5$, a cloud displaced outward at fixed external [pressure](../../../../pressure-split.md) has a restoring [pressure](../../../../pressure-split.md) deficit only on the descending branch. Thus **the homologous, isothermal radial mode is stable for $r_0>r_c$**, unstable for $r_z<r_0<r_c$, and marginal at $r_c$. The negative-pressure branch is not a physical equilibrium with a positive confining [pressure](../../../../pressure-split.md). This conclusion uses the stipulated gravitational-energy approximation, not the exact isothermal [density](../../../../density.md) profile.

<a id="1/image-original-pressure-radius-curve-and-stable-versus-unstable-branches-of-the-stipulated-virial-cloud-model"></a>
![](../../../../past-exam-of-the-formation-of-structure-in-the-universe-course-of-the-university-of-cambridge/2014/paper-1-virial-pressure.png)

**[Figure 1](#1/image-original-pressure-radius-curve-and-stable-versus-unstable-branches-of-the-stipulated-virial-cloud-model). Original pressure-radius curve and stable versus unstable branches of the stipulated virial cloud model**.

**[critical mass from a virial pressure turning point](../../../../critical-mass-from-a-virial-pressure-turning-point.md).** At the turning point, $B=3Ar_c/4$; hence

$$
\boxed{p_{\max}=\frac{A}{4r_c^3}
=\frac{10125}{1024\pi}\frac{c_s^8}{G^3M_0^2}
\propto\left(\frac{T^2}{M_0}\right)^2}.
$$

Using the cloud's [mean density](../../../../mean-density.md) $\bar\rho=3M_0/(4\pi r_0^3)$, the condition $r_0>4GM_0/(15c_s^2)$ becomes

$$
\boxed{M_0<M_{\rm crit}=\left(\frac{15c_s^2}{4G}\right)^{3/2}
\left(\frac{3}{4\pi\bar\rho}\right)^{1/2}
\propto\left(\frac{T^3}{\bar\rho}\right)^{1/2}}.
$$

Using the boundary [density](../../../../density.md) instead changes the numerical coefficient, not this scaling. The coefficient should not be identified with the exact [Bonnor-Ebert sphere](../../../../pressure-confined-isothermal-sphere.md) threshold because the assumed [potential energy](../../../../potential-energy.md) is different.

**[mass and luminosity weighting of a stellar initial mass function](../../../../mass-and-luminosity-weighting-of-a-stellar-initial-mass-function.md).** Impose finite birth-mass cutoffs $m_l,m_u$. The stellar birth [mass](../../../../mass.md) and main-sequence [luminosity](../../../../luminosity.md) scale as

$$
M_{\rm born}=\frac{\xi_0}{0.35}(m_l^{-0.35}-m_u^{-0.35}),\qquad
L_{\rm tot}\propto\frac{\xi_0}{2.65}(m_u^{2.65}-m_l^{2.65}).
$$

For a broad [mass](../../../../mass.md) interval, the low-mass end controls the first [integral](../../../../integral-split.md) and the high-mass end the second. Per logarithmic [mass](../../../../mass.md) interval the weights are respectively $m^2\xi\propto m^{-0.35}$ and $mL\xi\propto m^{2.65}$. Finite lifetimes remove massive stars from an aging population, so the [luminosity](../../../../luminosity.md) conclusion applies while those stars remain on the [main sequence](../../../../main-sequence.md).

**[exponential closed-box gas consumption](../../../../exponential-closed-box-gas-consumption.md).** The gross formation rate is $\Psi=\epsilon M_g$, but the permanent locking rate is $\alpha\Psi$. The [instantaneous recycling approximation](../../../../instantaneous-recycling-approximation.md) and [mass conservation](../../../../mass-conservation.md) give $\dot M_g=-\alpha\epsilon M_g$, $\dot M_*=\alpha\epsilon M_g$. Therefore

$$
\boxed{M_g=M_0e^{-\alpha\epsilon t},\qquad
M_*=M_0(1-e^{-\alpha\epsilon t}),\qquad
f_g=e^{-\alpha\epsilon t}}.
$$

Here $M_*$ means surviving locked stellar [mass](../../../../mass.md) in the [galactic gas fraction](../../../../galactic-gas-fraction.md), not the cumulative gross [mass](../../../../mass.md) that has passed through [star formation](../../../../star-formation.md).

**[locked-mass and returned-mass yield conventions](../../../../locked-mass-and-returned-mass-yield-conventions.md).** Pre-existing metals are locked at rate $\alpha Z\Psi$; the stipulated newly produced metal source is $b(1-\alpha)\Psi$. Thus

$$
\frac{d(M_gZ)}{dt}=-\alpha Z\Psi+b(1-\alpha)\Psi,
\qquad M_g\dot Z=b(1-\alpha)\Psi.
$$

For $\alpha>0$ and initially pristine gas,

$$
\boxed{Z=y\ln\frac{M_0}{M_g}=y\ln\frac1{f_g},\qquad
y=\frac{b(1-\alpha)}\alpha,\qquad
Z(t)=b(1-\alpha)\epsilon t}.
$$

The effective yield $y$ is per unit permanently locked [mass](../../../../mass.md); it is not the source parameter $b$. For $\alpha=0$, $M_g=M_0$ and the direct time equation gives $Z=b\epsilon t$. For $\alpha=1$, the explicitly stipulated metal source vanishes, so this particular enrichment model gives $Z=0$. Constant yield is a trace-enrichment approximation; the formal logarithmic divergence as gas is exhausted must not be interpreted as a physical metal fraction exceeding one.

**[backward extrapolation of exponential closed-box star formation](../../../../backward-extrapolation-of-exponential-closed-box-star-formation.md).** Denote the present [age of the universe](../../../../age-of-the-universe.md) by $t_{\rm now}$. With the last paragraph's $\alpha=1$,

$$
\boxed{\Psi(z\simeq3)=\left(1M_\odot\,\mathrm{yr^{-1}}\right)
\exp\left[0.5\left(\frac{t_{\rm now}}{\mathrm{Gyr}}-2\right)\right]}.
$$

Adopting a present [age of the universe](../../../../age-of-the-universe.md) $t_{\rm now}=13.8\,\mathrm{Gyr}$ for the estimate gives about **$365M_\odot\,\mathrm{yr^{-1}}$**, requiring $7.3\times10^{11}M_\odot$ of gas at that epoch in the same model. The boxed expression makes the dependence on the adopted present age explicit. This is an extreme history for a present Milky-Way-like system, although intense high-redshift [star formation](../../../../star-formation.md) by itself is not forbidden.

The extrapolation forces a fixed gas reservoir to decline exponentially over many [gas-depletion times](../../../../gas-depletion-time.md). Gas [accretion](../../../../accretion.md), outflows, evolving gas [density](../../../../density.md) and star-formation efficiency, delayed recycling, and galaxy assembly break that assumption. The empirical disk-averaged relation is not a universal constant-efficiency law for all gas: the original measurements combined [Balmer series](../../../../balmer-series.md) H-alpha, atomic gas, [carbon monoxide](../../../../carbon-monoxide.md) and [infrared](../../../../infrared.md) data, with tracer calibration and dust corrections entering the inference.[Abstract: observed tracers, sample, and fitted index](../../../../the-global-schmidt-law-in-star-forming-galaxies-by-robert-c-kennicutt-jr.md) Cosmological calculations explicitly support continuing cold-gas supply to rapidly forming high-redshift galaxies, providing a physical alternative to this closed-box backward extrapolation.[Abstract: stream-fed galaxies and comparison with observed abundance](../../../../cold-streams-in-early-massive-hot-haloes-as-the-main-mode-of-galaxy-formation-by-avishai-dekel-and-others.md)

## ↑ Ancestors (13)

1. [1](../1.md)
2. [Paper 1](../../paper-1-split.md)
3. [2014](../../split.md)
4. [Past exam of the formation of Structure in the Universe course of the University of Cambridge](../../../split.md)
5. [Formation of Structure in the Universe course of the University of Cambridge](../../../../formation-of-structure-in-the-universe-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
