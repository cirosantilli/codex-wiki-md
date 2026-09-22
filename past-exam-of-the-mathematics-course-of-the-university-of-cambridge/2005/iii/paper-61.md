# Paper 61

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper61.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper61.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 61](paper-61.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use [natural units](../../../physics.md#natural-units) with $c=1$, write $H=\dot a/a$, and measure [cosmic time](../../../cosmology.md#cosmic-time) from the [Big Bang](../../../cosmology.md#big-bang). The [cosmological continuity equation](../../../cosmology.md#cosmological-continuity-equation) follows by differentiating the [Friedmann equation](../../../cosmology.md#friedmann-equations) and using the [Friedmann acceleration equation](../../../cosmology.md#friedmann-acceleration-equation); for [pressureless matter](../../../cosmology.md#pressureless-matter) it gives $\dot\rho+3H\rho=0$, hence $\rho=\rho_0a^{-3}$ when the present [scale factor](../../../cosmology.md#scale-factor-cosmology) is $a_0=1$. The present [critical density](../../../cosmology.md#critical-density) and [cosmological density parameter](../../../cosmology.md#cosmological-density-parameter) give

$$
\rho_{c0}=\frac{3H_0^2}{8\pi G},\qquad \rho_0=\Omega_0\rho_{c0},\qquad k=H_0^2(\Omega_0-1)>0.
$$

Consequently, with $C=H_0^2\Omega_0$, the [Friedmann equation](../../../cosmology.md#friedmann-equations) becomes $\dot a^2=C/a-k$.

Introduce [conformal time](../../../cosmology.md#conformal-time) through $dt=a\,d\tau$. A prime denotes a [derivative](../../../calculus.md#derivative) with respect to $\tau$, so $a'=a\dot a$ and

$$
(a')^2=Ca-ka^2=k\left[\left(\frac C{2k}\right)^2-\left(a-\frac C{2k}\right)^2\right].
$$

Set $u=\sqrt{k}\tau$, with $u=0$ at the [Big Bang](../../../cosmology.md#big-bang). On the expanding branch the substitution $a=C(1-\cos u)/(2k)$ satisfies this equation. Integrating $dt=a\,du/\sqrt{k}$, with $t(0)=0$, gives the [closed matter-dominated Friedmann solution](../../../cosmology.md#closed-matter-dominated-friedmann-solution):

$$
\boxed{a(\tau)=\frac{\Omega_0}{2(\Omega_0-1)}(1-\cos u),\qquad t(\tau)=\frac{\Omega_0}{2H_0(\Omega_0-1)^{3/2}}(u-\sin u),\qquad u=\sqrt{k}\tau.}
$$

The parametrization continues smoothly through the maximum [scale factor](../../../cosmology.md#scale-factor-cosmology), reached at $u=\pi$, onto the contracting branch. Its curve in the $(t,a)$ plane is a rescaled [cycloid](../../../topology.md#cycloid).

For a presently expanding universe, $H_0>0$ selects $0<u_0<\pi$. The normalization $a(u_0)=1$ gives

$$
\cos u_0=\frac2{\Omega_0}-1,\qquad \sin u_0=\frac{2\sqrt{\Omega_0-1}}{\Omega_0},\qquad u_0=\arccos\left(\frac2{\Omega_0}-1\right).
$$

Substitution yields the [age of a closed dust universe](../../../cosmology.md#age-of-a-closed-dust-universe):

$$
\boxed{t_0=\frac{\Omega_0}{2H_0(\Omega_0-1)^{3/2}}\left[\arccos\left(\frac2{\Omega_0}-1\right)-\frac{2\sqrt{\Omega_0-1}}{\Omega_0}\right].}
$$

The first later zero of the [scale factor](../../../cosmology.md#scale-factor-cosmology) occurs at $u=2\pi$, so the [lifetime of a closed dust universe](../../../cosmology.md#lifetime-of-a-closed-dust-universe) gives the [Big Crunch](../../../cosmology.md#big-crunch) time

$$
\boxed{t_{\rm BC}=\frac{\pi\Omega_0}{H_0(\Omega_0-1)^{3/2}}.}
$$

This is the total lifetime measured from the [Big Bang](../../../cosmology.md#big-bang); the remaining [cosmic time](../../../cosmology.md#cosmic-time) is $t_{\rm BC}-t_0$. As a check, the [limit](../../../calculus.md#limit-of-a-function) $\Omega_0\downarrow1$ gives $H_0t_0\to2/3$, while the [Big Crunch](../../../cosmology.md#big-crunch) recedes to infinite time, as expected for a flat [matter-dominated universe](../../../linear-cosmological-density-perturbation.md#matter-domination) with zero [cosmological constant](../../../cosmology.md#cosmological-constant).

## 2

↑ **Parent:** [Paper 61](paper-61.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Use [natural units](../../../physics.md#natural-units) $\hbar=c=k_B=1$ and the unreduced [Planck mass](../../../physics.md#planck-mass) $M_P=G^{-1/2}$. [Neutrino decoupling](../../../cosmology.md#neutrino-decoupling) occurs when the [weak interaction](../../../standard-model.md#weak-interaction) rate falls below the [Hubble parameter](../../../cosmology.md#hubble-parameter). The [weak-decoupling temperature estimate](../../../cosmology.md#weak-decoupling-temperature-estimate) equates the given rate with the radiation-era expansion rate:

$$
G_F^2T_d^5\simeq1.66\sqrt{g_*}\frac{T_d^2}{M_P},\qquad \boxed{T_d\simeq\left(\frac{1.66\sqrt{g_*}}{G_F^2M_P}\right)^{1/3}\simeq1.8\ {\rm MeV}.}
$$

Here $g_*$ counts the [effective number of relativistic energy degrees of freedom](../../../cosmology.md#effective-number-of-relativistic-energy-degrees-of-freedom), and the [Fermi constant](../../../quantum-field-theory.md#fermi-constant) is $G_F\simeq10^{-5}\ {\rm GeV}^{-2}$. The omitted reaction-rate coefficients make this an order-of-magnitude estimate: **decoupling occurs at a temperature of order one MeV**.

The charge-conserving channel is $n+\nu_e\leftrightarrow p+e^-$, together with $p+\bar\nu_e\leftrightarrow n+e^+$. The positron sign in the printed neutron-capture channel violates [electric charge conservation](../../../electromagnetism.md#charge-conservation). [Chemical equilibrium](../../../thermodynamics.md#chemical-equilibrium) requires $\mu_n+\mu_{\nu_e}=\mu_p+\mu_e$. Negligible lepton [chemical potentials](../../../thermodynamics.md#chemical-potential) therefore give $\mu_n\simeq\mu_p$. Since [neutrons](../../../physics.md#neutron) and [protons](../../../physics.md#proton) are [nonrelativistic particles](../../../special-relativity.md#nonrelativistic-particle), their [Maxwell-Boltzmann distribution](../../../statistical-physics.md#maxwell-boltzmann-distribution) gives

$$
n_i=g_i\left(\frac{m_iT}{2\pi}\right)^{3/2}e^{(\mu_i-m_i)/T},\qquad \frac{n_n}{n_p}=\frac{g_n}{g_p}\left(\frac{m_n}{m_p}\right)^{3/2}e^{-(m_n-m_p)/T}.
$$

Both nucleons have two spin states, and their masses agree closely in the prefactor. Thus [neutron-proton chemical equilibrium](../../../cosmology.md#neutron-proton-chemical-equilibrium) implies

$$
\boxed{\frac{n_n}{n_p}=\frac{X_n}{X_p}\simeq e^{-Q/T_d},\qquad Q=m_n-m_p>0.}
$$

The heavier [neutron](../../../physics.md#neutron) is suppressed by a [Boltzmann factor](../../../statistical-physics.md#boltzmann-factor).

For the [deuterium equilibrium abundance](../../../cosmology.md#deuterium-equilibrium-abundance), retain the paper's convention $B=m_D-m_n-m_p<0$; the positive [nuclear binding energy](../../../physics.md#nuclear-binding-energy) is $\varepsilon_D=-B\simeq2.22\ {\rm MeV}$. [Chemical equilibrium](../../../thermodynamics.md#chemical-equilibrium) of $n+p\leftrightarrow D+\gamma$ gives $\mu_D=\mu_n+\mu_p$ because the equilibrium [photon](../../../quantum-mechanics.md#photon) [chemical potential](../../../thermodynamics.md#chemical-potential) vanishes. Using the [nonrelativistic Maxwell--Boltzmann number density](../../../statistical-physics.md#nonrelativistic-maxwell-boltzmann-number-density) for each species and dividing gives

$$
\frac{n_D}{n_nn_p}=\frac{g_D}{g_ng_p}\left(\frac{m_D}{m_nm_p}\right)^{3/2}\left(\frac{2\pi}{T}\right)^{3/2}e^{-B/T}.
$$

Here $g_D=3$ and $g_n=g_p=2$. With the [baryon-to-photon ratio](../../../cosmology.md#baryon-to-photon-ratio) $\eta=n_B/n_\gamma$, the [photon number density](../../../statistical-physics.md#photon-number-density) $n_\gamma=2\zeta(3)T^3/\pi^2$, and $m_D\simeq2m_N$, $m_n\simeq m_p\simeq m_N$, this becomes

$$
\boxed{\frac{X_D}{X_nX_p}\simeq\frac{12\zeta(3)}{\sqrt\pi}\,\eta\left(\frac{T}{m_N}\right)^{3/2}e^{-B/T}\simeq8.14\,\eta\left(\frac{T}{m_N}\right)^{3/2}e^{\varepsilon_D/T}.}
$$

In this convention $X_D=n_D/n_B$ counts nuclei, so its contribution to the fraction of baryons in [deuterium](../../../chemistry.md#deuterium) is $2X_D$.

The [deuterium bottleneck](../../../cosmology.md#deuterium-bottleneck) explains why [helium-4](../../../chemistry.md#helium-4) formation waits until $T$ is far below $\varepsilon_D$. At higher [temperature](../../../thermodynamics.md#temperature), there are vastly more [photons](../../../quantum-mechanics.md#photon) than baryons; even the dilute energetic tail can destroy newly formed [deuterium](../../../chemistry.md#deuterium). A crude estimate balances $\eta^{-1}e^{-\varepsilon_D/T}$ against one, giving $T\sim\varepsilon_D/\log(\eta^{-1})\sim0.1\ {\rm MeV}$ for $\eta$ of order $10^{-9}$. The power-law factors in the [deuterium equilibrium abundance](../../../cosmology.md#deuterium-equilibrium-abundance) and the nuclear reaction rates refine this estimate. Once stable [deuterium](../../../chemistry.md#deuterium) accumulates, further reactions can efficiently place nearly all surviving [neutrons](../../../physics.md#neutron) into [helium-4](../../../chemistry.md#helium-4).

Write $r_N=n_n/n_p$ at the onset of nuclear burning. Each [helium-4](../../../chemistry.md#helium-4) nucleus requires two [neutrons](../../../physics.md#neutron) and contains four baryons. [Neutron-limited helium synthesis](../../../cosmology.md#neutron-limited-helium-synthesis) therefore gives the [primordial helium mass fraction](../../../cosmology.md#primordial-helium-mass-fraction)

$$
\boxed{Y_4\simeq\frac{4n_{\rm He}}{n_B}\simeq2X_n(T_N)=\frac{2r_N}{1+r_N}.}
$$

For a realistic rough [cosmological weak freeze-out](../../../cosmology.md#cosmological-weak-freeze-out) estimate, $r_f$ is about $1/6$ and [free-neutron decay after freeze-out](../../../cosmology.md#free-neutron-decay-after-freeze-out) reduces it to about $1/7$, giving **roughly one quarter of the baryonic mass in helium-4**. The survival relation that conserves [baryon number](../../../standard-model.md#baryon-number) is $X_n(T_N)=r_f(1+r_f)^{-1}e^{-\Delta t/\tau_n}$; the corresponding $r_N$ is $X_n/(1-X_n)$.

The rough [neutrino decoupling](../../../cosmology.md#neutrino-decoupling) rate by itself does not determine that one-quarter value. Substituting $T_d=1.8\ {\rm MeV}$ literally into $e^{-Q/T_d}$ would give $r\simeq0.49$ and $Y_4\simeq0.65$ before neutron decay. [Neutron-proton chemical equilibrium](../../../cosmology.md#neutron-proton-chemical-equilibrium) persists to a lower temperature, approximately $0.7$--$0.8\ {\rm MeV}$ once the actual conversion rates are included. The rate scaling fixes the MeV scale; accurate abundances need the conversion coefficients and the delay through the [deuterium bottleneck](../../../cosmology.md#deuterium-bottleneck). This sequence is described in [David Tong's discussion of nucleosynthesis](https://www.davidtong.org/teaching/cosmology/cosmohtml/S2#S2.SS5.SSS3).

Increasing $Q$ reduces the equilibrium [neutron-to-proton ratio](../../../cosmology.md#neutron-to-proton-ratio), so **the primordial helium abundance decreases**. Holding the freeze-out temperature $T_f$ and the decay survival factor fixed, the [primordial helium response to the neutron-proton mass difference](../../../cosmology.md#primordial-helium-response-to-the-neutron-proton-mass-difference) is

$$
\boxed{\frac{Y_4(1.1Q)}{Y_4(Q)}\simeq\frac{1+e^{Q/T_f}}{1+e^{1.1Q/T_f}}.}
$$

For $Q\simeq1.29\ {\rm MeV}$ and $T_f=0.7$--$0.8\ {\rm MeV}$ this is about $0.85$--$0.87$, a reduction of roughly fifteen percent. A larger $Q$ also changes neutron decay and detailed weak rates; their quantitative effects require more microscopic information. The sign from the [Boltzmann factor](../../../statistical-physics.md#boltzmann-factor) is already clear.

## 3

↑ **Parent:** [Paper 61](paper-61.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Use [natural units](../../../physics.md#natural-units) and the unreduced [Planck mass](../../../physics.md#planck-mass) $M_P=G^{-1/2}$; it is $\sqrt{8\pi}$ times the [reduced Planck mass](../../../physics.md#reduced-planck-mass). A homogeneous canonical [inflaton](../../../cosmic-inflation.md#inflaton) has $\rho_\phi=\dot\phi^2/2+V$ and $P_\phi=\dot\phi^2/2-V$. [Vacuum domination by a scalar field](../../../cosmic-inflation.md#vacuum-domination-by-a-scalar-field) requires $\dot\phi_i^2/2\ll V(\phi_i)$, with other matter and the curvature term negligible in the [Friedmann equation](../../../cosmology.md#friedmann-equations). The [equation-of-state parameter](../../../cosmology.md#equation-of-state-parameter) is then near $-1$, and the [Friedmann acceleration equation](../../../cosmology.md#friedmann-acceleration-equation) gives [accelerating expansion](../../../cosmology.md#accelerating-expansion-of-the-universe).

For sustained [slow-roll inflation](../../../cosmic-inflation.md#slow-roll-approximation), [Hubble friction](../../../cosmology.md#hubble-friction) must dominate the [inflaton](../../../cosmic-inflation.md#inflaton) acceleration: $|\ddot\phi|\ll3H|\dot\phi|$, with the [scalar potential](../../../quantum-field-theory.md#scalar-potential) changing only slightly in one [Hubble time](../../../cosmology.md#hubble-time). In terms of the [potential slow-roll parameter](../../../cosmic-inflation.md#potential-slow-roll-parameter) and [second potential slow-roll parameter](../../../cosmic-inflation.md#second-potential-slow-roll-parameter), this requires

$$
\epsilon_V=\frac{M_P^2}{16\pi}\left(\frac{V'}V\right)^2\ll1,\qquad |\eta_V|=\left|\frac{M_P^2}{8\pi}\frac{V''}V\right|\ll1.
$$

For the quartic [scalar potential](../../../quantum-field-theory.md#scalar-potential),

$$
\epsilon_V=\frac{M_P^2}{\pi\phi^2},\qquad \eta_V=\frac{3M_P^2}{2\pi\phi^2}.
$$

Thus $|\phi_i|\gg M_P$ supplies a broad [slow-roll](../../../cosmic-inflation.md#slow-roll-approximation) range when $\lambda\ll1$. At an initial density of order the Planck density, potential domination gives

$$
\boxed{\phi_i^2\sim\frac{2M_P^2}{\sqrt\lambda},\qquad V_i\sim M_P^4,}
$$

so both [potential slow-roll parameters](../../../cosmic-inflation.md#potential-slow-roll-parameter) are small for small $\lambda$. Small initial [kinetic energy](../../../classical-mechanics.md#kinetic-energy) is a separate condition; the height of the [scalar potential](../../../quantum-field-theory.md#scalar-potential) alone does not enforce it. These classical equations describe the post-Planck evolution under the model assumptions, rather than resolving [quantum gravity](../../../quantum-theory.md#quantum-gravity) at the initial endpoint.

Take $\phi_i>0$; the negative branch follows by the symmetry $\phi\mapsto-\phi$. Dropping [kinetic energy](../../../classical-mechanics.md#kinetic-energy) from the [Friedmann equation](../../../cosmology.md#friedmann-equations) and acceleration from the [inflaton equation of motion](../../../cosmic-inflation.md#inflaton-equation-of-motion) gives

$$
H\simeq\frac1{M_P}\sqrt{\frac{2\pi\lambda}{3}}\,\phi^2,\qquad 3H\dot\phi\simeq-\lambda\phi^3.
$$

Writing $b=M_P\sqrt{\lambda/(6\pi)}$, the [quartic-potential slow-roll solution](../../../cosmic-inflation.md#quartic-potential-slow-roll-solution) is

$$
\boxed{\phi(t)\simeq\phi_i e^{-b(t-t_i)},\qquad a(t)\simeq a_i\exp\left[\frac{\pi\phi_i^2}{M_P^2}\left(1-e^{-2b(t-t_i)}\right)\right].}
$$

Indeed, $\dot\phi\simeq-b\phi$, and integrating $H=\dot a/a$ gives $\log(a/a_i)=\pi(\phi_i^2-\phi^2)/M_P^2$. These expressions apply during [slow-roll inflation](../../../cosmic-inflation.md#slow-roll-approximation); their formal late-time saturation must not be used beyond the end of that approximation.

The exact end of [accelerating expansion](../../../cosmology.md#accelerating-expansion-of-the-universe) is $\epsilon_H=-\dot H/H^2=1$, equivalently $\dot\phi^2=V$ for the scalar-dominated flat model. The [quartic-inflation endpoint estimate](../../../cosmic-inflation.md#quartic-inflation-endpoint-estimate) uses the leading potential condition $\epsilon_V\simeq1$, giving

$$
\boxed{|\phi_e|\sim M_P,\qquad |\phi_e|\simeq\frac{M_P}{\sqrt\pi}\ \text{using }\epsilon_V=1.}
$$

The numerical coefficient is an endpoint estimate: the [slow-roll approximation](../../../cosmic-inflation.md#slow-roll-approximation) breaks down there. Imposing $|\eta_V|=1$ estimates when slow roll loses accuracy and gives a different order-one coefficient, not a different exact acceleration condition.

The [slow-roll e-fold count](../../../cosmic-inflation.md#slow-roll-e-fold-count) is

$$
N\simeq\frac{8\pi}{M_P^2}\int_{\phi_e}^{\phi_i}\frac{V}{V'}\,d\phi=\frac{\pi}{M_P^2}(\phi_i^2-\phi_e^2).
$$

The [quartic-inflation expansion from Planck density](../../../cosmic-inflation.md#quartic-inflation-expansion-from-planck-density) combines this initial estimate with the conventional endpoint to give

$$
\boxed{N\sim\frac{2\pi}{\sqrt\lambda}-1,\qquad \frac{a_e}{a_i}\sim\exp\left(\frac{2\pi}{\sqrt\lambda}-1\right).}
$$

For small $\lambda$ the dominant term is enormous; the order-one endpoint uncertainty does not affect that conclusion.

To estimate the [reheating temperature](../../../cosmic-inflation.md#reheating-temperature), assume prompt, efficient [reheating](../../../cosmic-inflation.md#reheating) converts the end-of-inflation energy into a thermal radiation bath. With the same endpoint convention, $V_e\simeq\lambda M_P^4/(4\pi^2)$, and equating this to the radiation [energy density](../../../statistical-physics.md#energy-density) gives

$$
\frac{\pi^2}{30}g_*T_R^4\sim\frac{\lambda M_P^4}{4\pi^2},\qquad \boxed{T_R\sim\left(\frac{15\lambda}{2\pi^4g_*}\right)^{1/4}M_P\sim\lambda^{1/4}g_*^{-1/4}M_P.}
$$

The [quartic-inflation prompt-reheating estimate](../../../cosmic-inflation.md#quartic-inflation-prompt-reheating-estimate) fixes the scaling; the endpoint [kinetic energy](../../../classical-mechanics.md#kinetic-energy) changes the coefficient by order one. Without an inflaton coupling and its thermalization history, $V$ alone cannot specify the actual [reheating temperature](../../../cosmic-inflation.md#reheating-temperature).

Finally, during [cosmic inflation](../../../cosmic-inflation.md) the [comoving Hubble radius](../../../cosmology.md#comoving-hubble-radius) decreases:

$$
\frac d{dt}\frac1{aH}=-\frac{1-\epsilon_H}{a}<0.
$$

An initially causally connected patch is enlarged enough that the present observable region can lie within it. Its portions may subsequently be far outside one another's Hubble radii while retaining their common earlier thermal history. This solves the [horizon problem](../../../cosmology.md#horizon-problem) if the [number of e-folds](../../../cosmic-inflation.md#number-of-e-folds) is sufficiently large, conventionally of order sixty for the relevant thermal history; $N\sim2\pi/\sqrt\lambda$ can readily exceed that. The necessary count depends on [reheating](../../../cosmic-inflation.md#reheating) and later expansion. The causal mechanism and the conversion back to a hot universe are discussed in [David Tong's account of inflation](https://www.davidtong.org/teaching/cosmology/cosmohtml/S1#S1.SS5).

## 4

↑ **Parent:** [Paper 61](paper-61.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Use [natural units](../../../physics.md#natural-units), assume negligible neutrino [chemical potentials](../../../thermodynamics.md#chemical-potential), and approximate [neutrino decoupling](../../../cosmology.md#neutrino-decoupling) as occurring before [electron-positron annihilation in cosmology](../../../cosmology.md#electron-positron-annihilation-in-cosmology). At high [temperature](../../../thermodynamics.md#temperature), [weak interactions](../../../standard-model.md#weak-interaction) maintain a common temperature for [neutrinos](../../../standard-model.md#neutrino), [antineutrinos](../../../standard-model.md#antineutrino), [Electrons](../../../physics.md#electron), [Positrons](../../../physics.md#positron) and [photons](../../../quantum-mechanics.md#photon). Since $\Gamma_\nu/H\propto T^3$, the reaction rate eventually loses against expansion. Decoupled relativistic [neutrinos](../../../standard-model.md#neutrino) then free stream; their momenta redshift as $a^{-1}$, so their distribution retains a temperature parameter satisfying $aT_\nu=\mathrm{constant}$.

The still-coupled electromagnetic bath receives the [entropy](../../../thermodynamics.md#entropy) of annihilating [Electrons](../../../physics.md#electron) and [Positrons](../../../physics.md#positron). Its [effective number of relativistic entropy degrees of freedom](../../../cosmology.md#effective-number-of-relativistic-degrees-of-freedom) is initially

$$
g_{*s}^{\rm EM}=2+\frac78(2+2)=\frac{11}{2},
$$

where the two [photon](../../../quantum-mechanics.md#photon) polarizations count as bosonic states and the four electron-positron spin states have the [fermion](../../../quantum-mechanics.md#fermion) entropy weight $7/8$. After the pairs disappear, $g_{*s}^{\rm EM}=2$. [Cosmological entropy conservation](../../../cosmology.md#cosmological-entropy-conservation) in this coupled bath gives $g_{*s}^{\rm EM}(aT_\gamma)^3=\mathrm{constant}$. The three already decoupled neutrino species are excluded from this bath's entropy count. At decoupling $T_\nu=T_\gamma$, hence

$$
\boxed{\frac{T_\nu}{T_\gamma}=\left(\frac{2}{11/2}\right)^{1/3}=\left(\frac4{11}\right)^{1/3}\simeq0.714.}
$$

Subsequent expansion preserves this ratio in the idealized history. Residual interactions during annihilation give small corrections to the instantaneous-decoupling approximation. If a relic species later becomes massive, $T_\nu$ here remains the redshifting momentum-distribution parameter; it need not be its nonrelativistic kinetic temperature.

A single ordinary neutrino species includes one populated [neutrino](../../../standard-model.md#neutrino) [helicity](../../../special-relativity.md#helicity) and one [antineutrino](../../../standard-model.md#antineutrino) [helicity](../../../special-relativity.md#helicity). For negligible [chemical potential](../../../thermodynamics.md#chemical-potential), integration of the [Fermi-Dirac distribution](../../../statistical-physics.md#fermi-dirac-distribution) gives

$$
n_\nu+n_{\bar\nu}=\frac{3\zeta(3)}{2\pi^2}T_\nu^3,\qquad n_\gamma=\frac{2\zeta(3)}{\pi^2}T_\gamma^3.
$$

Therefore the [number density of a relativistic neutrino relative to photons](../../../cosmology.md#number-density-of-a-relativistic-neutrino-relative-to-photons), with the antiparticle included, is

$$
\boxed{\frac{n_\nu+n_{\bar\nu}}{n_\gamma}=\frac34\left(\frac{T_\nu}{T_\gamma}\right)^3=\frac3{11}.}
$$

The factor $3/4$ is the fermionic number-density weight, distinct from the energy and entropy weight $7/8$. This relation continues to hold after this species becomes nonrelativistic if its comoving particle number is conserved.

Under the proposed matter-dominated, spatially flat model, the [Friedmann equation](../../../cosmology.md#friedmann-equations) requires the present [relic-neutrino energy density](../../../cosmology.md#relic-neutrino-energy-density) to be approximately the [critical density](../../../cosmology.md#critical-density). Using the unreduced [Planck mass](../../../physics.md#planck-mass) $M_P=G^{-1/2}$ gives

$$
\rho_{c0}=\frac{3H_0^2M_P^2}{8\pi}\simeq m_\nu(n_\nu+n_{\bar\nu}).
$$

Thus the [critical-density mass of a thermal relic neutrino](../../../cosmology.md#critical-density-mass-of-a-thermal-relic-neutrino) is

$$
\boxed{m_\nu\simeq\frac{11\pi}{16\zeta(3)}\frac{H_0^2M_P^2}{T_{\gamma0}^3}.}
$$

Taking the paper's rounded values, $T_{\gamma0}=2\times10^{-13}\ {\rm GeV}$, $H_0=h/(4.5\times10^{41}\ {\rm GeV}^{-1})$ and $M_P\sim10^{19}\ {\rm GeV}$, gives

$$
\boxed{m_\nu\sim1.1\times10^{-7}h^2\ {\rm GeV}\sim10^2h^2\ {\rm eV}.}
$$

For $0.5<h<1$, this is of order $30$--$100\ {\rm eV}$ with these approximate constants. More precise constants change the coefficient, not the requested mass scale. This mass is much larger than the present momentum scale $T_{\nu0}\simeq1.4\times10^{-4}\ {\rm eV}$, validating the nonrelativistic [energy density](../../../statistical-physics.md#energy-density) approximation. The result assumes that one thermal relic species dominates the matter density; it is conditional on that model rather than a measurement of a neutrino mass.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2005](../../2005.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
