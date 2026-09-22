# Chemical potential

↑ **Parent:** [Thermodynamics](thermodynamics-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chemical_potential)

The [chemical potential](chemical-potential.md) measures how a [thermodynamic potential](thermodynamic-potential.md) changes when matter is added under specified constraints. It plays for matter exchange the role that [temperature](temperature.md) plays for [heat](heat.md) exchange: a difference supplies a direction, and equality characterizes [thermodynamic equilibrium](thermodynamic-equilibrium.md) when the corresponding exchange is allowed. This connects [diffusion](diffusion.md), [phase coexistence](phase-coexistence.md) and [chemical equilibrium](chemical-equilibrium.md) through one quantity.

For a single component, the particle convention is

$$
\mu_{\rm particle}=\left(\frac{\partial U}{\partial N}\right)_{S,V},
$$

where $U$ is [internal energy](internal-energy.md), $N$ counts particles, $S$ is [entropy](entropy.md) and $V$ is [volume](volume-thermodynamics.md). This [partial derivative](partial-derivative.md) holds [entropy](entropy.md) and [volume](volume-thermodynamics.md) fixed; it measures an incremental change rather than the average [energy](energy.md) per particle. See [David Tong, Statistical Physics, section 1.4](https://davidtong.org/pdfs/teaching/statistical-physics/statphys1.pdf).

In [chemistry](chemistry-split.md) the molar convention instead uses [amount of substance](amount-of-substance.md) $n$, measured in [moles](mole-unit.md):

$$
\mu_{\rm m}=\left(\frac{\partial G}{\partial n}\right)_{T,p},
\qquad n=\frac{N}{N_{\rm A}},
\qquad \mu_{\rm m}=N_{\rm A}\mu_{\rm particle}.
$$

Here $G$ is [Gibbs free energy](gibbs-free-energy.md), $T$ is [temperature](temperature.md), $p$ is [pressure](pressure.md) and $N_{\rm A}$ is the [Avogadro constant](avogadro-constant.md). The units are $\mathrm J$ per particle versus $\mathrm{J\,mol^{-1}}$. For several [chemical species](chemical-species.md), define each [chemical potential](chemical-potential.md) by varying only its own particle count or [amount of substance](amount-of-substance.md), with all other components' counts or amounts fixed. Many texts use $\mu$ for either convention, so the units and the variable being differentiated must identify it.

For a [simple compressible system](simple-compressible-system.md) with variable component inventories, the fundamental differentials are

$$
dU=T\,dS-p\,dV+\sum_i\mu_{{\rm particle},i}\,dN_i,
\qquad
dG=-S\,dT+V\,dp+\sum_i\mu_{{\rm m},i}\,dn_i.
$$

They describe changes between states in [thermodynamic equilibrium](thermodynamic-equilibrium.md) with only [pressure](pressure.md)-[volume](volume-thermodynamics.md) [work](work.md). If every component inventory is fixed, the sums vanish. The [Gibbs free energy](gibbs-free-energy.md) form follows by differentiating $G=U-TS+pV$ and using $dN_i=N_{\rm A}\,dn_i$; this is why the two definitions describe the same [chemical potential](chemical-potential.md) in different units.

A [chemical potential](chemical-potential.md) can be negative. Holding [entropy](entropy.md) fixed while adding matter need not increase [internal energy](internal-energy.md); Tong explains this explicitly for a classical [ideal gas](ideal-gas.md) in [Statistical Physics, section 2.2.4](https://davidtong.org/pdfs/teaching/statistical-physics/statphys2.pdf). Its absolute sign also depends on the reference [energy](energy.md): replacing $U$ by $U+\epsilon_0N$ shifts $\mu_{\rm particle}$ by $\epsilon_0$. A common reference shift cancels from differences for the same [chemical species](chemical-species.md), which are what determine exchange. Thus “energy cost” means a signed increment, not an always positive amount that must be supplied.

**Table of contents**

- [Chemical potential equality for particle exchange](chemical-potential-equality-for-particle-exchange.md)
  - [Chemical potential and Helmholtz free energy](chemical-potential-and-helmholtz-free-energy.md)
- [Chemical potential of an ideal gas](chemical-potential-of-an-ideal-gas.md)
- [Electrochemical potential](electrochemical-potential.md)
  - [Electrochemical gradient](electrochemical-gradient.md)
- [Chemical potential of a composition field](chemical-potential-of-a-composition-field.md)
- [Chemical equilibrium](chemical-equilibrium.md)
  - [Chemical disequilibrium](chemical-disequilibrium.md)
  - [Zero chemical potential from number-changing reactions](zero-chemical-potential-from-number-changing-reactions.md)
  - [Chemical relaxation time](chemical-relaxation-time.md)
  - [Equilibrium constant](equilibrium-constant.md)
    - [Dissociation constant](dissociation-constant.md)
  - [Standard state](standard-state.md)
    - [Thermodynamic activity](thermodynamic-activity.md)
      - [Activity coefficient](activity-coefficient.md)
  - [Reaction quotient](reaction-quotient.md)
  - [Photon chemical potential](photon-chemical-potential.md)

## ↑ Ancestors (5)

1. [Thermodynamics](thermodynamics-split.md)
2. [Statistical physics](statistical-physics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (133)

- [Boltzmann distribution](boltzmann-distribution.md)
- [Boltzmann suppression](boltzmann-suppression.md)
- [Boltzmann suppression of a nonrelativistic relic](boltzmann-suppression-of-a-nonrelativistic-relic.md)
- [Chemical equilibrium](chemical-equilibrium.md)
- [Chemical potential](chemical-potential.md)
- [Chemical potential and Helmholtz free energy](chemical-potential-and-helmholtz-free-energy.md)
- [Chemical potential equality for particle exchange](chemical-potential-equality-for-particle-exchange.md)
- [Chemical potential of a composition field](chemical-potential-of-a-composition-field.md)
- [Chemical potential of an ideal gas](chemical-potential-of-an-ideal-gas.md)
- [Clapeyron pressure relation for equal-density phases](clapeyron-pressure-relation-for-equal-density-phases.md)
- [Clausius-Clapeyron relation](clausius-clapeyron-relation.md)
- [Common-pressure melting-point slope](common-pressure-melting-point-slope.md)
- [Common-tangent construction for phase coexistence](common-tangent-construction-for-phase-coexistence.md)
- [Condensate compressibility in an optical lattice](condensate-compressibility-in-an-optical-lattice.md)
- [Constrained Gibbs minimization for chemical equilibrium](constrained-gibbs-minimization-for-chemical-equilibrium.md)
- [Cubic-quintic Gross–Pitaevskii equation](cubic-quintic-gross-pitaevskii-equation.md)
- [Degenerate neutrino and antineutrino energy density](degenerate-neutrino-and-antineutrino-energy-density.md)
- [Diffusion-capacitance analogy](diffusion-capacitance-analogy.md)
- [Diffusion-controlled droplet growth](diffusion-controlled-droplet-growth.md)
- [Electrochemical gradient](electrochemical-gradient.md)
- [Electrochemical potential](electrochemical-potential.md)
- [Electron-positron thermal pair abundance](electron-positron-thermal-pair-abundance.md)
- [Entropy density](entropy-density.md)
- [Entropy density at zero chemical potential](entropy-density-at-zero-chemical-potential.md)
- [Entropy density of a photon gas](entropy-density-of-a-photon-gas.md)
- [Fermi energy](fermi-energy.md)
- [Fermi level](fermi-level.md)
- [Finite-temperature electron equation of state](finite-temperature-electron-equation-of-state.md)
- [Gibbs free energy](gibbs-free-energy.md)
- [Gross–Pitaevskii equation](gross-pitaevskii-equation.md)
- [Helmholtz free energy](helmholtz-free-energy.md)
- [Kinetic equilibrium](kinetic-equilibrium.md)
- [Linear composition bias leaves coexistence compositions unchanged](linear-composition-bias-leaves-coexistence-compositions-unchanged.md)
- [Maxwell-Boltzmann distribution](maxwell-boltzmann-distribution.md)
- [Maxwell construction](maxwell-construction.md)
- [Maxwell relations](maxwell-relations.md)
- [Membrane transport](membrane-transport.md)
- [Nernst equilibrium potential](nernst-equilibrium-potential.md)
- [Nonrelativistic entropy at zero chemical potential](nonrelativistic-entropy-at-zero-chemical-potential.md)
- [Number density of a relativistic neutrino relative to photons](number-density-of-a-relativistic-neutrino-relative-to-photons.md)
- [Order-parameter mobility](order-parameter-mobility.md)
- [Osmosis](osmosis.md)
- [Ostwald ripening](ostwald-ripening.md)
- [Passive transport](passive-transport.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-39/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-67/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-71/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-71/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-55/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-55/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-1/10d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-4/15d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-4/33b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-61/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-61/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-83/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-83/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-83/2/v/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-83/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-83/4/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-3/34d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-62/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-3/10a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-3/34d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-62/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-62/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-84/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-84/1/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-84/1/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-84/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-84/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-84/4/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-4/33e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-4/34d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-62/3/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-3/15d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-72/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-4/34d/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-4/34d/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-48/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-71/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-42/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-49/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-49/2/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-55/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-81/4/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2/33c/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2/33c/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2/33c/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-53/2/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-310/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2/34d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4/34d/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-305/1/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-310/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-317/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-344/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-1/35a/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-3/36a/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-3/9b/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-344/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3/35d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-310/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-344/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-344/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-344/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-344/3/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-344/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-4/35a/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1/36a/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3/35a/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3/35a/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-344/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-2/37b/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-2/9d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-3/35b/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-4/35b/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-344/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-2/9e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-344/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-344/1/d/ii/solution.md)
- [Phonon](phonon.md)
- [Photon gas](photon-gas.md)
- [Primordial helium response to electron-neutrino degeneracy](primordial-helium-response-to-electron-neutrino-degeneracy.md)
- [Sakharov conditions](sakharov-conditions.md)
- [Solvation free energy](solvation-free-energy.md)
- [Solvation thermodynamic balance](solvation-thermodynamic-balance.md)
- [Standard state](standard-state.md)
- [Thermodynamic limit](thermodynamic-limit.md)
- [Two-component Bose-Einstein condensate](two-component-bose-einstein-condensate.md)
- [Uniform-current pumped polariton condensate](uniform-current-pumped-polariton-condensate.md)
- [Van der Waals liquid-gas coexistence](van-der-waals-liquid-gas-coexistence.md)
- [Zero chemical potential from number-changing reactions](zero-chemical-potential-from-number-changing-reactions.md)
