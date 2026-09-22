# Thermodynamic limit

↑ **Parent:** [Statistical physics](statistical-physics-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Thermodynamic_limit)

The [thermodynamic limit](thermodynamic-limit.md) describes a sequence of larger systems, not a single enormous specimen: particle number $N$ and [volume](volume-thermodynamics.md) $V$ tend to infinity with [number density](number-density.md) $n=N/V$ fixed. Hold the chosen [intensive and extensive thermodynamic quantities](intensive-and-extensive-thermodynamic-quantities.md) such as [temperature](temperature-split.md) $T$ and an applied [magnetic field](magnetic-field-split.md) fixed along that sequence. In the [canonical ensemble](canonical-ensemble-split.md) the controls are $T,N,V$; in the [grand canonical ensemble](grand-canonical-ensemble.md) one instead fixes $T$ and [chemical potential](chemical-potential-split.md), and the limiting [number density](number-density.md) is a result, possibly with a jump at [phase coexistence](phase-coexistence.md). These are different specifications of a limiting experiment.

The useful limit is usually an [intensive and extensive thermodynamic quantities](intensive-and-extensive-thermodynamic-quantities.md) normalization of the [Helmholtz free energy](helmholtz-free-energy.md), not a finite limit of the total [extensive quantity](extensive-quantity.md) itself:

$$
F_{N,V}=-k_BT\log Z_{N,V},\qquad
f(T,n)=\lim_{\substack{N,V\to\infty\\N/V=n}}\frac{F_{N,V}}{V},\qquad
a(T,n)=\lim_{\substack{N,V\to\infty\\N/V=n}}\frac{F_{N,V}}{N}=\frac{f(T,n)}n.
$$

Here $Z_{N,V}$ is the [canonical partition function](canonical-partition-function.md), $k_B$ is the [Boltzmann constant](boltzmann-constant.md), $f$ is [free-energy density](free-energy-density.md), and $a$ is [Helmholtz free energy](helmholtz-free-energy.md) per particle. Thus $F_{N,V}=Vf+o(V)$ when the limit exists; finite systems need not be exactly [extensive quantities](extensive-quantity.md) because of the [surface correction to thermodynamic free energy](surface-correction-to-thermodynamic-free-energy.md).

Specify the interactions and the growing containers too. For a conventional fluid, use a fixed [stable pair potential](stable-pair-potential.md) with a [tempered pair potential](tempered-pair-potential.md) tail, and containers whose boundary layer of any fixed thickness occupies a vanishing fraction of the [volume](volume-thermodynamics.md); uniformly enlarged cubes work, a tube of fixed cross-section does not give the same bulk limit. For a finite-range [Ising model](ising-model.md), keep the [lattice](lattice.md) spacing and bond coupling fixed while enlarging all intended spatial directions. Ordinary bounded wall interactions or [periodic boundary conditions](periodic-boundary-conditions.md) can then give the same bulk [free-energy density](free-energy-density.md), although [boundary conditions](boundary-condition.md) can select different [spontaneous symmetry breaking](spontaneous-symmetry-breaking.md) states. This is a set of hypotheses, not a theorem that every interaction has a boundary-independent limit.[§V.F, printed pp. 55–57: stable and tempered interactions and existence of the thermodynamic limit](the-large-deviation-approach-to-statistical-mechanics-by-hugo-touchette.md)

The [Curie–Weiss model](curie-weiss-model.md) below deliberately uses a different limiting prescription: its all-to-all coupling is divided by $N$. Without that factor its interaction [energy](energy-split.md) would grow as $N^2$, rather than as an [extensive quantity](extensive-quantity.md). The model has no spatial wall or [correlation length](correlation-length.md) to compare with a container; it is an exactly summable illustration of [finite-size rounding](finite-size-rounding.md), not a quantitative model of the fluid experiment below.

**Table of contents**

