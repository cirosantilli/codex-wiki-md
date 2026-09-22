<h1 id="section-d/d13/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [p-n junction](../../../../../../p-n-junction.md) brings p-type and n-type regions into contact. Majority-carrier diffusion initially leaves exposed ionized acceptors and donors, producing a [depletion region](../../../../../../depletion-region.md) and a [built-in potential](../../../../../../built-in-potential.md). At [thermal equilibrium](../../../../../../thermal-equilibrium-split.md) the electrochemical potential is constant: drift and diffusion currents cancel. The internal barrier is not a freely extractable battery voltage.

For a nondegenerate abrupt homojunction,

$$
V_{\rm bi}=\frac{k_BT}{q}\ln\frac{N_AN_D}{n_i^2},\qquad
W=\sqrt{\frac{2\epsilon_s}{q}(V_{\rm bi}-V)
\left(\frac1{N_A}+\frac1{N_D}\right)}.
$$

Here $V>0$ denotes [forward bias](../../../../../../forward-bias.md) and the [depletion approximation](../../../../../../depletion-approximation.md) is assumed. [forward bias](../../../../../../forward-bias.md) lowers the barrier and injects [minority carriers](../../../../../../minority-carrier.md); [reverse bias](../../../../../../reverse-bias.md) widens the depleted region and suppresses ordinary majority injection. In the ideal diffusion regime,

$$
\boxed{I=I_s[\exp(qV/(k_BT))-1].}
$$

Recombination can change the ideality factor; series resistance, high-level injection, leakage and breakdown limit this simple [Shockley diode equation](../../../../../../shockley-diode-equation.md). The original junction theory explicitly treats both [electron](../../../../../../electron.md) and hole currents, which is essential to [carrier injection](../../../../../../carrier-injection.md) and transistor action.[1949, pp.435–436, introduction: rectification, photosensitivity and injection of minority carriers](../../../../../../the-theory-of-p-n-junctions-in-semiconductors-and-p-n-junction-transistors-by-william-shockley.md)

As a rectifying [diode](../../../../../../diode.md), the junction conducts strongly in one bias direction and weakly in the other before breakdown. This permits power rectification, signal detection and electronic switching. Stored minority charge affects turn-off time, so a static exponential current-voltage relation alone does not specify switching speed. A [junction capacitance](../../../../../../junction-capacitance.md) $C_j\simeq\epsilon_sA/W$ varies with [reverse bias](../../../../../../reverse-bias.md) and can be used in a voltage-controlled capacitor; heavily doped or high-field junctions can instead exploit controlled tunnelling or avalanche breakdown.

In a [photodiode](../../../../../../photodiode.md), absorbed photons generate [electron-hole pairs](../../../../../../electron-hole-pair.md) and the depleted-region field assists collection. [reverse bias](../../../../../../reverse-bias.md) widens the collecting region and can improve speed, but adds dark-current noise and breakdown constraints. In a [solar cell](../../../../../../solar-cell.md), the same carrier generation supplies current against an external voltage. An ideal illuminated characteristic is $I=I_s(e^{qV/(k_BT)}-1)-I_{\rm ph}$: at open circuit the forward [diode](../../../../../../diode.md) current balances photocurrent, while useful power is taken at an intermediate operating point. Neither short circuit nor open circuit delivers power to a load.

A forward-biased [light-emitting diode](../../../../../../light-emitting-diode.md) injects [electrons](../../../../../../electron.md) and holes that can recombine radiatively. Efficient emission favors suitable direct-gap materials and carrier confinement; the characteristic [photon energy](../../../../../../photon-energy.md) is near the [semiconductor](../../../../../../semiconductor-split.md) [band gap](../../../../../../band-gap.md). [nonradiative recombination](../../../../../../nonradiative-recombination.md), escape losses, series resistance and heating limit efficiency. Two coupled junctions also form a [bipolar junction transistor](../../../../../../bipolar-junction-transistor.md): an emitter injects [minority carriers](../../../../../../minority-carrier.md) through a thin base, and a reverse-biased collector collects them. Useful current gain depends on efficient injection and limited base recombination, not simply on joining any three arbitrary regions.

These functions are experimentally distinguished by measuring dark and illuminated current-voltage curves, bias-dependent capacitance, transient switching or optical emission, with controlled [temperature](../../../../../../temperature-split.md) and current limits. **The common mechanism is bias-controlled [carrier injection](../../../../../../carrier-injection.md) or collection at a depletion barrier; the device geometry and operating mode determine which function is useful.**

## ↑ Ancestors (15)

1. [C](../c.md)
2. [D13](../../d13.md)
3. [Section D](../../../section-d.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
