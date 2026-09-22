# Single-electron superconducting tunneling

↑ **Parent:** [Superconductivity](superconductivity-split.md)

[Single-electron superconducting tunneling](single-electron-superconducting-tunneling.md) transfers individual [electrons](electron.md) across a barrier into or out of [quasiparticle](quasiparticle.md) states of a material with [superconductivity](superconductivity-split.md). In a normal-metal–insulator–superconductor junction, abbreviated NIS, only one electrode has [superconductivity](superconductivity-split.md). Such a junction can reveal a [superconducting energy gap](superconducting-energy-gap.md) without supporting a [DC Josephson effect](dc-josephson-effect.md) between two superconducting reservoirs.

For an elementary interpretation, assume an opaque barrier, approximately constant normal-electrode [density of states](density-of-states.md), and an energy-independent tunneling matrix element over the range probed. Write the superconducting [density of states](density-of-states.md) divided by its normal-state value as $n_s(E)$, with $E$ measured from its [chemical potential](chemical-potential-split.md). A signed voltage convention chosen for positive normal-electrode injection gives

$$
I_{\rm qp}(V)=\frac{1}{eR_N}\int_{-\infty}^{\infty}n_s(E)\,[f(E-eV)-f(E)]\,dE,
$$

where $f$ is the [Fermi-Dirac distribution](fermi-dirac-distribution.md) at a common [temperature](temperature-split.md) and $R_N$ is the normal-state junction [electrical resistance](electrical-resistance.md). This current convention is local to the NIS measurement. The expression counts occupied initial and empty final states; it is a quasiparticle transport model, not a [current-phase relation of a superconducting weak link](current-phase-relation-of-a-superconducting-weak-link.md).

An original analytic illustration uses the ideal fully gapped [BCS theory](bcs-theory.md) spectrum at zero [temperature](temperature-split.md), with positive gap edge $\Delta$:

$$
n_s(E)=\begin{cases}0,&|E|<\Delta,\\ |E|/\sqrt{E^2-\Delta^2},&|E|>\Delta.\end{cases}
$$

For positive $V$, the occupation difference restricts the [integral](integral-split.md) to $0<E<eV$. Since $d\sqrt{E^2-\Delta^2}/dE=E/\sqrt{E^2-\Delta^2}$, integration and odd extension give

$$
I_{\rm qp}(V)=\begin{cases}0,& |eV|\leq\Delta,\\ \displaystyle\frac{\operatorname{sgn}(V)}{eR_N}\sqrt{(eV)^2-\Delta^2},& |eV|>\Delta.\end{cases}
$$

The threshold is $\Delta/e$ for this NIS model. In the corresponding zero-temperature single-electron process between two fully gapped superconductors, creating excitations on both sides instead requires $|eV|\geq\Delta_1+\Delta_2$. That quasiparticle threshold does not forbid coherent pair [electric current](electric-current.md) below it. At finite [temperature](temperature-split.md), thermally populated [quasiparticles](quasiparticle.md) soften the simple threshold argument.

At zero [temperature](temperature-split.md) in the NIS approximation, $R_N\,dI_{\rm qp}/dV=n_s(eV)$ away from the singular gap edge. Thus a voltage sweep probes the excitation [density of states](density-of-states.md). The ideal divergence is rounded in real measurements, and at nonzero [temperature](temperature-split.md) the [derivative](derivative.md) samples a thermally broadened range of [energies](energy-split.md). For $|eV|>\Delta$, the model has $VI_{\rm qp}>0$: electrical work creates excitations and is dissipated on relaxation. This distinguishes its steady transport from the conservative [Josephson coupling energy](josephson-coupling-energy.md).

**Table of contents**

- [Giaever gap experiment](giaever-gap-experiment.md)

## ↑ Ancestors (5)

1. [Superconductivity](superconductivity-split.md)
2. [Statistical physics](statistical-physics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (5)

- [AC Josephson effect](ac-josephson-effect.md)
- [Josephson junction](josephson-junction.md)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2017/1/a/solution.md)
- [Quantum escape of a current-biased Josephson junction](quantum-escape-of-a-current-biased-josephson-junction.md)
- [Single-electron superconducting tunneling](single-electron-superconducting-tunneling.md)
