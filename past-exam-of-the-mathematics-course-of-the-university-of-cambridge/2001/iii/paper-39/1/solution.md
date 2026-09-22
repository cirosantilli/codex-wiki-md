<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [specific intensity](../../../../../specific-intensity.md) of a [blackbody](../../../../../blackbody.md) is direction-independent over its outward hemisphere. Its outward flux per unit frequency is therefore

$$
F_\nu=\int_{\rm outward} B_\nu\cos\theta\,d\Omega
=2\pi B_\nu\int_0^{\pi/2}\cos\theta\sin\theta\,d\theta=\pi B_\nu.
$$

Multiplying by the stellar surface area gives the [spectral luminosity](../../../../../spectral-luminosity.md)

$$
\boxed{L_\nu=4\pi^2R_s^2B_\nu.}
$$

Using the [Planck law](../../../../../planck-s-law.md), the [hydrogen-ionizing photon production rate](../../../../../hydrogen-ionizing-photon-production-rate.md) follows by dividing each spectral contribution by its [photon](../../../../../photon.md) energy and integrating above the threshold:

$$
Q_H=\int_{I_H/h}^\infty\frac{L_\nu}{h\nu}\,d\nu
=\frac{8\pi^2R_s^2}{c^2}\int_{I_H/h}^\infty\frac{\nu^2}{e^{h\nu/kT_s}-1}\,d\nu.
$$

With $x=h\nu/(kT_s)$ and $y=I_H/(kT_s)$, this becomes

$$
Q_H=\frac{8\pi^2I_H^3}{h^3c^2}\frac{R_s^2}{y^3}
\int_y^\infty\frac{x^2}{e^x-1}\,dx.
$$

For the initial hydrogen-only [photon](../../../../../photon.md) balance, assume an [ionization-bounded nebula](../../../../../ionization-bounded-nebula.md) at steady [photoionization equilibrium](../../../../../photoionization-equilibrium.md), negligible dust absorption and ionizing-photon leakage, negligible [collisional ionization](../../../../../collisional-ionization.md), and local reabsorption of [photons](../../../../../photon.md) from direct ground-state recombinations. A ground-state recombination then causes another [photoionization](../../../../../photoionization.md) and produces no net removal of a proton. Net removal is counted by [Case B recombination](../../../../../case-b-recombination.md), whose coefficient is $\beta=\sum_{n\geq2}\alpha_n$. Integrating the local balance gives

$$
\boxed{\int N_eN_+\beta\,dV=Q_H
=\frac{8\pi^2I_H^3}{h^3c^2}\frac{R_s^2}{y^3}
\int_y^\infty\frac{x^2}{e^x-1}\,dx.}
$$

The stellar [temperature](../../../../../temperature.md) $T_s$ sets the [photon](../../../../../photon.md) supply; the gas [temperature](../../../../../temperature.md) sets the recombination coefficients. They are not generally equal. For uniform [hydrogen](../../../../../hydrogen.md) and constant gas [temperature](../../../../../temperature.md), the [Strömgren radius](../../../../../stromgren-radius.md) is

$$
R_H=\left(\frac{3Q_H}{4\pi\beta_HN_eN_H}\right)^{1/3},
$$

with $N_e=N_H$ in fully ionized pure [hydrogen](../../../../../hydrogen.md).

For the hydrogen-helium mixture, define the [blackbody ionizing photon function](../../../../../blackbody-ionizing-photon-function.md)

$$
F(y)=\int_y^\infty\frac{x^2}{e^x-1}\,dx,\qquad
Q(E_0)=\frac{8\pi^2R_s^2(kT_s)^3}{h^3c^2}F(E_0/kT_s).
$$

The three relevant thresholds are approximately $13.6$, $24.6$ and $54.4\,\mathrm{eV}$, for $\mathrm H^0$, $\mathrm{He}^0$ and $\mathrm{He}^+$ respectively. Higher stellar [temperature](../../../../../temperature.md) increases the relative supply of the harder [photons](../../../../../photon.md). These cumulative [photon](../../../../../photon.md) rates cannot be assigned independently to the three species: a [photon](../../../../../photon.md) above a [helium](../../../../../helium.md) threshold can instead ionize [hydrogen](../../../../../hydrogen.md), and [helium](../../../../../helium.md) recombination radiation can also ionize [hydrogen](../../../../../hydrogen.md). The absorption cross-sections and the diffuse radiation determine the effective allocation.

A useful sharp-front model of [nested hydrogen-helium ionization zones](../../../../../nested-hydrogen-helium-ionization-zones.md) has an inner $\mathrm{He}^{++}$ sphere of radius $R_2$, a $\mathrm{He}^+$ shell ending at $R_1$, and an outer hydrogen-ionized region ending at $R_H$, with $R_2\leq R_1\leq R_H$. Let $n_H,n_{He}$ be uniform nuclear number densities. The [electron number densities](../../../../../electron-number-density.md) in these three regions are $n_H+2n_{He}$, $n_H+n_{He}$ and $n_H$. For constant gas [temperature](../../../../../temperature.md), integrating the recombination rates gives

