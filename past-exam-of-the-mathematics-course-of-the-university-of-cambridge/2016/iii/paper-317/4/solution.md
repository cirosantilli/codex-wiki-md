<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For a slowly evolving spherical star, use a Lagrangian [enclosed mass](../../../../../enclosed-mass.md) coordinate $m$. Let $u$ be specific thermal internal energy and $D/Dt$ follow a mass element. The [stellar energy balance equation](../../../../../stellar-energy-balance-equation.md) is

$$
\boxed{\frac{\partial L}{\partial m}
=\epsilon_{\rm nuc}-\epsilon_\nu-\frac{Du}{Dt}
-P\frac{D}{Dt}\left(\frac1\rho\right)
=\epsilon_{\rm nuc}-\epsilon_\nu+\epsilon_{\rm grav}.}
$$

The outward [luminosity](../../../../../luminosity.md) is energy transported through the mass shell, $\epsilon_{\rm nuc}$ is nuclear rest-mass energy released per unit mass and time, and $\epsilon_\nu$ is escaping [neutrino](../../../../../neutrino.md) power per unit mass. Define the [gravothermal stellar energy generation](../../../../../gravothermal-stellar-energy-generation.md) by $\epsilon_{\rm grav}=-Du/Dt-PD(1/\rho)/Dt$. At fixed composition it is $-TDS/Dt$ by the [first law of thermodynamics](../../../../../first-law-of-thermodynamics.md). During composition changes the full internal-energy derivative must use the appropriate equation of state, with nuclear rest-mass changes counted only once. If a tabulated nuclear rate already subtracts reaction-neutrino energy, that loss must not be subtracted a second time in $\epsilon_\nu$.

In a nearly steady [main sequence](../../../../../main-sequence.md) star, [stellar nuclear fusion](../../../../../stellar-nuclear-fusion.md) supplies most of the [luminosity](../../../../../luminosity.md). Before stable hydrogen ignition, [Kelvin-Helmholtz contraction](../../../../../kelvin-helmholtz-mechanism.md) releases gravitational energy. In a gas-supported hydrostatic star the [stellar virial theorem](../../../../../stellar-virial-theorem.md) gives $U\simeq-\Omega/2$, so about half the change in gravitational binding energy heats the star and half is available for radiation. The associated timescale is $GM^2/(RL)$. After nuclear burning ends, a [white dwarf](../../../../../white-dwarf.md) can shine by losing stored thermal energy; crystallization releases latent heat, and composition separation can add gravitational energy. These are heat and gravitational reservoirs rather than sustained hydrogen fusion.

[Stellar nuclear fusion](../../../../../stellar-nuclear-fusion.md) is possible because lighter nuclei can combine into products with larger [nuclear binding energy](../../../../../nuclear-binding-energy.md). The energy per reaction is $Q=(m_{\rm initial}-m_{\rm final})c^2$, including the relevant particles consistently. Although thermal energies are below the [Coulomb barrier](../../../../../coulomb-barrier.md), [quantum tunnelling](../../../../../quantum-tunnelling.md) permits fusion. The [thermonuclear reaction rate](../../../../../thermonuclear-reaction-rate.md) averages a cross-section over the thermal relative-speed distribution:

$$
r_{12}=\frac{n_1n_2}{1+\delta_{12}}\langle\sigma v\rangle,\qquad
\epsilon_{12}=\frac{r_{12}Q_{\rm deposited}}\rho.
$$

For nonresonant charged-particle reactions the energy weighting contains $\exp[-E/(kT)-\sqrt{E_G/E}]$; the compromise between the thermal tail and penetration produces the [Gamow peak](../../../../../gamow-peak.md). A resonance can greatly enhance the rate. Density, abundances and [temperature](../../../../../temperature.md) therefore all affect the [stellar energy-generation rate](../../../../../stellar-energy-generation-rate.md), and power laws such as $T^4$ or $T^{16}$ are local approximations.

For the [proton–proton chain](../../../../../proton-proton-chain.md), first produce deuterium and helium-3:

$$
p+p\longrightarrow {}^2\mathrm H+e^++\nu_e,\qquad
{}^2\mathrm H+p\longrightarrow{}^3\mathrm{He}+\gamma.
$$

The initial reaction is slow because it converts a proton to a neutron through the weak interaction. It is the bottleneck that allows long hydrogen-burning lifetimes. The alternative pep reaction $p+e^-+p\to{}^2\mathrm H+\nu_e$ also feeds the same chain. There are three principal [proton-proton chain branches](../../../../../proton-proton-chain-branches.md). In pp I, two helium-3 nuclei terminate the chain:

