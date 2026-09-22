<h1 id="schrodinger-equation">Schrödinger equation</h1>

↑ **Parent:** [Mathematical physics](mathematical-physics-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Schrödinger_equation)

The [Schrödinger equation](schrodinger-equation.md) governs the evolution of a [quantum state](quantum-state.md) between instances of [measurement in quantum mechanics](quantum-measurement-split.md). For a particle of [mass](mass.md) $m>0$ moving in a prescribed real [potential energy](potential-energy.md) $V(\mathbf r,t)$, its position [wavefunction](wave-function-split.md) satisfies

$$
i\hbar\frac{\partial\psi}{\partial t}=H(t)\psi,
\qquad H(t)=-\frac{\hbar^2}{2m}\nabla^2+V(\mathbf r,t),
\qquad \hbar=\frac{h}{2\pi}.
$$

Here $h$ is the [Planck constant](planck-constant.md), $\nabla^2$ is the [Laplace operator](laplace-operator.md), and the [Hamiltonian operator](hamiltonian-quantum-mechanics.md) combines [kinetic energy](kinetic-energy.md) with [potential energy](potential-energy.md). Specify an initial [wavefunction](wave-function-split.md), an [operator domain](operator-domain.md) and any [boundary conditions](boundary-condition.md): the differential expression alone does not completely specify a physical model. The [Born rule](born-rule.md) then turns the evolving [probability amplitude](probability-amplitude.md) into position [probabilities](probability.md) through $\rho=|\psi|^2$ and integration over a region.

This scalar [Schrödinger operator](schrodinger-operator.md) describes [nonrelativistic quantum mechanics](nonrelativistic-quantum-mechanics.md), with relevant [momenta](momentum-split.md) much smaller than $mc$, where $c$ is the [speed of light](speed-of-light.md). It omits the constant rest [energy](energy-split.md) $mc^2$, assumes fixed particle number, and suppresses active [spin](spin.md) dynamics and coupling to a [magnetic vector potential](magnetic-vector-potential.md). A free [electron](electron.md) with a fixed, uncoupled [spin](spin.md) state can still use this scalar model; the [Pauli equation](pauli-equation.md) supplies the additional [spin](spin.md) components and magnetic coupling when needed. A prescribed real $V$ describes a closed evolution model or an approximation in which the source of that [potential energy](potential-energy.md) is treated as external. Dissipation, particle creation and a general [measurement in quantum mechanics](quantum-measurement-split.md) need further modelling.

For a time-independent [self-adjoint](self-adjoint-operator.md) [Hamiltonian operator](hamiltonian-quantum-mechanics.md), the [spectral theorem](spectral-theorem.md) defines [unitary time evolution](unitary-time-evolution.md) by

$$
\psi(t)=e^{-iHt/\hbar}\psi(0),\qquad
\|\psi(t)\|^2=\|\psi(0)\|^2.
$$

Initial states in the [operator domain](operator-domain.md) satisfy the differential equation in the [Hilbert space](hilbert-space-split.md) sense; the [unitary operator](unitary-operator.md) also evolves all other states in that [Hilbert space](hilbert-space-split.md). Time-dependent [Hamiltonian operators](hamiltonian-quantum-mechanics.md) need suitable regularity and domain hypotheses; their evolution is not generally the exponential of $-itH(t)/\hbar$.

The local reason for conservation is especially tangible. Multiply the [Schrödinger equation](schrodinger-equation.md) by the [complex conjugate](complex-conjugate.md) $\psi^*$, subtract its conjugate multiplied by $\psi$, and use the fact that the real [potential energy](potential-energy.md) terms cancel. For smooth [wavefunctions](wave-function-split.md) this gives the [probability continuity equation](probability-continuity-equation.md)

$$
\partial_t\rho+\nabla\cdot\mathbf j=0,\qquad
\mathbf j=\frac{\hbar}{m}\operatorname{Im}(\psi^*\nabla\psi).
$$

