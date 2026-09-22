<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use a complex pair [order parameter](../../../../order-parameter.md) $\Psi=|\Psi|e^{i\theta}$ with signed charge $q$, $|q|=2e$. A local isotropic [Ginzburg-Landau theory of superconductivity](../../../../ginzburg-landau-theory-of-superconductivity.md) has free [energy](../../../../energy-split.md)

$$
F=\int d^3x\left[\alpha|\Psi|^2+\frac\beta2|\Psi|^4+
\frac{|(-i\hbar\nabla-q\mathbf A)\Psi|^2}{2m_*}+\frac{B^2}{2\mu_0}\right].
$$

For $\alpha<0$, $\beta>0$, the uniform amplitude is $|\Psi_0|^2=-\alpha/\beta$. Variation gives the static field equation and [supercurrent](../../../../supercurrent.md)

$$
\frac{(-i\hbar\nabla-q\mathbf A)^2}{2m_*}\Psi+\alpha\Psi+\beta|\Psi|^2\Psi=0,
\qquad
\mathbf j_s=\frac{q}{m_*}\operatorname{Re}\left[\Psi^*(-i\hbar\nabla-q\mathbf A)\Psi\right].
$$

The [vector potential](../../../../vector-potential.md) obeys Maxwell's equations, including $\nabla\times\mathbf B=\mu_0(\mathbf j_s+\mathbf j_n)+\mu_0\epsilon_0\partial_t\mathbf E$ and $\nabla\times\mathbf E=-\partial_t\mathbf B$, with $\mathbf B=\nabla\times\mathbf A$ and $\mathbf E=-\nabla\phi-\partial_t\mathbf A$. The static approximation drops the displacement current. A common dissipative near-transition dynamical extension is the [time-dependent Ginzburg-Landau equation](../../../../time-dependent-ginzburg-landau-equation.md)

$$
\Gamma\left(\partial_t+\frac{iq\phi}{\hbar}\right)\Psi=-\frac{\delta F}{\delta\Psi^*},\qquad\Gamma>0.
$$

It is a phenomenological relaxation law in its applicable regime, not a universal microscopic Schrödinger equation for every superconductor. Its covariant time derivative and the covariant spatial derivative ensure consistent phase and electromagnetic gauge transformations.

The amplitude and screening lengths are

$$
\xi=\frac{\hbar}{\sqrt{2m_*|\alpha|}},\qquad
\lambda=\sqrt{\frac{m_*}{\mu_0q^2|\Psi_0|^2}},\qquad\kappa=\lambda/\xi.
$$

For $\kappa>1/\sqrt2$ the ideal model is type II. An [Abrikosov vortex](../../../../abrikosov-vortex.md) has a $2\pi n$ phase winding, a core with suppressed $|\Psi|$ of size $\xi$, and circulating screening currents over $\lambda$. Single-valuedness implies [fluxoid and flux quantization in a superconductor](../../../../fluxoid-and-flux-quantization-in-a-superconductor.md):

$$
\Phi+\mu_0\lambda^2\oint\mathbf j_s\cdot d\boldsymbol\ell=n\Phi_0,
\qquad\boxed{\Phi_0=\frac{h}{2e}.}
$$

The sign of $n$ depends on the chosen circulation and charge convention. Far from the core, where the contour current term is negligible, each singly wound vortex carries one flux quantum in magnitude.

The equilibrium [lower critical magnetic field](../../../../lower-critical-magnetic-field.md) marks favorable entry of the first vortex; for $\kappa\gg1$, $\mu_0H_{c1}\simeq[\Phi_0/(4\pi\lambda^2)](\ln\kappa+C)$ with an order-one core correction $C$. The [upper critical magnetic field](../../../../upper-critical-magnetic-field.md) follows by linearizing the order-parameter equation in the field:

$$
\boxed{\mu_0H_{c2}=\frac{\Phi_0}{2\pi\xi^2}.}
$$

Between these fields lies the superconducting mixed state, often with an [Abrikosov vortex lattice](../../../../abrikosov-vortex-lattice.md). The ideal equilibrium entry and exit fields need not yield large irreversible loops. [Flux pinning](../../../../flux-pinning.md) and surface barriers impede vortex motion; field sweeps then retain history-dependent flux and produce [magnetic hysteresis](../../../../magnetic-hysteresis.md) and dissipative losses.

A [superconducting weak link](../../../../superconducting-weak-link.md), such as a tunnel junction or narrow constriction, couples the phases of two superconductors. With consistent choices of phase and voltage orientation, the [Josephson effect](../../../../josephson-effect.md) gives

$$
\boxed{I_s=I_c\sin\delta,\qquad\hbar\dot\delta=2eV,\qquad f_J=\frac{2e|V|}{h}.}
$$

The [Gauge-invariant Josephson phase](../../../../gauge-invariant-josephson-phase.md) includes the line integral of $\mathbf A$ across the link. A zero voltage can sustain a phase-dependent steady current; a constant nonzero voltage makes that contribution oscillate. Microwave irradiation can lock this oscillation to an applied [frequency](../../../../frequency.md), giving voltage steps at $V_n=nhf/(2e)$, an experimental test of coherent pair transport rather than an ordinary resistive current law.

A [DC SQUID](../../../../dc-squid.md) places two weak links in a loop. For identical junction critical currents $I_0$ and negligible self-inductance, flux quantization fixes their relative phase difference to $2\pi\Phi_{\rm ext}/\Phi_0$. Adding the two sinusoidal currents and maximizing over their common phase gives

$$
\boxed{I_{c,\rm SQUID}=2I_0\left|\cos\left(\frac{\pi\Phi_{\rm ext}}{\Phi_0}\right)\right|.}
$$

The flux-periodic response provides sensitive magnetic measurements. Junction asymmetry or appreciable loop inductance changes the ideal contrast and can introduce additional hysteresis; the phase-coherent [interference](../../../../interference-wave-propagation.md) principle remains. The [Jaklevic Josephson interference experiment](../../../../jaklevic-josephson-interference-experiment.md) is a motivating experimental realization of this link between a superconducting loop, weak links and [magnetic flux](../../../../magnetic-flux.md).

## ↑ Ancestors (13)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [2013](../../split.md)
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