$$
{}^3\mathrm{He}+{}^3\mathrm{He}\longrightarrow{}^4\mathrm{He}+2p.
$$

In pp II, helium-3 first captures an existing helium-4 nucleus, then [electron capture](../../../../../electron-capture.md) and proton capture finish the branch:

$$
{}^3\mathrm{He}+{}^4\mathrm{He}\longrightarrow{}^7\mathrm{Be}+\gamma,\qquad
{}^7\mathrm{Be}+e^-\longrightarrow{}^7\mathrm{Li}+\nu_e,\qquad
{}^7\mathrm{Li}+p\longrightarrow2\,{}^4\mathrm{He}.
$$

In pp III, the beryllium-7 instead captures a proton:

$$
{}^7\mathrm{Be}+p\longrightarrow{}^8\mathrm B+\gamma,\qquad
{}^8\mathrm B\longrightarrow{}^8\mathrm{Be}^{*}+e^++\nu_e,\qquad
{}^8\mathrm{Be}^{*}\longrightarrow2\,{}^4\mathrm{He}.
$$

Relative branch weights change with [temperature](../../../../../temperature.md) and composition. All branches convert four protons into a net helium-4 nucleus, with two weak conversions and two [neutrinos](../../../../../neutrino.md), allowing for the electron consumed in pp II. After including positron annihilation, the atomic-mass energy budget is approximately **$26.7\,\mathrm{MeV}$ per net helium-4 nucleus**, but the deposited heat is smaller by the branch-dependent escaping-neutrino energy. Near ordinary low-mass main-sequence conditions, $\epsilon_{pp}\propto\rho X_H^2T^4$ is a useful local approximation.

The [CNO cycle](../../../../../cno-cycle.md) provides an alternative catalyzed [hydrogen burning](../../../../../hydrogen-burning.md) route in hotter cores. The [CNO-I cycle](../../../../../cno-i-cycle.md), also called the [CN cycle](../../../../../cno-i-cycle.md), consists of

$$
\begin{aligned}
{}^{12}\mathrm C+p&\longrightarrow{}^{13}\mathrm N+\gamma,\\
{}^{13}\mathrm N&\longrightarrow{}^{13}\mathrm C+e^++\nu_e,\\
{}^{13}\mathrm C+p&\longrightarrow{}^{14}\mathrm N+\gamma,\\
{}^{14}\mathrm N+p&\longrightarrow{}^{15}\mathrm O+\gamma,\\
{}^{15}\mathrm O&\longrightarrow{}^{15}\mathrm N+e^++\nu_e,\\
{}^{15}\mathrm N+p&\longrightarrow{}^{12}\mathrm C+{}^4\mathrm{He}.
\end{aligned}
$$

The carbon seed is regenerated: the net reaction again consumes four protons and produces one helium-4 nucleus, two positrons and two [neutrinos](../../../../../neutrino.md). The slow ${}^{14}\mathrm N(p,\gamma){}^{15}\mathrm O$ reaction governs the ordinary cycle and causes nitrogen-14 to accumulate. The [CNO-II cycle](../../../../../cno-ii-cycle.md) branches through ${}^{15}\mathrm N(p,\gamma){}^{16}\mathrm O$, ${}^{16}\mathrm O(p,\gamma){}^{17}\mathrm F$, ${}^{17}\mathrm F\to{}^{17}\mathrm O+e^++\nu_e$, and ${}^{17}\mathrm O(p,\alpha){}^{14}\mathrm N$, after which the main cycle continues. Thus CNO nuclei are catalytic in the closed cycles, although their relative abundances change. A local rate is $\epsilon_{\rm CNO}\propto\rho X_HX_{\rm CNO}T^\eta$ with a much steeper exponent than the [PP chain](../../../../../proton-proton-chain.md); the preceding homology problem specifies $\eta=16$. The concentration of this heating near the centre favors a [convective core](../../../../../convective-core.md) in hotter, more massive hydrogen-burning stars.

Once hydrogen is exhausted in a core, contraction can raise its [temperature](../../../../../temperature.md) enough for [core helium burning](../../../../../core-helium-burning.md). The [Triple-alpha process](../../../../../triple-alpha-process.md) overcomes the absence of stable mass-5 and mass-8 nuclei by maintaining a tiny transient beryllium-8 population:

$$
{}^4\mathrm{He}+{}^4\mathrm{He}\rightleftharpoons{}^8\mathrm{Be},\qquad
{}^8\mathrm{Be}+{}^4\mathrm{He}\longrightarrow{}^{12}\mathrm C^{*}
\longrightarrow{}^{12}\mathrm C+\gamma\text{ rays}.
$$