The [divergence theorem](divergence-theorem.md) identifies the change in probability inside a region with minus the outward [probability current](probability-current.md). Decay at infinity, or appropriate probability-conserving [boundary conditions](boundary-condition.md), preserves [wavefunction normalization](wavefunction-normalization.md). Conservation of total probability does not require a stationary [probability density](probability-density.md).

Its usefulness comes from being a [linear partial differential equation](linear-partial-differential-equation.md): [quantum superpositions](quantum-superposition.md) of solutions are solutions, while different [quantum phases](quantum-phase.md) can produce [interference](interference-wave-propagation.md). For a fixed [Hamiltonian operator](hamiltonian-quantum-mechanics.md), the [time-independent Schrödinger equation](time-independent-schrodinger-equation.md) finds the [energy eigenstates](energy-eigenstate.md); each then acquires just its own time-dependent [quantum phase](quantum-phase.md). One [eigenvalue problem](eigenvalue-problem.md) therefore organizes both allowed [energies](energy-split.md) and the evolution of arbitrary [quantum superpositions](quantum-superposition.md), with a [continuous spectrum](continuous-spectrum.md) included when required. This is the attractive bridge between a spatial wave problem and a clock: [energy](energy-split.md) differences determine the rate at which relative [quantum phases](quantum-phase.md) change. It makes atomic [spectral lines](spectral-line.md), [quantum tunnelling](quantum-tunnelling.md) and [quantum scattering](quantum-scattering-split.md) calculable from a specified model.

For an explicit example without confinement, take a [free particle](free-particle.md) on the whole line, $V=0$, initially in a [Gaussian wave packet](gaussian-wave-packet.md) with position [standard deviation](standard-deviation.md) $\sigma_0$ and mean [momentum](momentum-split.md) $\hbar k_0$:

$$
\psi(x,0)=\frac{e^{-x^2/(4\sigma_0^2)+ik_0x}}{(2\pi\sigma_0^2)^{1/4}},\qquad
t_s=\frac{2m\sigma_0^2}{\hbar},\quad \tau=\frac{t}{t_s},\quad v_0=\frac{\hbar k_0}{m}.
$$

Unlike a single [plane wave](plane-wave.md), this [wavefunction](wave-function-split.md) satisfies [wavefunction normalization](wavefunction-normalization.md). A [Fourier transform](fourier-transform-split.md) writes it as a [quantum superposition](quantum-superposition.md) of [plane waves](plane-wave.md). Their [dispersion relation](dispersion-relation-split.md) is $\omega(k)=\hbar k^2/(2m)$, so each Fourier component gains the factor $e^{-i\hbar k^2t/(2m)}$. Completing the square in the resulting [Gaussian integral](gaussian-integral.md) gives

$$
\psi(x,t)=\frac{1}{(2\pi\sigma_0^2)^{1/4}\sqrt{1+i\tau}}
\exp\!\left[-\frac{(x-v_0t)^2}{4\sigma_0^2(1+i\tau)}+ik_0x-\frac{i\hbar k_0^2t}{2m}\right],
$$

with the square root chosen continuously from $t=0$. Its position [probability density](probability-density.md) and [standard deviation](standard-deviation.md) are

$$
\rho(x,t)=\frac{\exp[-(x-v_0t)^2/(2\sigma_t^2)]}{\sqrt{2\pi}\,\sigma_t},\qquad
\sigma_t=\sigma_0\sqrt{1+\tau^2}.
$$

The centre moves with the [group velocity](group-velocity.md) $\omega'(k_0)=v_0$ and the [wave packet](wave-packet.md) spreads because different [wavenumbers](wavenumber.md) have different [group velocities](group-velocity.md). This is unitary [wave dispersion](wave-dispersion.md), without a random [force](force-split.md) or loss of probability. Independently, the initial [momentum](momentum-split.md) [standard deviation](standard-deviation.md) is $\Delta p=\hbar/(2\sigma_0)$ and the initial position-momentum [covariance](covariance.md) vanishes. Free evolution gives $x(t)=x(0)+p(0)t/m$ in the [Heisenberg picture](heisenberg-picture.md), hence

