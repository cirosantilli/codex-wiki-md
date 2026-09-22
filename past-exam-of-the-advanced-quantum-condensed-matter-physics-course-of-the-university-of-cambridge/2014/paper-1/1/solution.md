<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A normal [Fermi liquid](../../../../fermi-liquid-split.md) is an interacting fermion phase continuously connected to a [Fermi gas](../../../../fermi-gas.md) without broken symmetry. Its [Landau quasiparticles](../../../../landau-quasiparticle.md) are dressed particle/hole excitations near the [Fermi surface](../../../../fermi-surface.md), with the same conserved quantum numbers, finite [quasiparticle residue](../../../../quasiparticle-residue.md) and a decay width small compared with their excitation energy. Their reference dispersion already includes zero-temperature interaction renormalization; “bare quasiparticle” here does not mean a free atom.[Low-energy quasiparticles and effective dispersion](../../../../the-theory-of-a-fermi-liquid-by-lev-davidovich-landau.md)

The rate assumes $k_BT,|\xi|\ll E_F$, $\xi=\epsilon-\mu$, regular scattering amplitudes and [density of states](../../../../density-of-states.md), equilibrium [Fermi-Dirac distributions](../../../../fermi-dirac-distribution.md), and two-body collisions conserving energy and momentum. [Pauli exclusion principle](../../../../pauli-exclusion-principle.md) restricts the available phase space. It describes a regular three-dimensional normal liquid, not a one-dimensional interacting electron liquid. On the surface, $\tau^{-1}\propto T^2$; at $T=0$ and $\xi>0$, it is proportional to $\xi^2$. Hence excitations become increasingly sharp. The quoted asymmetric occupation factor is for particle out-scattering: a hole decay or full spectral width also needs the complementary in-scattering process; it does not imply exponentially stable deep holes.

Symmetry $f_{ab}=f_{ba}$ cancels the quadratic functional's factor one-half, giving the [thermal Landau quasiparticle energy shift](../../../../thermal-landau-quasiparticle-energy-shift.md)

$$
\boxed{\widetilde\epsilon_a=\epsilon_a+\frac1V\sum_b f_{ab}\delta n_b+O(\delta n^2).}
$$

Here $a=(\mathbf k,\lambda)$, and the derivative is with respect to an occupation, not particle density. Replacing the homogeneous momentum sum by an energy integral defines a smooth angularly averaged kernel $H_a(\epsilon)$. With $\delta n=n_F(\epsilon;\mu,T)-\Theta(\mu_0-\epsilon)$,

$$
\delta\epsilon_a=H_a(\mu_0)\delta\mu+\frac{\pi^2}{6}(k_BT)^2H_a'(\mu_0)+O(T^4).
$$

Fixed density gives $\delta\mu=-(\pi^2/6)(k_BT)^2D'(\mu_0)/D(\mu_0)+O(T^4)$; fixed chemical potential instead has $\delta\mu=0$. Thus **$\widetilde\epsilon_a=\epsilon_a+O(T^2)$** in either case, provided the kernels are smooth and no instability intervenes. This is the [Sommerfeld expansion](../../../../sommerfeld-expansion.md); singular spectra require separate treatment.[§3.6.4, fixed-density Sommerfeld expansion](../../../../statistical-physics-by-david-tong.md)

The leading entropy is therefore that of quasiparticles with their zero-temperature [effective mass](../../../../band-effective-mass.md):

$$
\boxed{C_V/T\longrightarrow\gamma=\frac{\pi^2k_B^2}{3}D^*(\mu_0).}
$$

$D^*$ here is the total, spin-summed [density of states](../../../../density-of-states.md). The plotted low-temperature slopes require the enhanced masses $5.4m$ at molar volume $26.2\,\mathrm{cm^3\,mol^{-1}}$ and $2.7m$ at $36.8\,\mathrm{cm^3\,mol^{-1}}$, rather than the bare-mass predictions. At fixed molar particle number, $\gamma_{\rm mol}\propto m^*V_{\rm mol}^{2/3}$. Agreement is restricted to the low-temperature limit: the measured curves depart markedly from a fixed-mass ideal-gas extrapolation at higher temperature. This supports long-lived quasiparticles with smooth low-energy parameters, but heat capacity alone does not measure their lifetime or prove adiabatic continuity.

## ↑ Ancestors (13)

1. [1](../1.md)
2. [Paper 1](../../paper-1-split.md)
3. [2014](../../split.md)
4. [Past exam of the advanced Quantum Condensed Matter Physics course of the University of Cambridge](../../../split.md)
5. [Advanced Quantum Condensed Matter Physics course of the University of Cambridge](../../../../advanced-quantum-condensed-matter-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
