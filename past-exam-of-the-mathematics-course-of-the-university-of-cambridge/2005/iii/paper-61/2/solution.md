<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use [natural units](../../../../../natural-units.md) $\hbar=c=k_B=1$ and the unreduced [Planck mass](../../../../../planck-mass.md) $M_P=G^{-1/2}$. [Neutrino decoupling](../../../../../neutrino-decoupling.md) occurs when the [weak interaction](../../../../../weak-interaction.md) rate falls below the [Hubble parameter](../../../../../hubble-parameter.md). The [weak-decoupling temperature estimate](../../../../../weak-decoupling-temperature-estimate.md) equates the given rate with the radiation-era expansion rate:

$$
G_F^2T_d^5\simeq1.66\sqrt{g_*}\frac{T_d^2}{M_P},\qquad \boxed{T_d\simeq\left(\frac{1.66\sqrt{g_*}}{G_F^2M_P}\right)^{1/3}\simeq1.8\ {\rm MeV}.}
$$

Here $g_*$ counts the [effective number of relativistic energy degrees of freedom](../../../../../effective-number-of-relativistic-energy-degrees-of-freedom.md), and the [Fermi constant](../../../../../fermi-constant.md) is $G_F\simeq10^{-5}\ {\rm GeV}^{-2}$. The omitted reaction-rate coefficients make this an order-of-magnitude estimate: **decoupling occurs at a temperature of order one MeV**.

The charge-conserving channel is $n+\nu_e\leftrightarrow p+e^-$, together with $p+\bar\nu_e\leftrightarrow n+e^+$. The positron sign in the printed neutron-capture channel violates [electric charge conservation](../../../../../charge-conservation.md). [Chemical equilibrium](../../../../../chemical-equilibrium.md) requires $\mu_n+\mu_{\nu_e}=\mu_p+\mu_e$. Negligible lepton [chemical potentials](../../../../../chemical-potential.md) therefore give $\mu_n\simeq\mu_p$. Since [neutrons](../../../../../neutron.md) and [protons](../../../../../proton.md) are [nonrelativistic particles](../../../../../nonrelativistic-particle.md), their [Maxwell-Boltzmann distribution](../../../../../maxwell-boltzmann-distribution.md) gives

$$
n_i=g_i\left(\frac{m_iT}{2\pi}\right)^{3/2}e^{(\mu_i-m_i)/T},\qquad \frac{n_n}{n_p}=\frac{g_n}{g_p}\left(\frac{m_n}{m_p}\right)^{3/2}e^{-(m_n-m_p)/T}.
$$

Both nucleons have two spin states, and their masses agree closely in the prefactor. Thus [neutron-proton chemical equilibrium](../../../../../neutron-proton-chemical-equilibrium.md) implies

$$
\boxed{\frac{n_n}{n_p}=\frac{X_n}{X_p}\simeq e^{-Q/T_d},\qquad Q=m_n-m_p>0.}
$$

The heavier [neutron](../../../../../neutron.md) is suppressed by a [Boltzmann factor](../../../../../boltzmann-factor.md).

For the [deuterium equilibrium abundance](../../../../../deuterium-equilibrium-abundance.md), retain the paper's convention $B=m_D-m_n-m_p<0$; the positive [nuclear binding energy](../../../../../nuclear-binding-energy.md) is $\varepsilon_D=-B\simeq2.22\ {\rm MeV}$. [Chemical equilibrium](../../../../../chemical-equilibrium.md) of $n+p\leftrightarrow D+\gamma$ gives $\mu_D=\mu_n+\mu_p$ because the equilibrium [photon](../../../../../photon.md) [chemical potential](../../../../../chemical-potential.md) vanishes. Using the [nonrelativistic Maxwell--Boltzmann number density](../../../../../nonrelativistic-maxwell-boltzmann-number-density.md) for each species and dividing gives

$$
\frac{n_D}{n_nn_p}=\frac{g_D}{g_ng_p}\left(\frac{m_D}{m_nm_p}\right)^{3/2}\left(\frac{2\pi}{T}\right)^{3/2}e^{-B/T}.
$$

Here $g_D=3$ and $g_n=g_p=2$. With the [baryon-to-photon ratio](../../../../../baryon-to-photon-ratio.md) $\eta=n_B/n_\gamma$, the [photon number density](../../../../../photon-number-density.md) $n_\gamma=2\zeta(3)T^3/\pi^2$, and $m_D\simeq2m_N$, $m_n\simeq m_p\simeq m_N$, this becomes

