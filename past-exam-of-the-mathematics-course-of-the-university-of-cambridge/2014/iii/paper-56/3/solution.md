<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Near the accretor assume fully ionized hydrogen, tight electric coupling between protons and electrons, isotropic radiation and opacity dominated by [Thomson scattering](../../../../../thomson-scattering.md). The gravitational force on an electron–proton pair is approximately $GMm_p/r^2$; the outward [radiation pressure](../../../../../radiation-pressure.md) force is $\sigma_TL/(4\pi r^2c)$. Balancing them gives the [Eddington luminosity](../../../../../eddington-luminosity.md)

$$
\boxed{L_E=\frac{4\pi GMm_pc}{\sigma_T}.}
$$

Writing $L=\epsilon_r\dot M_{\rm in}c^2$ defines the [radiative efficiency of black-hole accretion](../../../../../radiative-efficiency-of-black-hole-accretion.md). In the approximation that the radiated rest-mass fraction is ignored in the mass bookkeeping, $\dot M\simeq\dot M_{\rm in}$, so at the [Eddington accretion rate](../../../../../eddington-accretion-rate.md)

$$
\frac{dM}{dt}\simeq\frac{4\pi Gm_p}{\epsilon_r c\sigma_T}M,
\qquad
\boxed{M(t)=M_0e^{t/\tau},\quad \tau\simeq\epsilon_r\frac{c\sigma_T}{4\pi Gm_p}.}
$$

This is the printed approximate [Salpeter time](../../../../../salpeter-time.md); $\tau\simeq4.5\times10^7\,\mathrm{yr}$ for the adopted efficiency. More exactly $\dot M=(1-\epsilon_r)\dot M_{\rm in}$, giving $\tau=\epsilon_r t_E/(1-\epsilon_r)$ with $t_E=c\sigma_T/(4\pi Gm_p)\simeq4.5\times10^8\,\mathrm{yr}$. The difference is a ten-percent-level convention here, not a change from exponential growth. Continuous fuelling, constant efficiency and unit [Eddington ratio](../../../../../eddington-ratio.md) are additional idealizations.

Next normalize the ionizing spectrum rather than replacing every photon by a threshold photon. For $L_\nu=A\nu^{-2}$ above $\nu_0$,

$$
L_{\rm ion}=\int_{\nu_0}^\infty L_\nu\,d\nu=\frac A{\nu_0},\qquad
Q_H=\int_{\nu_0}^\infty\frac{L_\nu}{h_P\nu}\,d\nu=\frac A{2h_P\nu_0^2}.
$$

Here $h_P$ is Planck's constant, distinct from the cosmological $h$. The [mean ionizing photon energy of a power-law spectrum](../../../../../mean-ionizing-photon-energy-of-a-power-law-spectrum.md) is therefore $\langle E\rangle=L_{\rm ion}/Q_H=2E_0=27.2\,\mathrm{eV}$. With ionizing luminosity fraction $f_{\rm ion}=0.30$, the [hydrogen-ionizing photon production rate](../../../../../hydrogen-ionizing-photon-production-rate.md) is $Q_H=f_{\rm ion}L_E/(2E_0)$.

Assume a sharp spherical [ionization front](../../../../../ionization-front.md), homogeneous initially neutral hydrogen at the cosmic mean baryon density, escape fraction one, one primary ionization per photon, and no recombinations or secondary ionizations. The [ionization-front growth from an exponentially brightening source](../../../../../ionization-front-growth-from-an-exponentially-brightening-source.md) is then fixed by photon conservation. In the printed approximate mass convention,

$$
N_\gamma(t)=\frac{f_{\rm ion}\epsilon_rc^2}{2E_0}\,[M(t)-M_0].
$$

Take the stated separation to be a proper separation at the seed-formation epoch, and take the distant halo to follow the expansion on this large scale. Its initial separation $R_i$ defines a fixed comoving radius $X=R_i(1+z_i)$. The number of hydrogen nuclei initially within that radius is

$$
N_H=\frac{M_H}{m_p},\qquad
M_H=\frac{4\pi}3R_i^3\Omega_b\rho_{\rm crit,0}(1+z_i)^3.
$$

Although the proper density subsequently falls, this comoving hydrogen inventory is constant. Thus the photon count does not require freezing the expansion for the entire growth interval.

The supplied [critical density](../../../../../critical-density.md) gives $\Omega_b\rho_{\rm crit,0}=6.86\times10^9M_\odot\,\mathrm{Mpc}^{-3}$, so $M_H\simeq2.87\times10^{13}M_\odot$ for the initial proper-distance interpretation. Equating $N_\gamma=N_H$ requires

$$
\Delta M= M_H\frac{2E_0}{f_{\rm ion}\epsilon_rm_pc^2}
\simeq2.78\times10^7M_\odot,
$$

and therefore

$$
\boxed{t_{\rm front}=\tau\log\left(1+\frac{\Delta M}{M_0}\right)
\simeq6.68\times10^8\,\mathrm{yr}.}
$$

