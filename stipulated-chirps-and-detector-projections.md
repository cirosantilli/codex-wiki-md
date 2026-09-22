# Stipulated chirps and detector projections

↑ **Parent:** [Newtonian binary chirp](newtonian-binary-chirp.md)

To construct an original example rather than imitate [GW150914](gw150914.md), set $G=6.67430\times10^{-11}\,\mathrm{m^3\,kg^{-1}\,s^{-2}}$, $c=299\,792\,458\,\mathrm{m\,s^{-1}}$, and adopt the rounded [solar mass](solar-mass.md) $M_\odot=1.98847\times10^{30}\,\mathrm{kg}$. Compare $10+10$ and $20+20$ [solar mass](solar-mass.md) binaries starting at $20\,\mathrm{Hz}$. Stop each at the stipulated [orbital compactness](orbital-compactness.md) threshold

$$
x=\frac{GM}{ac^2}=\left(\frac{\pi GMf}{c^3}\right)^{2/3}=0.10,\qquad
f_{\rm cut}=\frac{c^3}{\pi GM}(0.10)^{3/2}.
$$

This is a conservative pedagogical stopping rule, not a claimed error bound: the relative speed already reaches $\sqrt{0.10}\,c$. Higher-order corrections accumulate [wave phase](phase-waves.md) well before merger, and precision inference requires better models. The two cutoffs are approximately $102.2$ and $51.1\,\mathrm{Hz}$ respectively; doubling the [chirp mass](chirp-mass.md) multiplies $\dot f$ at fixed $f$ by $2^{5/3}$.

For a nearby stipulated source at distance $D$, neglect [redshift](redshift.md) and define inclination $\iota$ as the angle between the orbital [angular momentum](angular-momentum.md) and the line of sight. The leading [quadrupole formula](quadrupole-formula.md) yields

$$
A(f)=\frac{4(G\mathcal M)^{5/3}(\pi f)^{2/3}}{c^4D},\qquad
h_+=A(f)\frac{1+\cos^2\iota}{2}\cos\Phi,\qquad
h_\times=A(f)\cos\iota\sin\Phi.
$$

The numerator of $A$ has units $\mathrm{m^5\,s^{-4}}$, matching $c^4D$, so both polarizations are dimensionless. Its $f^{2/3}$ growth and the rising [frequency](frequency.md) produce the tightening, strengthening oscillations. For face-on viewing the polarization components have equal magnitudes in [phase quadrature](phase-quadrature.md); for edge-on viewing the cross component vanishes, agreeing with [circular-binary quadrupole radiation](circular-binary-quadrupole-radiation.md).

<a id="image-stipulated-newtonian-binary-chirps-and-two-ideal-detector-projections"></a>
![](newtonian-binary-chirps-detector-projections.png)

**[Figure 2](#image-stipulated-newtonian-binary-chirps-and-two-ideal-detector-projections). Stipulated Newtonian binary chirps and two ideal detector projections**. Calculated examples only: no measured [LIGO](ligo.md) strain or noise. Upper panels compare equal-mass binaries up to $x=0.10$. Lower panels use $20+20$ [solar masses](solar-mass.md), $D=500\,\mathrm{Mpc}$ and $\iota=60$ degrees. Ideal overhead detectors have $(F_+,F_\times)=(1,0)$ and $(1/2,\sqrt3/2)$; the second record has a stipulated $7\,\mathrm{ms}$ delay, then is shifted back for comparison. These geometries and delay are not fitted Hanford–Livingston responses.

Shifting an arrival time aligns the chirp evolution, but different polarization projections need not overlay after only a sign flip. The last panel divides the ideal projected records by their known envelope factors to expose this phase difference. A physical source model must jointly explain those differences, not erase them by arbitrary rescaling. Independent integration of the separation equation, the radiated [power](power.md) and $d\Phi/dt=2\pi f$ checks the analytic chirp against orbital [energy](energy-split.md) balance over the entire stipulated interval.

## ↑ Ancestors (6)

1. [Newtonian binary chirp](newtonian-binary-chirp.md)
2. [Gravitational wave](gravitational-wave-split.md)
3. [General relativity](general-relativity-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