$$
\sigma_t^2=\sigma_0^2+\frac{t^2}{m^2}(\Delta p)^2
=\sigma_0^2+\frac{\hbar^2t^2}{4m^2\sigma_0^2}.
$$

This independently checks the spreading law. The [Gaussian integral](gaussian-integral.md) of $\rho$ is one at every time; the decreasing peak is exactly offset by increasing width.

As hypothetical preparation parameters, choose a free [electron](electron.md) with $\sigma_0=1\,\mathrm{nm}$ and $k_0=2\,\mathrm{nm}^{-1}$. Using $\hbar\simeq1.054571817\times10^{-34}\,\mathrm{J\,s}$ and $m\simeq9.1093837\times10^{-31}\,\mathrm{kg}$ gives

$$
t_s\simeq17.276\,\mathrm{fs},\qquad
v_0\simeq2.31535\times10^5\,\mathrm{m\,s^{-1}},\qquad
\Delta p\simeq5.27286\times10^{-26}\,\mathrm{kg\,m\,s^{-1}}.
$$

The rounded [electron](electron.md) [mass](mass.md) uses the 2022 adjustment.[Electron mass, 2022 CODATA adjustment; rounded here to eight significant figures](codata-value-electron-mass-by-national-institute-of-standards-and-technology.md) At $t=t_s$, the centre is $4\,\mathrm{nm}$ and $\sigma_t=\sqrt2\,\mathrm{nm}$; at $t=2t_s$, they are $8\,\mathrm{nm}$ and $\sqrt5\,\mathrm{nm}$. The mean [kinetic energy](kinetic-energy.md) stays

$$
\langle H\rangle=\frac{\hbar^2}{2m}\left(k_0^2+\frac{1}{4\sigma_0^2}\right)\simeq0.1619\,\mathrm{eV}.
$$

It includes both mean motion and the [momentum](momentum-split.md) spread. The mean speed is about $7.72\times10^{-4}c$ and the [momentum](momentum-split.md) spread corresponds to $1.93\times10^{-4}c$, making the nonrelativistic model accurate for the appreciably occupied part of this ideal [Gaussian distribution](normal-distribution.md). Its mathematically unbounded tails are an idealization.

<a id="image-translation-and-spreading-of-a-free-gaussian-wave-packet"></a>
![](schrodinger-free-gaussian-spreading.png)

