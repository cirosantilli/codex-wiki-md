# Helmholtz free energy

↑ **Parent:** [Thermodynamic free energy](thermodynamic-free-energy.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Helmholtz_free_energy)

The [Helmholtz free energy](helmholtz-free-energy.md) is

$$
F=U-TS,
$$

where $U$ is [internal energy](internal-energy-split.md), also denoted $E$ elsewhere here, $T$ is absolute [temperature](temperature-split.md), and $S$ is [entropy](entropy-split.md). For the [closed system](closed-system.md) of fixed composition and only [pressure](pressure-split.md)-[volume](volume-thermodynamics.md) [work](work.md) described above, spontaneous relaxation at fixed [temperature](temperature-split.md) and [volume](volume-thermodynamics.md) cannot increase $F$. Stable [thermodynamic equilibrium](thermodynamic-equilibrium.md) is a [global minimum](global-minimum.md) over the permitted alternatives, including different [thermodynamic phases](thermodynamic-phase.md). A rigid vessel fixes the total [volume](volume-thermodynamics.md); it does not require each coexisting [thermodynamic phase](thermodynamic-phase.md) to retain its own [volume](volume-thermodynamics.md).

For a constructed comparison at $300\,\mathrm K$, suppose one candidate has $1.5\,\mathrm{kJ}$ more [internal energy](internal-energy-split.md) but $6\,\mathrm{J\,K^{-1}}$ more [entropy](entropy-split.md) than another at the same [temperature](temperature-split.md) and [volume](volume-thermodynamics.md). Its difference is

$$
\Delta F=1500-300(6)=-300\,\mathrm J.
$$

Thus the candidate with higher [internal energy](internal-energy-split.md) has lower [Helmholtz free energy](helmholtz-free-energy.md). This is the practical reason for retaining the [entropy](entropy-split.md) term when selecting a state.

For equilibrium states within a smooth branch of fixed composition, the [first law of thermodynamics](first-law-of-thermodynamics-split.md) gives $dU=T\,dS-p\,dV$, hence

$$
dF=-S\,dT-p\,dV,\qquad
S=-\left(\frac{\partial F}{\partial T}\right)_V,\qquad
p=-\left(\frac{\partial F}{\partial V}\right)_T.
$$

