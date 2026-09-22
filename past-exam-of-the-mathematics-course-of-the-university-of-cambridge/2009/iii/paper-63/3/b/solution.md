<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use $f=X_{22}$ for the neon-22 [mass](../../../../../../mass.md) fraction, temporarily keeping it distinct from the earlier metallicity. Let $n_b=\rho/m_u$ be the baryon density, ignoring small nuclear [mass](../../../../../../mass.md) defects. Equal masses of [carbon](../../../../../../carbon.md) and [oxygen](../../../../../../oxygen.md) give

$$
n_C=\frac{1-f}{24}n_b,\qquad n_O=\frac{1-f}{32}n_b,\qquad
n_{22}=\frac f{22}n_b.
$$

Carbon-12 and oxygen-16 each have equal [proton](../../../../../../proton.md) and [neutron](../../../../../../neutron.md) numbers, while neon-22 has ten [protons](../../../../../../proton.md) and twelve [neutrons](../../../../../../neutron.md). The total [proton](../../../../../../proton.md) and [neutron](../../../../../../neutron.md) numbers per baryon are consequently

$$
Y_e=6\frac{1-f}{24}+8\frac{1-f}{32}+10\frac f{22}
=\frac12-\frac f{22},
$$



$$
1-Y_e=\frac12+\frac f{22}.
$$

Hence

$$
\boxed{\frac{\langle Z\rangle}{\langle N\rangle}
=\frac{Y_e}{1-Y_e}=\frac{11-f}{11+f}.}
$$

The equal [carbon](../../../../../../carbon.md)/[oxygen](../../../../../../oxygen.md) [mass](../../../../../../mass.md) split cancels from this result: any mixture of these two symmetric nuclei has the same electron fraction. Taking the paper's metallicity symbol to mean $f$ gives its requested expression.

The literal pre-helium-burning [nitrogen](../../../../../../nitrogen.md) interpretation, however, needs a correction. Each initial nitrogen-14 nucleus receives two alpha particles, including eight additional baryons, before becoming neon-22; the intervening [beta-plus decay](../../../../../../beta-plus-decay.md) also emits a [neutrino](../../../../../../neutrino.md). Thus, if the entire original metallicity is nitrogen-14 with [mass](../../../../../../mass.md) fraction $Z_{\mathrm{initial}}$, conservation of the number of seed nuclei gives

$$
X_{22}=\frac{22}{14}Z_{\mathrm{initial}},\qquad
\boxed{\frac{\langle Z\rangle}{\langle N\rangle}
=\frac{7-Z_{\mathrm{initial}}}{7+Z_{\mathrm{initial}}}.}
$$

This is [neon-22 neutron excess from nitrogen-14](../../../../../../neon-22-neutron-excess-from-nitrogen-14.md). The two expressions are compatible only when their arguments are distinguished: the displayed $(11-Z)/(11+Z)$ law uses the final [neon](../../../../../../neon.md) [mass](../../../../../../mass.md) fraction, not literally the earlier [nitrogen](../../../../../../nitrogen.md) [mass](../../../../../../mass.md) fraction. Treating those fractions as equal is an extra simplifying approximation, not a consequence of the stated capture chain.

A [radioactively powered Type Ia supernova light curve](../../../../../../radioactively-powered-type-ia-supernova-light-curve.md) rises to a broad maximum over roughly weeks as energy deposited in expanding ejecta diffuses out, then declines over the following weeks and months. Its power comes predominantly from the [nickel-56 decay chain](../../../../../../nickel-56-decay-chain.md), first [nickel](../../../../../../nickel.md) to [cobalt](../../../../../../cobalt.md) and then [cobalt](../../../../../../cobalt.md) to [iron](../../../../../../iron.md). Gamma rays and charged decay products deposit heat, which is reprocessed into optical and infrared radiation. At later times, declining [cobalt](../../../../../../cobalt.md) decay power and increasing gamma-ray escape shape the tail. It is not sustained nuclear fusion in the expanding ejecta. The amount of radioactive [nickel](../../../../../../nickel.md), [photon](../../../../../../photon.md) diffusion time and deposition efficiency all matter, so an uncorrected fixed [luminosity](../../../../../../luminosity.md) is only an idealization.

For the requested two-isotope yield calculation, assume the same total processed iron-group [mass](../../../../../../mass.md), namely $1M_\odot$ as inferred from the zero-neon reference. Treat the final freeze-out ashes as nickel-56 and iron-54, neglecting residual light particles and additional weak neutronization. If $w$ is the [nickel](../../../../../../nickel.md) [mass](../../../../../../mass.md) fraction, conservation of electron fraction gives

$$
\frac w2+(1-w)\frac{26}{54}=\frac12-\frac f{22}.
$$

Since $26/54=1/2-1/54$, this reduces to the [metallicity dependence of nickel-56 yield](../../../../../../metallicity-dependence-of-nickel-56-yield.md)

$$
\boxed{w=1-\frac{27}{11}f.}
$$

Under the paper's intended identification $f=Z=1/50$,

$$
\boxed{M_{56}=\left(1-\frac{27}{550}\right)M_\odot
=\frac{523}{550}M_\odot\simeq0.95M_\odot\quad\text{(two significant figures)}.}
$$

If instead $Z=1/50$ denotes the earlier [nitrogen](../../../../../../nitrogen.md) [mass](../../../../../../mass.md) fraction, retaining the actual capture stoichiometry gives $w=1-27Z/7=323/350$ and $M_{56}\simeq0.92M_\odot$. The same [temperature](../../../../../../temperature.md) and density do not alone fix a total burned [mass](../../../../../../mass.md); equality of that [mass](../../../../../../mass.md) is also implicit in the comparison. The two-isotope assumption is a bulk-ash approximation, not a complete equilibrium network with all free particles identically absent.

For otherwise comparable explosions, approximate the peak [luminosity](../../../../../../luminosity.md) by a quantity proportional to the radioactive [nickel](../../../../../../nickel.md) [mass](../../../../../../mass.md). Let $d$ be the true distance to an extremely low-neon event, and use the solar calibration $L_\odot/L_0=523/550$. Its measured flux is $F=L_0/(4\pi d^2)$, but the inferred standard-candle distance is

$$
\boxed{\frac{d_{\mathrm{est}}}{d}
=\sqrt{\frac{L_\odot}{L_0}}=\sqrt{\frac{523}{550}}\simeq0.975.}
$$

The source is intrinsically brighter than the calibration, so the distance is underestimated by about $2.5\%$, conventionally described here as about $3\%$. Equivalently, $d/d_{\mathrm{est}}=\sqrt{550/523}\simeq1.0255$, consistent with the supplied rounded factor $1.03$. Using the literal [nitrogen](../../../../../../nitrogen.md) metallicity instead gives about a $4\%$ underestimate. These are conditional composition effects in this simplified model; real Type Ia distance estimation also standardizes light-curve shape and color.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 63](../../../paper-63-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