**[Figure 11](#image-translation-and-spreading-of-a-free-gaussian-wave-packet). Translation and spreading of a free Gaussian wave packet**. [Source](schrodinger-free-gaussian-spreading.py). Calculated [electron](electron.md) position [probability densities](probability-density.md) for the hypothetical $1\,\mathrm{nm}$ preparation above, together with the position [standard deviation](standard-deviation.md). The area under every curve is one. The dashed width curve illustrates pure translation without spreading for comparison; it is not the free solution. No curve represents measured data.

The complex width also explains where the probability goes. Write $\psi=\sqrt\rho\,e^{i\theta}$, where $\theta$ is the dimensionless [quantum phase](quantum-phase.md). Differentiating the exact solution gives

$$
\partial_x\theta=k_0+\frac{\tau(x-v_0t)}{2\sigma_0^2(1+\tau^2)},\qquad
\frac{j}{\rho}=\frac{\hbar}{m}\partial_x\theta
=v_0+\frac{t}{t_s^2+t^2}(x-v_0t).
$$

Relative to the moving centre, the [probability current](probability-current.md) $j_{\mathrm{rel}}=j-v_0\rho$ points outward on both sides for $t>0$. This is a flux statement, not an additional assumption about individual particle trajectories. At $t=t_s$ and $x-v_0t=\pm\sigma_0$, the relative flow speeds $j_{\mathrm{rel}}/\rho$ are $\pm\sigma_0/(2t_s)$, about $\pm2.8942\times10^4\,\mathrm{m\,s^{-1}}$. The probability within a moving interval of half-width $\sigma_0$ falls from about $0.6827$ initially to $0.5205$ at $t_s$, exactly because of this outward [probability current](probability-current.md).

<a id="image-curved-quantum-phase-drives-spreading-probability-current"></a>
![](schrodinger-gaussian-phase-current.png)

**[Figure 12](#image-curved-quantum-phase-drives-spreading-probability-current). Curved quantum phase drives spreading probability current**. [Source](schrodinger-gaussian-phase-current.py). The same free [Gaussian wave packet](gaussian-wave-packet.md) at $t=t_s$. With $y=(x-v_0t)/\sigma_0$, removing the carrier $k_0x$ and a spatially constant [quantum phase](quantum-phase.md) leaves $y^2/8$. The right panel plots $t_sj_{\mathrm{rel}}=(\sigma_0\rho)y/2$: negative to the left, positive to the right. Flux through the marked moving interval endpoints explains its decreasing probability.

Historically, the 1926 [Quantisierung als Eigenwertproblem (Erste Mitteilung) by Erwin Schrödinger](quantisierung-als-eigenwertproblem-erste-mitteilung-by-erwin-schrodinger.md) began with the stationary [hydrogen atom](hydrogen-atom.md) problem. It distinguishes discrete negative [energies](energy-split.md) from a positive [continuous spectrum](continuous-spectrum.md); it is not yet the general evolution equation displayed above.[Printed pp. 361–363, especially p. 362: discrete and continuous spectrum](quantisierung-als-eigenwertproblem-erste-mitteilung-by-erwin-schrodinger.md) The opening of [quantum mechanics](quantum-mechanics-split.md) discusses its original vibrating-string analogy.

In the 12 December 1933 lecture [The fundamental idea of wave mechanics by Erwin Schrödinger](nobel-lectures-physics-1922-1941/the-fundamental-idea-of-wave-mechanics-by-erwin-schrodinger.md), [Erwin Schrödinger](erwin-schrodinger.md) explains the move from independent rays to waves through [diffraction](diffraction.md), then applies that analogy to [atomic physics](atomic-physics-split.md). His closing pages explicitly acknowledge the difficulty of reconciling wave language with observed particle tracks. This retrospective physical argument motivates the model; it does not derive the modern [Born rule](born-rule.md) from [classical mechanics](classical-mechanics-split.md).[Nobel Lectures, Physics 1922–1941, printed pp. 313–316; inspected in the Columbia University mirror](nobel-lectures-physics-1922-1941/the-fundamental-idea-of-wave-mechanics-by-erwin-schrodinger.md)

The dates separate proposal from measurement: the [de Broglie wavelength](de-broglie-wavelength.md) belongs to the 1924 thesis, the [Schrödinger equation](schrodinger-equation.md) to 1926, and the [Davisson–Germer experiment](davisson-germer-experiment.md)'s [electron diffraction](electron-diffraction.md) beams to 1927.[Printed pp. 389–390: 1924 proposal, deliberate 1926 search and early-1927 diffraction discovery](the-discovery-of-electron-waves-by-clinton-j-davisson.md) That linked experiment describes the prepared [nickel](nickel.md) crystal, evacuated [electron](electron.md) gun, angular collector scans, retarding-potential selection and heating controls. Its measured collector [electric current](electric-current.md) tests wave-dependent scattering probabilities; it neither measures a [wavefunction](wave-function-split.md) directly nor establishes this equation uniquely.

**Table of contents**

- [Radial Schrödinger equation for a central potential](radial-schrodinger-equation-for-a-central-potential.md)
- [Pauli equation](pauli-equation.md)
  - [Zero modes of a positive transverse Pauli field](zero-modes-of-a-positive-transverse-pauli-field.md)
- [Free Schrodinger equation](free-schrodinger-equation.md)
- [Time-independent Schrödinger equation](time-independent-schrodinger-equation.md)
  - [Inverse construction of a quantum potential](inverse-construction-of-a-quantum-potential.md)
  - [Classically forbidden region](classically-forbidden-region.md)
  - [Classically allowed region](classically-allowed-region.md)
  - [Wavefunction matching at a finite potential step](wavefunction-matching-at-a-finite-potential-step.md)
    - [Bound-state matching in a symmetric stepped well](bound-state-matching-in-a-symmetric-stepped-well.md)
    - [Quantum quarter-wave matching layer](quantum-quarter-wave-matching-layer.md)
  - [Schrödinger operator](schrodinger-operator.md)
  - [Bound-state quantization condition](bound-state-quantization-condition.md)
- [Time-dependent Schrödinger equation](time-dependent-schrodinger-equation.md)
  - [Madelung equations](madelung-equations.md)
- [Nondegeneracy of one-dimensional bound states](nondegeneracy-of-one-dimensional-bound-states.md)

## ↑ Ancestors (3)

1. [Mathematical physics](mathematical-physics-split.md)
2. [Physics](physics-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (169)

- [Barnett equivalent magnetic field](barnett-equivalent-magnetic-field.md)
- [Barrier-top scattering](barrier-top-scattering.md)
- [Boundary force in an infinite square well](boundary-force-in-an-infinite-square-well.md)
- [Circular-orbit derivation of the Bohr model](circular-orbit-derivation-of-the-bohr-model.md)
- [Driven two-level Rabi model](driven-two-level-rabi-model.md)
- [Dynamical phase](dynamical-phase.md)
- [Energy eigenstate](energy-eigenstate.md)
- [Erwin Schrödinger](erwin-schrodinger.md)
- [Finite-well confinement in a semiconductor heterostructure](finite-well-confinement-in-a-semiconductor-heterostructure.md)
- [Gauge-invariant Josephson phase](gauge-invariant-josephson-phase.md)
- [Hamiltonian (quantum mechanics)](hamiltonian-quantum-mechanics.md)
- [Harmonic-oscillator wavefunction inflections](harmonic-oscillator-wavefunction-inflections.md)
- [History of physics](history-of-physics.md)
- [Infinite square well](infinite-square-well.md)
- [Jost solution](jost-solution.md)
- [Light-cone Hamiltonian](light-cone-hamiltonian.md)
- [Local relation](local-relation.md)
- [Many-worlds interpretation](many-worlds-interpretation.md)
- [Matrix and wave mechanics equivalence](matrix-and-wave-mechanics-equivalence.md)
- [Nobel Prize in Physics in 1933](nobel-prize-in-physics-in-1933.md)
- [Nondegeneracy of one-dimensional bound states](nondegeneracy-of-one-dimensional-bound-states.md)
- [Nonrelativistic quantum mechanics](nonrelativistic-quantum-mechanics.md)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2012/paper-1/3/solution.md)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2012/paper-1/4/solution.md)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2016/paper-1/2/a/solution.md)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2017/1/c/solution.md)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2018/section-b/b2/solution.md)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2019/section-b/6/solution.md)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2021/section-b/4/a/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-2b/section-b/33/c/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-2/9f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-1/18d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-1/9d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-1/9a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-2/9a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-3/20a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-2/8d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-1/15g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-3/16g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-3/7g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-4/32d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-4/6b/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-60/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-1/15b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-1/32d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-60/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-3/16a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-4/6a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-61/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-61/3/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-1/15b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-2/16b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-3/7b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-52/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-3/30e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-3/30e/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-3/34b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-4/32c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-3/34e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ib/paper-2/17b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ib/paper-2/17b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-46/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-62/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4/30a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-3/16b/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-3/8b/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-2/17b/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-3/8b/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4/6b/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-3/8b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-1/34a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-341/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-3/16b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-4/6b/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ib/paper-2/14a/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3/34c/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-2/15c/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-341/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-2/15b/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-4/4b/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-325/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-341/section-a/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-1/14d/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-2/15d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-3/6d/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-4/4d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-2/15a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-2/15a/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-4/15a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-4/4a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-3/34e/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-4/34e/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-325/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-325/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-341/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-341/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-1/35b/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-325/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ib/paper-4/4b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-325/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-1/6/ii/solution.md)
- [Solution](past-exam-of-the-mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge/2019/paper-2/section-a-ii/15/i/solution.md)
- [Solution](past-exam-of-the-mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge/2022/paper-2/section-b/21/i/solution.md)
- [Solution](past-exam-of-the-mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge/2022/paper-2/section-b/21/ii/b/solution.md)
- [Solution](past-exam-of-the-mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge/2023/paper-2/section-b/21/iii/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2010/paper-2/section-a/2/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2010/paper-2/section-c/c11/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2011/paper-2/section-b/b8/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2011/paper-2/section-c/c10/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2011/paper-2/section-c/c11/b/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2012/paper-1/section-a/2/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2012/paper-1/section-c/c11/a/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2014/paper-1/section-b/b7/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2015/paper-1/section-c/c11/b/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2015/paper-1/section-c/c11/c/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-1/section-c/c11/b/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-1/section-b/b6/a/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-1/section-b/b6/b/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-1/section-b/b7/a/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-1/section-b/b7/b/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-1/section-b/b9/c/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-1/section-c/c10/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-1/section-c/c11/c/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-1/section-a/3/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-1/section-b/b7/a/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-1/section-b/b8/a/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-1/section-b/b8/d/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-1/section-c/c10/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-2/section-c/c11/c/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2021/paper-2/section-c/c8/a/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2022/paper-1/section-d/d9/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-1/section-d/d13/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-1/section-d/d13/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/section-d/12/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/section-d/13/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/section-b/9/b/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/section-b/9/c/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1/section-b/b8/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1/section-a/a2/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1/section-b/b1/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2006/section-b/b6/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2012/3/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2019/section-b/4/b/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2022/section-b/5/a/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-field-theory-course-of-the-university-of-cambridge/2013/paper-1/2/b/solution.md)
- [Solution](past-exam-of-the-quantum-information-course-of-the-university-of-cambridge/2014/paper-1/3/c/solution.md)
- [Solution](past-exam-of-the-theoretical-physics-ii-course-of-the-university-of-cambridge/2012/paper-1/6/b/solution.md)
- [Solution](past-exam-of-the-theoretical-physics-ii-course-of-the-university-of-cambridge/2014/paper-1/1/b/solution.md)
- [Solution](past-exam-of-the-theoretical-physics-ii-course-of-the-university-of-cambridge/2015/paper-1/3/a/solution.md)
- [Solution](past-exam-of-the-theoretical-physics-ii-course-of-the-university-of-cambridge/2017/3/b/solution.md)
- [Solution](past-exam-of-the-theoretical-physics-ii-course-of-the-university-of-cambridge/2017/4/a/solution.md)
- [Solution](past-exam-of-the-theoretical-physics-ii-course-of-the-university-of-cambridge/2019/1/c/solution.md)
- [Pauli equation](pauli-equation.md)
- [Postulates of quantum mechanics](postulates-of-quantum-mechanics.md)
- [Probability continuity equation](probability-continuity-equation.md)
- [Quantum bouncer](quantum-bouncer.md)
- [Quantum mechanics](quantum-mechanics-split.md)
- [Quantum optimal control](quantum-optimal-control.md)
- [Quantum state continuity at a finite Hamiltonian step](quantum-state-continuity-at-a-finite-hamiltonian-step.md)
- [Quantum variational principle](quantum-variational-principle.md)
- [Radial Schrödinger equation for a central potential](radial-schrodinger-equation-for-a-central-potential.md)
- [Relativistic matter-wave velocities](relativistic-matter-wave-velocities.md)
- [Schrödinger equation](schrodinger-equation.md)
- [Time-independent Schrödinger equation](time-independent-schrodinger-equation.md)
- [Unitary time evolution](unitary-time-evolution.md)
- [Variational costate gradient for Hamiltonian quantum control](variational-costate-gradient-for-hamiltonian-quantum-control.md)
- [Variational method](variational-method.md)
- [Wavefunction node](wavefunction-node.md)
- [Work in a two-level sudden quench](work-in-a-two-level-sudden-quench.md)
