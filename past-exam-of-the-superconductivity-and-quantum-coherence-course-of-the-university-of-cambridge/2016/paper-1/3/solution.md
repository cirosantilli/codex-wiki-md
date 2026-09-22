<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

[Ginzburg-Landau theory of superconductivity](../../../../ginzburg-landau-theory-of-superconductivity.md) organizes a continuous superconducting transition through a slowly varying complex [order parameter](../../../../order-parameter.md). In the simplest isotropic single-component SI model,

$$
F-F_n=\int d^3x\left[\alpha|\psi|^2+\frac\beta2|\psi|^4+\frac{|(-i\hbar\nabla-q\mathbf A)\psi|^2}{2m_*}+\frac{|\mathbf B|^2}{2\mu_0}\right],
\qquad \mathbf B=\nabla\times\mathbf A.
$$

Here $\beta>0$, $m_*>0$, $\alpha$ changes sign at $T_c$, and $q=-2e$ fixes a charge/phase convention. The phenomenological normalization of $\psi$ determines the coefficient values; it should not be confused without qualification with a literal density of independently identifiable pairs.

[Microscopic derivation of Ginzburg-Landau theory](../../../../microscopic-derivation-of-ginzburg-landau-theory.md) expands the BCS response near $T_c$ in small gap amplitude and slow spatial gradients. It identifies the complex order parameter with a scaled pair amplitude, supplies the coefficients from the electronic microscopic parameters, and explains the pair charge in the gauge coupling. The agreement is a controlled near-transition limit, not a statement that the truncated local functional remains exact at all temperatures. [Lev Gor'kov](../../../../lev-gor-kov.md) established this connection explicitly in 1959.[1959 abstract and derivation: near-$T_c$ reduction and twice-electron charge](../../../../microscopic-derivation-of-the-ginzburg-landau-equations-in-the-theory-of-superconductivity-by-lev-gor-kov.md)

Below the transition, minimization gives $|\psi_0|^2=-\alpha/\beta$ and condensation-energy density $\alpha^2/(2\beta)$. A variation with respect to $\psi^*$ gives

$$
\frac{(-i\hbar\nabla-q\mathbf A)^2}{2m_*}\psi+\alpha\psi+\beta|\psi|^2\psi=0.
$$

Variation with respect to $\mathbf A$ gives the [supercurrent](../../../../supercurrent.md)

$$
\mathbf j=\frac{q\hbar}{m_*}\operatorname{Im}(\psi^*\nabla\psi)-\frac{q^2}{m_*}|\psi|^2\mathbf A,
$$

coupled to the [magnetostatic Ampère law](../../../../magnetostatic-ampere-law.md). For nearly uniform amplitude this reduces to [London screening](../../../../london-screening.md) and the [Meissner effect](../../../../meissner-effect.md). The theory supplies two different length scales:

$$
\xi^2=\frac{\hbar^2}{2m_*|\alpha|},\qquad
\lambda^2=\frac{m_*}{\mu_0q^2|\psi_0|^2},\qquad \kappa=\frac\lambda\xi.
$$

The amplitude can vary over the [superconducting coherence length](../../../../superconducting-coherence-length.md), whereas the [magnetic field](../../../../magnetic-field-split.md) is screened over the [London penetration depth](../../../../london-penetration-depth.md).

The surface-energy distinction at $\kappa=1/\sqrt2$ explains why type-I and type-II behavior are possible within the same framework. In the type-II regime, quantized winding produces an [Abrikosov vortex](../../../../abrikosov-vortex.md) with a finite core and circulating current. Periodic solutions yield an [Abrikosov vortex lattice](../../../../abrikosov-vortex-lattice.md). Linearization about the normal state gives $B_{c2}=\Phi_0/(2\pi\xi^2)$, while core and field energetics determine the lower entry field. These predictions connect a spatial field theory to measurable vortex patterns and critical fields, beyond a spatially uniform BCS gap equation. Thin-film critical-field observations helped motivate the large-$\kappa$ regime; magnetic-decoration experiments subsequently made vortex positions visible.[pp.975–977, film motivation, mixed-state solutions and experimental vortex evidence](../../../../nobel-lecture-type-ii-superconductors-and-the-vortex-lattice-by-alexei-alexeyevich-abrikosov.md)

These phenomena also enable applications. Type-II conductors support high-field magnets, but [flux pinning](../../../../flux-pinning.md) is needed to limit vortex-motion losses. Phase coherence and fluxoid quantization permit persistent-current loops and interference devices. A weak link supplies [Josephson coupling energy](../../../../josephson-coupling-energy.md), allowing SQUID magnetometry and nonlinear quantum circuits; a junction's detailed current–phase law requires a weak-link model, rather than following automatically from the spatially uniform bulk functional. Microstructure can raise a useful critical current without greatly changing the equilibrium upper field, illustrating the difference between thermodynamic stability and transport performance.

The simple functional has identifiable limits. Far below $T_c$, the small-gap expansion is uncontrolled; rapidly varying fields can require nonlocal microscopic electrodynamics. Very near a transition in a fluctuating low-dimensional or strongly anisotropic material, mean-field minimization can miss important thermal or quantum fluctuations. Unconventional or multiband pairing can require several order-parameter components and additional gradient couplings. Strong fields can introduce spin-polarization pair breaking omitted by the orbital model. Finally, the static functional predicts equilibrium extrema, not quasiparticle spectra, dissipation, vortex velocities or a unique amplitude-mode frequency without further dynamical input. These are reasons to choose an appropriate extension or a microscopic calculation, not reasons to discard the successful near-transition predictions.

## ↑ Ancestors (13)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [2016](../../split.md)
4. [Past exam of the superconductivity and Quantum Coherence course of the University of Cambridge](../../../split.md)
5. [Superconductivity and Quantum Coherence course of the University of Cambridge](../../../../superconductivity-and-quantum-coherence-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