$$
\boxed{\frac{X_D}{X_nX_p}\simeq\frac{12\zeta(3)}{\sqrt\pi}\,\eta\left(\frac{T}{m_N}\right)^{3/2}e^{-B/T}\simeq8.14\,\eta\left(\frac{T}{m_N}\right)^{3/2}e^{\varepsilon_D/T}.}
$$

In this convention $X_D=n_D/n_B$ counts nuclei, so its contribution to the fraction of baryons in [deuterium](../../../../../deuterium.md) is $2X_D$.

The [deuterium bottleneck](../../../../../deuterium-bottleneck.md) explains why [helium-4](../../../../../helium-4.md) formation waits until $T$ is far below $\varepsilon_D$. At higher [temperature](../../../../../temperature.md), there are vastly more [photons](../../../../../photon.md) than baryons; even the dilute energetic tail can destroy newly formed [deuterium](../../../../../deuterium.md). A crude estimate balances $\eta^{-1}e^{-\varepsilon_D/T}$ against one, giving $T\sim\varepsilon_D/\log(\eta^{-1})\sim0.1\ {\rm MeV}$ for $\eta$ of order $10^{-9}$. The power-law factors in the [deuterium equilibrium abundance](../../../../../deuterium-equilibrium-abundance.md) and the nuclear reaction rates refine this estimate. Once stable [deuterium](../../../../../deuterium.md) accumulates, further reactions can efficiently place nearly all surviving [neutrons](../../../../../neutron.md) into [helium-4](../../../../../helium-4.md).

Write $r_N=n_n/n_p$ at the onset of nuclear burning. Each [helium-4](../../../../../helium-4.md) nucleus requires two [neutrons](../../../../../neutron.md) and contains four baryons. [Neutron-limited helium synthesis](../../../../../neutron-limited-helium-synthesis.md) therefore gives the [primordial helium mass fraction](../../../../../primordial-helium-mass-fraction.md)

$$
\boxed{Y_4\simeq\frac{4n_{\rm He}}{n_B}\simeq2X_n(T_N)=\frac{2r_N}{1+r_N}.}
$$

For a realistic rough [cosmological weak freeze-out](../../../../../cosmological-weak-freeze-out.md) estimate, $r_f$ is about $1/6$ and [free-neutron decay after freeze-out](../../../../../free-neutron-decay-after-freeze-out.md) reduces it to about $1/7$, giving **roughly one quarter of the baryonic mass in helium-4**. The survival relation that conserves [baryon number](../../../../../baryon-number.md) is $X_n(T_N)=r_f(1+r_f)^{-1}e^{-\Delta t/\tau_n}$; the corresponding $r_N$ is $X_n/(1-X_n)$.

The rough [neutrino decoupling](../../../../../neutrino-decoupling.md) rate by itself does not determine that one-quarter value. Substituting $T_d=1.8\ {\rm MeV}$ literally into $e^{-Q/T_d}$ would give $r\simeq0.49$ and $Y_4\simeq0.65$ before neutron decay. [Neutron-proton chemical equilibrium](../../../../../neutron-proton-chemical-equilibrium.md) persists to a lower temperature, approximately $0.7$--$0.8\ {\rm MeV}$ once the actual conversion rates are included. The rate scaling fixes the MeV scale; accurate abundances need the conversion coefficients and the delay through the [deuterium bottleneck](../../../../../deuterium-bottleneck.md). This sequence is described in [David Tong's discussion of nucleosynthesis](https://www.davidtong.org/teaching/cosmology/cosmohtml/S2#S2.SS5.SSS3).

Increasing $Q$ reduces the equilibrium [neutron-to-proton ratio](../../../../../neutron-to-proton-ratio.md), so **the primordial helium abundance decreases**. Holding the freeze-out temperature $T_f$ and the decay survival factor fixed, the [primordial helium response to the neutron-proton mass difference](../../../../../primordial-helium-response-to-the-neutron-proton-mass-difference.md) is

$$
\boxed{\frac{Y_4(1.1Q)}{Y_4(Q)}\simeq\frac{1+e^{Q/T_f}}{1+e^{1.1Q/T_f}}.}
$$

For $Q\simeq1.29\ {\rm MeV}$ and $T_f=0.7$--$0.8\ {\rm MeV}$ this is about $0.85$--$0.87$, a reduction of roughly fifteen percent. A larger $Q$ also changes neutron decay and detailed weak rates; their quantitative effects require more microscopic information. The sign from the [Boltzmann factor](../../../../../boltzmann-factor.md) is already clear.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 61](../../paper-61-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
