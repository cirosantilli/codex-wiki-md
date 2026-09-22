<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

**Two stages of the thermal history.** [Big Bang nucleosynthesis](../../../big-bang-nucleosynthesis.md) is nuclear assembly in an almost fully ionized, radiation-dominated plasma. Around $t\sim1\ \mathrm s$, at [temperatures](../../../temperature-split.md) of order $1\ \mathrm{MeV}/k_B$, the weak [neutron](../../../neutron-split.md)–[proton](../../../proton.md) conversion rate falls below the expansion rate. The neutron-to-proton abundance freezes out at order $1/5$ and then decreases by [neutron](../../../neutron-split.md) decay. The [deuterium bottleneck](../../../deuterium-bottleneck.md) delays effective nuclear assembly until $k_BT\sim0.07$–$0.1\ \mathrm{MeV}$, at ages of a few minutes: the high photon-to-baryon ratio permits photodissociation despite the deuteron binding energy exceeding the mean [photon energy](../../../photon-energy.md). Once deuterium survives, reactions rapidly put most remaining [neutrons](../../../neutron-split.md) into helium-4. A [neutron-to-proton ratio](../../../neutron-to-proton-ratio.md) near $1/7$ gives a [helium](../../../helium.md) mass fraction $Y_p\simeq2(n/p)/(1+n/p)\simeq1/4$, with [hydrogen](../../../hydrogen.md) dominant by number and small residual deuterium, helium-3 and lithium-7 abundances. Expansion and low density prevent substantial heavy-element production. Nuclear binding is involved; neutral atoms do not yet survive.

[Photon decoupling](../../../photon-decoupling.md) occurs much later, near a few thousand kelvin and a few hundred thousand years, after matter has overtaken radiation in the expansion dynamics. [Electrons](../../../electron.md) and nuclei form neutral atoms during [cosmological recombination](../../../recombination-cosmology.md). The resulting decline of free-electron density reduces Thomson opacity, and [photons](../../../photon.md) begin to free stream over cosmological distances. Those [photons](../../../photon.md) form the observed [cosmic microwave background](../../../cosmic-microwave-background-split.md). Atomic binding and scattering opacity, rather than new nuclear reactions, control this stage. [Helium](../../../helium.md) forms neutral atoms earlier than [hydrogen](../../../hydrogen.md). Recombination, [photon](../../../photon.md) last scattering, [baryon](../../../baryon.md) drag release and the later thermal decoupling of the gas are related but not identical events.

The [temperature](../../../temperature-split.md) falls through expansion: after the relevant entropy releases have ended, $T_\gamma\propto a^{-1}$ and number densities scale as $a^{-3}$. Big Bang nucleosynthesis lies in the [radiation-dominated universe](../../../radiation-dominated-universe.md); [photon decoupling](../../../photon-decoupling.md) lies after matter–radiation equality, when a matter-dominated approximation is useful but radiation is not exactly negligible.