Light propagation adds a retarded-time correction of order a few million years, small compared with this growth time; it should not be replaced by instantaneous propagation when modelling the very early front. Expansion increases the proper distance to the comoving halo during the wait, but not the required comoving photon inventory. If the unspecified distance is instead a comoving distance, the inventory is smaller by $10^3$ and the corresponding answer is **$t_{\rm front}\simeq3.57\times10^8\,\mathrm{yr}$**. A distance held at a fixed proper radius until arrival would need a different evolving-volume treatment.

Using exact rest-mass bookkeeping changes $N_\gamma$ to $f_{\rm ion}\epsilon_rc^2\Delta M/[2E_0(1-\epsilon_r)]$ and $\tau$ to $5.0\times10^7\,\mathrm{yr}$. The proper-at-formation case then gives about **$7.37\times10^8\,\mathrm{yr}$**, and the comoving-distance case about $3.91\times10^8\,\mathrm{yr}$. These modest changes are smaller than the uncertainties of the sharp-front, no-recombination model. In particular real absorption of the high-energy tail, secondary electrons and a nonunit escape fraction would require radiative-transfer corrections.

The small halo initially holds cool gas in [hydrostatic equilibrium](../../../../../hydrostatic-equilibrium.md). [Photoionization](../../../../../photoionization.md) deposits energy far above its virial binding scale. With the emitted mean energy, the excess per primary ionization is $13.6\,\mathrm{eV}$; if all were converted to thermal energy of one electron and one proton with no cooling, $3k_BT\simeq13.6\,\mathrm{eV}$ would give about $5\times10^4\,\mathrm K$. Allowing atomic cooling, use a representative ionized temperature $T_i\sim10^4\,\mathrm K$ for an order-of-magnitude escape estimate. Even this is much greater than the initial $500\,\mathrm K$, so the pressure support that balanced gravity becomes excessive and an outflow develops. **The baryons are photoheated and undergo [photoevaporation of a dark-matter minihalo](../../../../../photoevaporation-of-a-dark-matter-minihalo.md); the shallow halo loses much of its gas and its future [star formation](../../../../../star-formation.md) is suppressed.**

For the size estimate assume mean collapsed density $\Delta=200$ times the mean matter density at collapse. Its [virial radius of a dark-matter halo](../../../../../virial-radius-of-a-dark-matter-halo.md) is

$$
R_h=\left[\frac{3M_h}{4\pi\Delta\Omega_m\rho_{\rm crit,0}(1+z_{\rm coll})^3}\right]^{1/3}
\simeq1.91\times10^{-4}\,\mathrm{Mpc}=191\,\mathrm{pc}.
$$

This is an order-of-magnitude virial convention, not an exact conversion of the approximate quoted temperature: different factors in the [virial temperature](../../../../../virial-temperature.md) definition give comparable radii near $10^2\,\mathrm{pc}$. Keep the radius of the bound halo fixed after its stated collapse, rather than rescaling it with the later cosmic mean density. Fully ionized pure hydrogen has [mean molecular weight](../../../../../mean-molecular-weight.md) $\mu_i=1/2$. With monatomic $\gamma=5/3$, its [adiabatic sound speed](../../../../../adiabatic-sound-speed.md) is

$$
c_s=\sqrt{\frac{\gamma k_BT_i}{\mu_im_p}}\simeq16.6\,\mathrm{km\,s^{-1}}.
$$

This exceeds the virial escape-speed scale $\sqrt{2GM_h/R_h}\simeq3.0\,\mathrm{km\,s^{-1}}$. A sound-crossing outflow estimate gives

$$
\boxed{t_{\rm evap}\sim\frac{R_h}{c_s}\simeq1.1\times10^7\,\mathrm{yr},}
$$

measured after the [ionization front](../../../../../ionization-front.md) arrives. Using an isothermal [sound speed](../../../../../speed-of-sound.md), a different virial factor or a hotter post-front gas changes this by factors of order unity. It is not a second hundreds-of-millions-of-years black-hole growth interval.

The crossing-time estimate assumes the relevant gas can be ionized without a long trapped-front delay. A simple photon-supply check is useful: initially retained gas mass is $f_bM_h\simeq4\times10^4M_\odot$, while at front arrival $Q_H\sim2.4\times10^{55}\,\mathrm{s^{-1}}$. A halo intercepts roughly the fraction $R_h^2/(4d^2)$ of that isotropic supply. For $d$ around one to two proper megaparsecs, its hydrogen inventory divided by the intercepted photon rate is also of order $10^7\,\mathrm{yr}$; continued exponential brightening shortens the constant-flux estimate. Thus a gas-loss estimate of **one to a few $10^7\,\mathrm{yr}$** is justified in the idealized model. A detailed evaporation time is not uniquely determined without the gas profile, post-ionization temperature and shielding; retained recombinations would further delay a front in dense gas.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