These [derivatives](derivative.md) extract [entropy](entropy-split.md) and [pressure](pressure-split.md); the differential is not an evolution equation for relaxation. If [chemical species](chemical-species.md) amounts $n_i$ vary, add $\sum_i\mu_i\,dn_i$, with molar [chemical potentials](chemical-potential-split.md) $\mu_i$. A [closed system](closed-system.md) can still change [chemical species](chemical-species.md) amounts through [chemical reactions](chemical-reaction-split.md); the fixed-composition simplification then needs the conserved-inventory constraints of [chemical equilibrium](chemical-equilibrium.md). See [MIT 5.60, Lecture 14, fundamental equations and chemical potentials](https://ocw.mit.edu/courses/5-60-thermodynamics-kinetics-spring-2008/e763a06aa3b5de09cd6bfea6280f219c_5_60_lecture14.pdf).

The minimum principle has a short explanation. At fixed [volume](volume-thermodynamics.md), no boundary [work](work.md) occurs, so $Q=\Delta U$. A [thermal reservoir](heat-bath.md) at positive [temperature](temperature-split.md) $T$ loses [entropy](entropy-split.md) $Q/T$. Consequently

$$
\Delta S_{\rm total}=\Delta S-\frac{\Delta U}{T}=-\frac{\Delta F}{T}\geq0,
$$

by the [Second law of thermodynamics](second-law-of-thermodynamics-split.md). Here both endpoint states share the imposed [temperature](temperature-split.md). See [MIT 5.60, Lecture 12, criteria for spontaneous change](https://ocw.mit.edu/courses/5-60-thermodynamics-kinetics-spring-2008/64efc6f359b20c43dab61fc77791d744_5_60_lecture12.pdf).

The microscopic counterpart is $F=-k_BT\ln Z$ in the [canonical ensemble](canonical-ensemble-split.md), with [Boltzmann constant](boltzmann-constant.md) $k_B$ and [partition function](canonical-partition-function.md) $Z$. The [partition function](canonical-partition-function.md) examples compute the balance between [internal energy](internal-energy-split.md) and [entropy](entropy-split.md); the [chemical equilibrium](chemical-equilibrium.md) example already displays an ideal-mixture [Helmholtz free energy](helmholtz-free-energy.md) minimum.

## ↑ Ancestors (7)

1. [Thermodynamic free energy](thermodynamic-free-energy.md)
2. [Thermodynamic potential](thermodynamic-potential-split.md)
3. [Thermodynamics](thermodynamics-split.md)
4. [Statistical physics](statistical-physics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (96)

- [Abrikosov vortex lattice](abrikosov-vortex-lattice.md)
- [Adsorption confinement free energy](adsorption-confinement-free-energy.md)
- [Chemical equilibrium](chemical-equilibrium.md)
- [Chemical potential and Helmholtz free energy](chemical-potential-and-helmholtz-free-energy.md)
- [Chemical potential of an ideal gas](chemical-potential-of-an-ideal-gas.md)
- [Chemical relaxation time](chemical-relaxation-time.md)
- [Coarse-grained variable](coarse-grained-variable.md)
- [Crooks fluctuation theorem](crooks-fluctuation-theorem.md)
- [Entropic force](entropic-force.md)
- [Entropic spring](entropic-spring.md)
- [Entropy excess of a van der Waals gas](entropy-excess-of-a-van-der-waals-gas.md)
- [Extent of reaction](extent-of-reaction.md)
- [Finite-size rounding](finite-size-rounding.md)
- [Finite-system analyticity](finite-system-analyticity.md)
- [Gibbs free energy](gibbs-free-energy.md)
- [Ginzburg-Landau theory of superconductivity](ginzburg-landau-theory-of-superconductivity.md)
- [Helium-3 pair order parameter](helium-3-pair-order-parameter.md)
- [Helmholtz free energy](helmholtz-free-energy.md)
- [Internal energy of a van der Waals gas](internal-energy-of-a-van-der-waals-gas.md)
- [Limits of adiabatic demagnetization](limits-of-adiabatic-demagnetization.md)
- [Maxwell relations](maxwell-relations.md)
- [Mechanical stability](mechanical-stability.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2021/paper-2/a7/b/solution.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2022/paper-2/a6/d/solution.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2022/paper-2/a8/a/i/solution.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2023/paper-2/a6/a/solution.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2023/paper-2/a8/a/i/solution.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2024/paper-2/a6/a/solution.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2024/paper-2/a8/d/i/solution.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2025/paper-2/a7/a/i/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1/4/a/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1/4/b/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1/5/a/solution.md)
- [Solution](past-exam-of-the-genetics-course-of-the-university-of-cambridge/2024/paper-1/7/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-46/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-46/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-46/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-2/34d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-2/34d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-51/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-76/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-76/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-81/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-303/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-303/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-4/35a/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-344/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-2/35d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3/35d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4/35a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2001/paper-2/10/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2005/paper-2/7/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-2/17/a/solution.md)
- [Solution](past-exam-of-the-mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge/2023/paper-2/section-b/23/iii/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2010/paper-1/section-c/c13/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2011/paper-1/section-a/a3/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2012/paper-2/section-c/c13/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2013/paper-2/section-c/c11/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2018/paper-2/section-c/c10/c/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2018/paper-2/section-c/c10/free-energy-identity/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2019/paper-2/section-c/c10/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1/section-b/b4/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1/section-b/b2/c/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2004/section-b/b8/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2006/section-a/a2/a/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2009/section-a/a2/a/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2009/section-a/a4/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-field-theory-course-of-the-university-of-cambridge/2013/paper-1/3/b/solution.md)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2017/1/a/solution.md)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2022/section-b/4/b/solution.md)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2022/section-b/4/c/solution.md)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2022/section-b/4/d/solution.md)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2022/section-b/4/e/solution.md)
- [Solution](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2022/3/b/solution.md)
- [Solution](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2022/3/c/solution.md)
- [Solution](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2022/3/d/solution.md)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2017/3/a/solution.md)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2017/4/solution.md)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2019/section-b/5/solution.md)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2021/section-a/1/solution.md)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2021/section-b/4/a/solution.md)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2021/section-b/4/b/solution.md)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2021/section-b/4/d/solution.md)
- [Quenched disorder](quenched-disorder.md)
- [Surface correction to thermodynamic free energy](surface-correction-to-thermodynamic-free-energy.md)
- [Thermodynamic equilibrium](thermodynamic-equilibrium.md)
- [Thermodynamic force conjugate to an internal variable](thermodynamic-force-conjugate-to-an-internal-variable.md)
- [Thermodynamic free energy](thermodynamic-free-energy.md)
- [Thermodynamic limit](thermodynamic-limit.md)
- [Thermodynamic potential](thermodynamic-potential-split.md)
- [Thermodynamics of a liquid film](thermodynamics-of-a-liquid-film.md)
- [Thermoelastic Maxwell relation for a stretched band](thermoelastic-maxwell-relation-for-a-stretched-band.md)
- [Thermoelasticity](thermoelasticity.md)
- [Translational partition function](translational-partition-function.md)
- [Two-level paramagnetic cooling model](two-level-paramagnetic-cooling-model.md)
- [Van der Waals liquid-gas coexistence](van-der-waals-liquid-gas-coexistence.md)