**[Photon](../../../photon.md) density and [baryon](../../../baryon.md) abundance.** The [cosmic microwave background](../../../cosmic-microwave-background-split.md) has a [black-body radiation](../../../black-body-radiation.md) spectrum obeying [Planck's law](../../../planck-s-law.md):

$$
u_\nu=\frac{8\pi h\nu^3}{c^3}\frac1{e^{h\nu/(k_BT)}-1},\qquad T_0\simeq2.725\ \mathrm K,
$$

where $u_\nu$ is spectral energy density, not a photon-number density. The measured [temperature](../../../temperature-split.md) is about $2.72548\ \mathrm K$.[Abstract: literature-combined black-body [temperature](../../../temperature-split.md), 2.72548 ± 0.00057 K](../../../the-temperature-of-the-cosmic-microwave-background-by-dale-j-fixsen.md) The mean [photon energy](../../../photon-energy.md) in a black body is

$$
\langle E_\gamma\rangle=\frac{\pi^4}{30\zeta(3)}k_BT\simeq2.701k_BT.
$$

Using the supplied rounded energy density gives

$$
\boxed{n_{\gamma0}\simeq\frac{4\times10^{-14}}{2.701k_BT_0}\simeq3.9\times10^8\ \mathrm{m^{-3}}}.
$$

The exact black-body number integral at $2.725\ \mathrm K$ gives $4.1\times10^8\ \mathrm{m^{-3}}$; the difference reflects rounding of the stated energy density. Either estimate is adequate.

A numerical photon-to-baryon ratio additionally needs a [baryon](../../../baryon.md) density, which is not printed in this question. Make that observational input explicit rather than infer [baryons](../../../baryon.md) from radiation alone. For illustration take the standard rounded physical density $\Omega_bh_H^2\simeq0.022$, with $H_0=100h_H\ \mathrm{km\,s^{-1}\,Mpc^{-1}}$. This is consistent with the cosmological parameter fits available around the paper's date.[Base ΛCDM parameter tables: physical [baryon](../../../baryon.md) density near 0.022; illustrative expansion normalization H0 about 68 km s−1 Mpc−1 and matter fraction about 0.31](../../../planck-2015-cosmological-parameters-by-planck-collaboration.md) It gives

$$
\rho_{b0}=(\Omega_bh_H^2)\frac{3(100\ \mathrm{km\,s^{-1}\,Mpc^{-1}})^2}{8\pi G}\simeq4.1\times10^{-28}\ \mathrm{kg\,m^{-3}},\qquad n_{b0}\simeq\frac{\rho_{b0}}{m_p}\simeq0.25\ \mathrm{m^{-3}}.
$$

Counting [baryons](../../../baryon.md), including those bound in [helium](../../../helium.md), rather than counting nuclei then gives

$$
\boxed{\frac{n_\gamma}{n_b}\sim1.6\times10^9,\qquad \eta\equiv\frac{n_b}{n_\gamma}\sim6\times10^{-10}}.
$$

Both populations dilute as $a^{-3}$ after [electron](../../../electron.md)–positron annihilation, so this ratio also applies at [hydrogen](../../../hydrogen.md) recombination in the standard adiabatic history.

**Estimating decoupling.** The large [photon](../../../photon.md) excess explains why setting $k_BT$ equal to the [Hydrogen binding energy](../../../hydrogen-binding-energy.md) $\chi_H=13.6\ \mathrm{eV}$ is wrong. Even a small ionizing tail can oppose neutral-atom formation. The crude exponential balance $e^{-\chi_H/(k_BT)}\sim\eta$ gives $\chi_H/(k_BT)\sim\ln(1/\eta)\sim21$, or $T\sim7\times10^3\ \mathrm K$. This only establishes the scale and the large suppression below $\chi_H/k_B$; it neglects phase-space factors and the opacity criterion.

A more controlled elementary [Saha-Thomson decoupling estimate](../../../saha-thomson-decoupling-estimate.md) uses the [hydrogen-only Saha equation](../../../hydrogen-only-saha-equation.md). With $X_e=n_e/n_H$ and ground-state statistical weights combined in the usual way,

$$
\frac{X_e^2}{1-X_e}=\frac1{n_H}\left(\frac{2\pi m_ek_BT}{h^2}\right)^{3/2}e^{-\chi_H/(k_BT)},\qquad
n_H\simeq(1-Y_p)n_{b0}\left(\frac T{T_0}\right)^3.
$$

The [electron](../../../electron.md) translational phase-space factor is significant inside the logarithm. This equilibrium relation places the sharp neutralization interval around $T\sim(3\text{–}4)\times10^3\ \mathrm K$. Combine it with the approximate [Thomson decoupling rate criterion](../../../thomson-decoupling-rate-criterion.md)

$$
\Gamma_\gamma=n_e\sigma_Tc\sim H,\qquad
H\simeq H_0\sqrt{\Omega_m}\left(\frac T{T_0}\right)^{3/2}.
$$

For $Y_p\simeq0.25$, $n_{b0}\simeq0.25\ \mathrm{m^{-3}}$, $H_0\simeq68\ \mathrm{km\,s^{-1}\,Mpc^{-1}}$, and $\Omega_m\simeq0.31$, solving these two approximate relations gives $T\simeq3.1\times10^3\ \mathrm K$, with equilibrium $X_e$ of order $10^{-2}$. Thus the appropriate estimate is

$$
\boxed{T_{\rm dec}\sim3\times10^3\ \mathrm K,\qquad k_BT_{\rm dec}\sim0.26\ \mathrm{eV},\qquad z_{\rm dec}\sim1100}.
$$

This is not a precision recombination calculation. Hydrogen-only equilibrium omits the kinetic bottleneck in escaping Lyman [photons](../../../photon.md), two-photon processes, the detailed [helium](../../../helium.md) history and freeze-out; $\Gamma/H\sim1$ is not identical to the maximum of the last-scattering visibility function. These approximations must be improved to predict an accurate free-electron fraction or a percent-level last-scattering redshift. The high photon-to-baryon ratio alone does not fix that detailed history.

The [electrons](../../../electron.md) are highly nonrelativistic: $k_BT/(m_ec^2)\sim5\times10^{-7}$, and their thermal root-mean-square speed is only about $10^{-3}c$. [Photon](../../../photon.md) coupling does not make their kinetic energies relativistic.

**Age–[temperature](../../../temperature-split.md) relation.** During a nearly flat pressureless matter-dominated phase, with radiation, curvature and vacuum energy neglected in the expansion equation,

$$
\rho_m\propto a^{-3},\qquad \left(\frac{\dot a}a\right)^2\propto a^{-3},\qquad \boxed{a(t)\propto t^{2/3}}.
$$

Here the Big Bang time is chosen as $t=0$. Conserved [photon](../../../photon.md) entropy gives $T\propto a^{-1}$, so

$$
\boxed{T\propto t^{-2/3},\qquad t\propto T^{-3/2}}.
$$

To normalize this relation, use the matter-era expansion rate expressed in present-day measured parameters, rather than assume the late universe is still matter dominated:

$$
\boxed{t(T)\simeq\frac{2}{3H_0\sqrt{\Omega_m}}\left(\frac{T_0}T\right)^{3/2}}.
$$

The same illustrative parameters give $t_{\rm dec}\sim4.5\text{–}5\times10^5\ \mathrm{yr}$ for $T_{\rm dec}\sim3.0\text{–}3.1\times10^3\ \mathrm K$. Radiation was still a meaningful correction; retaining it reduces the age, and a more complete recombination calculation gives the familiar scale of roughly $4\times10^5\ \mathrm{yr}$.[§6.7: recombination and [photon decoupling](../../../photon-decoupling.md) near redshift 10^3, at an age around 400000 years; distinction from detailed kinetic ionization-history calculations](../../../planck-2015-cosmological-parameters-by-planck-collaboration.md) A numerical age cannot follow from a proportionality $t\propto T^{-3/2}$ alone: an expansion or density normalization is essential. The small amount of dark energy at decoupling can be neglected even though it affects the present age.

## ↑ Ancestors (11)

1. [4](../4.md)
2. [2016](../../2016-split.md)
3. [Past exam of the general relativity and cosmology course of the University of Oxford](../../split.md)
4. [General relativity and cosmology course of the University of Oxford](../../../general-relativity-and-cosmology-course-of-the-university-of-oxford.md)
5. [Year 3 of the physics course of the University of Oxford](../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