The [Hoyle state](../../../../../hoyle-state.md), an excited carbon-12 resonance near the three-alpha threshold, makes the second capture efficient enough despite beryllium-8's very short lifetime. The net conversion is $3\,{}^4\mathrm{He}\to{}^{12}\mathrm C$, releasing about **$7.27\,\mathrm{MeV}$**. Because three alpha particles are required, the specific rate scales as $\rho^2Y^3$; a schematic resonant rate is

$$
\epsilon_{3\alpha}\propto\rho^2Y^3T_8^{-3}e^{-44/T_8},\qquad
T_8=T/(10^8\,\mathrm K).
$$

Its local [temperature](../../../../../temperature.md) exponent is $-3+44/T_8$, of order forty near $T_8=1$. A degenerate core cannot expand promptly to regulate this increase, giving a [helium flash](../../../../../helium-flash.md); in a nondegenerate core the [stellar thermostat](../../../../../stellar-thermostat.md) permits stable helium burning. The competing ${}^{12}\mathrm C(\alpha,\gamma){}^{16}\mathrm O$ reaction determines much of the eventual carbon-oxygen mixture.

If the core becomes hot enough, [carbon burning](../../../../../carbon-burning.md) follows, for example through ${}^{12}\mathrm C+{}^{12}\mathrm C\to{}^{20}\mathrm{Ne}+\alpha$ and ${}^{12}\mathrm C+{}^{12}\mathrm C\to{}^{23}\mathrm{Na}+p$. [Neon burning](../../../../../neon-burning.md) begins with [photodisintegration](../../../../../nuclear-photodisintegration.md), ${}^{20}\mathrm{Ne}+\gamma\to{}^{16}\mathrm O+\alpha$, followed by alpha capture such as ${}^{20}\mathrm{Ne}+\alpha\to{}^{24}\mathrm{Mg}+\gamma$. The first step consumes heat, but the combined rearrangement can release net energy. [Oxygen burning](../../../../../oxygen-burning.md) includes ${}^{16}\mathrm O+{}^{16}\mathrm O\to{}^{28}\mathrm{Si}+\alpha$ and channels producing phosphorus and other nearby nuclei. At still higher temperatures, [silicon burning](../../../../../silicon-burning.md) proceeds through [photodisintegration](../../../../../nuclear-photodisintegration.md) and particle captures in a reaction network approaching quasi-statistical equilibrium, producing iron-group nuclei. It is not simply direct silicon-plus-silicon fusion; the products depend on the electron fraction and weak-interaction timescale.

The increasing [nuclear binding energy](../../../../../nuclear-binding-energy.md) per nucleon supplies progressively less energy as products approach the iron group. Further fusion past that region cannot provide sustained net heat to support a core. Massive stars can therefore end with an unstable iron-group core; lower-mass stars do not attain all these burning stages and instead leave remnants such as [carbon-oxygen white dwarfs](../../../../../carbon-oxygen-white-dwarf.md). Heavy-element neutron captures can synthesize nuclei beyond the iron group without being the principal hydrostatic power source.

Finally, [stellar neutrino energy loss](../../../../../stellar-neutrino-energy-loss.md) competes with every heat source. Reaction [neutrinos](../../../../../neutrino.md) accompany the proton–proton and CNO chains. Hot or dense material also emits [neutrino](../../../../../neutrino.md) pairs through $e^-+e^+\to\nu+\bar\nu$, plasmon decay, $e^-+\gamma\to e^-+\nu+\bar\nu$, and electron-ion bremsstrahlung. These [neutrinos](../../../../../neutrino.md) usually escape, unlike the [photons](../../../../../photon.md) whose transport is diffusive; [neutrino](../../../../../neutrino.md) trapping requires much more extreme collapse conditions. Late burning has smaller fuel-energy reservoirs and strong [neutrino](../../../../../neutrino.md) cooling, so its duration is much shorter than core hydrogen burning. The surface [luminosity](../../../../../luminosity.md) is the escaping photon power, $L=4\pi R^2\sigma T_{\rm eff}^4$, not the sum of [photons](../../../../../photon.md) and unobserved [neutrino](../../../../../neutrino.md) power. [Radiative diffusion in a star](../../../../../radiative-diffusion-in-a-star.md), convection and electron conduction redistribute energy, while the energy-balance equation distinguishes true sources, losses and storage. Accretion or mass loss adds boundary energy and mechanical work when present, rather than changing the nuclear reaction budget.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 317](../../paper-317-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