$$
\begin{aligned}
Q_H^{\rm eff}&=\frac{4\pi}{3}\beta_H n_H\{n_HR_H^3+n_{He}(R_1^3+R_2^3)\},\\
Q_{HeI}^{\rm eff}&=\frac{4\pi}{3}\beta_{HeI}n_{He}(n_H+n_{He})(R_1^3-R_2^3),\\
Q_{HeII}^{\rm eff}&=\frac{4\pi}{3}\beta_{HeII}n_{He}(n_H+2n_{He})R_2^3.
\end{aligned}
$$

Here the effective budgets mean net species-specific ionizations after eliminating local ground-state recycling. Their calculation must include [photon](../../../../../photon.md) competition and any interspecies diffuse contribution; the [helium](../../../../../helium.md) coefficients label the recombining [ion](../../../../../ion.md)'s emitted spectrum. Once these budgets are specified, solve the third equation for $R_2^3$, the second for $R_1^3-R_2^3$, and the first for $R_H^3$.

For an isolated [helium](../../../../../helium.md) front with approximately common [electron number density](../../../../../electron-number-density.md), the useful scaling is

$$
\left(\frac{R_{He}}{R_H}\right)^3
\simeq\frac{Q_{He}^{\rm eff}}{Q_H^{\rm eff}}
\frac{n_H\beta_H}{n_{He}\beta_{He}}.
$$

Thus the small [helium](../../../../../helium.md) abundance partly compensates for the smaller hard-photon supply. A cooler central star produces little $\mathrm{He}^{++}$ and can have a substantially smaller helium-ionized zone. A sufficiently hot star can ionize [helium](../../../../../helium.md) throughout most of the [hydrogen](../../../../../hydrogen.md) region. If independent radius estimates place a [helium](../../../../../helium.md) front beyond the [hydrogen](../../../../../hydrogen.md) front, the independent [photon](../../../../../photon.md) allocations are inconsistent: the fronts and transfer must be treated together. **The radii depend on [photon](../../../../../photon.md) hardness, abundance, [electron number density](../../../../../electron-number-density.md) and recombination rates, not on thresholds alone.** The sharp-front equations are an approximation; they do not assert three exact independently conserved [photon](../../../../../photon.md) budgets for a real mixed nebula.

For a nonuniform nebula, an observed [recombination line](../../../../../recombination-line.md) with [effective recombination coefficient](../../../../../effective-recombination-coefficient.md) $\alpha_\ell^{\rm eff}$ has [luminosity](../../../../../luminosity.md)

$$
L_\ell=h\nu_\ell\int N_eN_{\rm parent}\alpha_\ell^{\rm eff}\,dV.
$$

If gas [temperature](../../../../../temperature.md) and density permit a known approximately constant ratio $\beta/\alpha_\ell^{\rm eff}$, the integrated line gives

$$
Q^{\rm eff}=\frac{\beta}{\alpha_\ell^{\rm eff}}\frac{L_\ell}{h\nu_\ell}.
$$

The unknown density distribution cancels because the same recombination integral appears in both quantities. For a stellar continuum measurement at a nonionizing frequency $\nu_o$,

$$
F_{\nu_o,*}=\pi B_{\nu_o}(T_s)\frac{R_s^2}{d^2}.
$$

When the inferred recombination budget traces the full appropriate ionizing-photon supply, define $\Phi_{E_0}(T)=\int_{E_0/h}^\infty B_\nu(T)/(h\nu)\,d\nu$ and obtain the [Zanstra method](../../../../../zanstra-method.md) equation

$$
\boxed{\frac{F_\ell}{h\nu_\ell F_{\nu_o,*}}\frac{\beta}{\alpha_\ell^{\rm eff}}
=\frac{\Phi_{E_0}(T_s)}{B_{\nu_o}(T_s)}.}
$$

Both $R_s$ and the distance $d$ cancel. [Hydrogen](../../../../../hydrogen.md) and [helium](../../../../../helium.md) recombination lines probe different hardness thresholds, so their ratios and the stellar continuum constrain $T_s$ and test the assumed spectrum and trapping. For a mixed nebula, use the corresponding transfer-corrected [photon](../../../../../photon.md) budgets. [temperature](../../../../../temperature.md) gradients require emission-weighted coefficients; dust, leakage, density-bounded [helium](../../../../../helium.md) zones or departures from a [blackbody](../../../../../blackbody.md) can produce discrepant [hydrogen](../../../../../hydrogen.md) and [helium](../../../../../helium.md) Zanstra estimates. Line fluxes alone without an appropriate budget or continuum normalization need not uniquely determine $T_s$.

Finally, locate the derived $T_s$ and [luminosity](../../../../../luminosity.md) on the [Hertzsprung-Russell diagram](../../../../../hertzsprung-russell-diagram.md). The central stars are hot exposed cores following [post-asymptotic giant branch evolution](../../../../../post-asymptotic-giant-branch-evolution.md): envelope loss creates the [planetary nebula](../../../../../planetary-nebula.md), contraction heats the core, and continued shell burning can support an approximately constant [luminosity](../../../../../luminosity.md) as the star moves leftward. Later the [luminosity](../../../../../luminosity.md) falls and the remnant approaches the [white dwarf](../../../../../white-dwarf.md) cooling sequence. Comparing central-star positions with [stellar evolution](../../../../../stellar-evolution.md) tracks constrains core masses and evolutionary ages; comparison with nebular expansion ages tests whether the core heats rapidly enough to ionize the expelled envelope. **The central-star locus traces the transition from an envelope-losing giant to a compact stellar remnant.**

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
