<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

At [neutrino decoupling](../../../../../neutrino-decoupling.md), the interaction rate is comparable with the [Hubble parameter](../../../../../hubble-parameter.md). Equating the supplied rates gives

$$
G_F^2T_D^5=\frac{1.66\sqrt{g_*}T_D^2}{m_P},\qquad
\boxed{T_D=\left(\frac{1.66\sqrt{g_*}}{G_F^2m_P}\right)^{1/3}\simeq1.6\,\mathrm{MeV}.}
$$

Here the [Planck mass](../../../../../planck-mass.md) is the unreduced $m_P=G^{-1/2}\simeq1.22\times10^{19}\,\mathrm{GeV}$ in [natural units](../../../../../natural-units.md), $G_F\simeq10^{-5}\,\mathrm{GeV}^{-2}$, and the [effective number of relativistic energy degrees of freedom](../../../../../effective-number-of-relativistic-energy-degrees-of-freedom.md) is $g_*=10.75$. The supplied rate gives an order-of-magnitude [neutrino decoupling](../../../../../neutrino-decoupling.md) estimate; a precise neutron-proton conversion temperature uses its own weak-rate coefficients.

The [chemical equilibrium](../../../../../chemical-equilibrium.md) condition for $n+\nu_e\leftrightarrow p+e^-$ is $\mu_n+\mu_{\nu_e}=\mu_p+\mu_e$. With negligible lepton [chemical potentials](../../../../../chemical-potential.md), $\mu_n=\mu_p$. The [nonrelativistic Maxwell--Boltzmann number density](../../../../../nonrelativistic-maxwell-boltzmann-number-density.md) therefore gives

$$
\frac{n_n}{n_p}=\frac{g_n}{g_p}\left(\frac{m_n}{m_p}\right)^{3/2}e^{-(m_n-m_p)/T}
\simeq\boxed{e^{-Q/T}=\frac{X_n}{X_p}},
$$

because $g_n=g_p=2$ and the small mass difference can be neglected in the prefactor. This is the [neutron-proton chemical equilibrium](../../../../../neutron-proton-chemical-equilibrium.md) relation.

For the [deuterium equilibrium abundance](../../../../../deuterium-equilibrium-abundance.md), $\mu_D=\mu_n+\mu_p$ because photons have zero [chemical potential](../../../../../chemical-potential.md). The sign convention in the paper is important: $B=m_D-m_n-m_p<0$, while the positive [nuclear binding energy](../../../../../nuclear-binding-energy.md) is $\Delta_D=-B$. Using spin multiplicities $g_D=3$, $g_n=g_p=2$ gives

$$
\frac{n_D}{n_nn_p}=\frac34\left(\frac{2\pi m_D}{m_nm_pT}\right)^{3/2}e^{-B/T}.
$$

With $n_B=\eta n_\gamma$, $m_n\simeq m_p\simeq m_N$, $m_D\simeq2m_N$ and [photon number density](../../../../../photon-number-density.md) $n_\gamma=2\zeta(3)T^3/\pi^2$, this becomes

$$
\boxed{X_D\simeq\frac{12\zeta(3)}{\sqrt\pi}\,\eta X_nX_p\left(\frac{T}{m_N}\right)^{3/2}e^{-B/T}.}
$$

Here $X_D=n_D/n_B$ is a number fraction; the fraction of baryons bound in [deuterium](../../../../../deuterium.md) is $2X_D$. The formula estimates the onset of the [deuterium bottleneck](../../../../../deuterium-bottleneck.md) opening while depletion of free [neutrons](../../../../../neutron.md) and [protons](../../../../../proton.md) remains small. Because $\eta\ll1$, stable [deuterium](../../../../../deuterium.md) becomes abundant only far below the positive [nuclear binding energy](../../../../../nuclear-binding-energy.md), not simply at $T=\Delta_D$.

Let $T_f$ denote [cosmological weak freeze-out](../../../../../cosmological-weak-freeze-out.md) of the [neutron-to-proton ratio](../../../../../neutron-to-proton-ratio.md), $r_f=e^{-Q/T_f}$, and let $t_N$ mark efficient nuclear burning. [Free-neutron decay after freeze-out](../../../../../free-neutron-decay-after-freeze-out.md) gives

$$
X_n(t_N)\simeq\frac{r_f}{1+r_f}e^{-(t_N-t_f)/\tau_n},\qquad\tau_n=\frac{t_{1/2}}{\log2}.
$$

Almost every surviving [neutron](../../../../../neutron.md) enters helium-4, whose [atomic nucleus](../../../../../atomic-nucleus.md) contains two [neutrons](../../../../../neutron.md) and four baryons. Thus [neutron-limited helium synthesis](../../../../../neutron-limited-helium-synthesis.md) gives

$$
\boxed{Y_p\simeq2X_n(t_N)=\frac{2r_f}{1+r_f}e^{-(t_N-t_f)/\tau_n}.}
$$

A longer neutron [half-life](../../../../../half-life.md) leaves more [neutrons](../../../../../neutron.md) available, increasing the [primordial helium mass fraction](../../../../../primordial-helium-mass-fraction.md). If the longer lifetime reflects weaker [weak interactions](../../../../../weak-interaction.md), the accompanying earlier [cosmological weak freeze-out](../../../../../cosmological-weak-freeze-out.md) can reinforce that effect.

During [radiation domination](../../../../../radiation-domination.md), $H\propto\sqrt{Gg_*}\,T^2$ whereas the weak conversion rate is proportional to $T^5$. Hence $T_f\propto(Gg_*)^{1/6}$. Increasing the [effective number of relativistic energy degrees of freedom](../../../../../effective-number-of-relativistic-energy-degrees-of-freedom.md) raises $T_f$, increasing $r_f$, and shortens the interval for [free-neutron decay after freeze-out](../../../../../free-neutron-decay-after-freeze-out.md). Both increase the [primordial helium mass fraction](../../../../../primordial-helium-mass-fraction.md) while nuclear burning remains efficient. The same reasoning gives the [primordial helium response to a varying gravitational constant](../../../../../primordial-helium-response-to-a-varying-gravitational-constant.md): larger $G$ over this interval produces more helium, with fixed microscopic rates and the approximate [Friedmann equation](../../../../../friedmann-equations.md) unchanged. Smaller $G$ has the opposite effect. A particular varying-$G$ model must specify its background expansion and time history; the simple trend must not be extrapolated to changes so large that nuclear burning itself fails.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 55](../../paper-55-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