- [Relative fluctuations of an extensive observable](relative-fluctuations-of-an-extensive-observable.md)
- [Finite-system analyticity](finite-system-analyticity.md)
- [Symmetry-breaking order of limits](symmetry-breaking-order-of-limits.md)
- [Finite-size rounding](finite-size-rounding.md)
- [Surface correction to thermodynamic free energy](surface-correction-to-thermodynamic-free-energy.md)
- [Carbon-dioxide viewing-cell phase-transition experiment](carbon-dioxide-viewing-cell-phase-transition-experiment.md)
- [Critical opalescence](critical-opalescence.md)
- [Stable pair potential](stable-pair-potential.md)
- [Tempered pair potential](tempered-pair-potential.md)

## ↑ Ancestors (4)

1. [Statistical physics](statistical-physics-split.md)
2. [Branches of physics](branches-of-physics.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (73)

- [Berezinskii–Kosterlitz–Thouless transition](berezinskii-kosterlitz-thouless-transition.md)
- [Carbon-dioxide viewing-cell phase-transition experiment](carbon-dioxide-viewing-cell-phase-transition-experiment.md)
- [Constrained order-parameter free energy](constrained-order-parameter-free-energy.md)
- [Energy gap](energy-gap.md)
- [Extensive quantity](extensive-quantity.md)
- [Fermi energy](fermi-energy.md)
- [Fermi sea](fermi-sea.md)
- [Finite-scale vortex renormalization](finite-scale-vortex-renormalization.md)
- [Gaussian variational kernel for a gradient quartic interaction](gaussian-variational-kernel-for-a-gradient-quartic-interaction.md)
- [Ising-chain domain-wall energy convention](ising-chain-domain-wall-energy-convention.md)
- [Ising ring magnetization fluctuations](ising-ring-magnetization-fluctuations.md)
- [Magnetization scaling-function matching](magnetization-scaling-function-matching.md)
- [Microcanonical energy-shell entropy](microcanonical-energy-shell-entropy.md)
- [Open-chain endpoint corrections for an exponential Ising kernel](open-chain-endpoint-corrections-for-an-exponential-ising-kernel.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-3/47/c/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-3/47/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-72/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-72/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-64/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-69/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-69/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-69/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-69/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-46/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-46/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-46/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-46/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-46/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-46/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-51/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-51/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-51/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-50/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-59/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-43/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-1/35d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-49/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-75/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-42/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-303/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4/34d/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-303/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-303/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-1/35a/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-4/35a/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-344/1/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-344/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4/35a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-337/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-344/1/e/solution.md)
- [Solution](past-exam-of-the-phase-transitions-and-collective-phenomena-course-of-the-university-of-cambridge/2012/paper-1/1/a/solution.md)
- [Solution](past-exam-of-the-phase-transitions-and-collective-phenomena-course-of-the-university-of-cambridge/2012/paper-1/3/c/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2019/paper-2/section-c/c13/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-field-theory-course-of-the-university-of-cambridge/2015/paper-1/1/e/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-field-theory-course-of-the-university-of-cambridge/2015/paper-1/3/b/solution.md)
- [Solution](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2016/paper-1/4/b/solution.md)
- [Solution](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2022/3/d/solution.md)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2012/paper-1/2/c/solution.md)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2015/paper-1/2/b/solution.md)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2017/2/b/solution.md)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2018/section-b/b4/solution.md)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2019/section-a/2/solution.md)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2021/section-b/5/a/solution.md)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2021/section-b/5/e/solution.md)
- [Pure thermodynamic phase](pure-thermodynamic-phase.md)
- [Replica trick](replica-trick.md)
- [Spontaneous symmetry breaking](spontaneous-symmetry-breaking.md)
- [Stable pair potential](stable-pair-potential.md)
- [Surface correction to thermodynamic free energy](surface-correction-to-thermodynamic-free-energy.md)
- [Symmetry-breaking order of limits](symmetry-breaking-order-of-limits.md)
- [Tempered pair potential](tempered-pair-potential.md)
- [Thermodynamic limit](thermodynamic-limit.md)
- [Two-electron Laughlin relative probability](two-electron-laughlin-relative-probability.md)
