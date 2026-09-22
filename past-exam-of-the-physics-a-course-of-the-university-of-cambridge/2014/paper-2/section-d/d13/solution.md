<h1 id="section-d/d13/solution">Solution</h1>

↑ **Parent:** [D13](../d13.md)

Donor doping supplies conduction [electrons](../../../../../electron.md) to [n-type semiconductor](../../../../../n-type-semiconductor.md); acceptor doping supplies [holes](../../../../../electron-hole.md) to [p-type semiconductor](../../../../../p-type-semiconductor.md). In the nondegenerate, fully ionized limit, majority densities are approximately $n_n=N_D$ and $p_p=N_A$, while minority densities follow $np=n_i^2$. On contact, majority carriers diffuse across the junction, exposing positive donor ions on the n side and negative acceptor ions on the p side. The depletion-region [electric field](../../../../../electric-field-split.md) points from n to p and opposes further [diffusion](../../../../../diffusion.md). At [thermal equilibrium](../../../../../thermal-equilibrium-split.md) the [Fermi level](../../../../../fermi-level.md) is uniform and drift balances [diffusion](../../../../../diffusion.md), with no net current.

For an abrupt junction with uniform doping and permittivity $\varepsilon_s$, charge neutrality gives $N_Dx_n=N_Ax_p$. [Poisson's equation](../../../../../poisson-s-equation.md) then gives

$$
V_{\rm bi}=\frac{k_BT}{q}\log\frac{N_AN_D}{n_i^2},\qquad
\boxed{W=x_n+x_p=
\sqrt{\frac{2\varepsilon_s}{q}\left(\frac1{N_A}+\frac1{N_D}\right)(V_{\rm bi}-V)}}.
$$

Positive applied $V$ means [forward bias](../../../../../forward-bias.md): it lowers the barrier and narrows the [depletion region](../../../../../depletion-region.md). Most depletion width lies in the more lightly doped side. The formula assumes the [depletion approximation](../../../../../depletion-approximation.md) and fails once its operating assumptions break down.

[forward bias](../../../../../forward-bias.md) increases minority densities at the depletion edges by the factor $e^{qV/k_BT}$. In the neutral material, the steady [diffusion](../../../../../diffusion.md)–[recombination](../../../../../recombination-cosmology.md) equation gives exponentially decaying excess minorities, with lengths $L_n=\sqrt{D_n\tau_n}$ and $L_p=\sqrt{D_p\tau_p}$. Taking the carrier gradients at the junction yields

$$
\boxed{I=I_S\left(e^{qV/k_BT}-1\right),\qquad
I_S=qA_jn_i^2\left(\frac{D_n}{L_nN_A}+\frac{D_p}{L_pN_D}\right)}.
$$

This ideal [diode](../../../../../diode.md) law assumes low injection, nondegenerate statistics, negligible depletion-region [recombination](../../../../../recombination-cosmology.md) and series resistance, and sufficiently long neutral regions. Its exponential comes from the bias-dependent injection barrier; there is no universal abrupt “turn-on” voltage. [reverse bias](../../../../../reverse-bias.md) suppresses injection, giving an approximate $-I_S$ current until additional leakage or breakdown matters.[Bell System Technical Journal 28, pp. 435–489, minority-carrier injection and rectifying-junction theory](../../../../../the-theory-of-p-n-junctions-in-semiconductors-and-p-n-junction-transistors-by-william-shockley.md)

Rectification uses the asymmetric [current-voltage characteristic](../../../../../current-voltage-characteristic.md); controlled reverse breakdown enables voltage references, with current limiting. Bias-dependent depletion capacitance enables varactors. [photodiodes](../../../../../photodiode.md) and [solar cells](../../../../../solar-cell.md) collect optically generated carriers through the junction field and diffusion toward it; efficient [light-emitting diodes](../../../../../light-emitting-diode.md) use radiative [electron](../../../../../electron.md)–[hole](../../../../../electron-hole.md) [recombination](../../../../../recombination-cosmology.md), preferably in a direct-gap material. Series resistance, high injection, trap-assisted [recombination](../../../../../recombination-cosmology.md), heating and finite carrier storage explain departures from the ideal steady-state law.

## ↑ Ancestors (14)

1. [D13](../d13.md)
2. [Section D](../../section-d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2014](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
