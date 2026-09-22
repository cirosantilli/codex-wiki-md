# Energy eigenvalue

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)

An energy eigenvalue is an [eigenvalue](linear-operator-theory.md#eigenvalue) of the [Hamiltonian operator](quantum-system.md#hamiltonian-quantum-mechanics) $H$: there is a nonzero [vector](vector-space.md#vector) $\psi$ in its [operator domain](vector-space.md#operator-domain) $D(H)$ with

$$
H\psi=E\psi.
$$

For a [self-adjoint operator](linear-operator-theory.md#self-adjoint-operator), $E$ is real. Normalizing $\psi$ produces an [energy eigenstate](#energy-eigenstate); an ideal [energy measurement](wave-function.md#energy-measurement) then returns $E$ with probability one. The associated [energy eigenspace](#energy-eigenspace) includes all vectors with this same [energy eigenvalue](energy-eigenvalue.md), including the zero vector, which represents no [quantum state](quantum-system.md#quantum-state). Different [energy eigenvalues](energy-eigenvalue.md) have orthogonal [energy eigenspaces](#energy-eigenspace). [Teschl, Mathematical Methods in Quantum Mechanics, Lemma 2.20](https://www.mat.univie.ac.at/~gerald/ftp/book-schroe/schroe.pdf).

The [energy eigenvalues](energy-eigenvalue.md) form the [point spectrum](linear-operator-theory.md#point-spectrum), which can be only part of the [spectrum](linear-operator-theory.md#spectrum-functional-analysis). The term [discrete spectrum](functional-analysis.md#discrete-spectrum) more specifically means isolated [eigenvalues](linear-operator-theory.md#eigenvalue) of finite multiplicity. The usual fixed-nucleus [hydrogen atom](mathematical-physics.md#hydrogen-atom) model has discrete negative [bound state](quantum-system.md#bound-state) [energy eigenvalues](energy-eigenvalue.md) together with a continuum at nonnegative [energy](energy.md). [Teschl, Mathematical Methods in Quantum Mechanics, sections 6.4 and 10.2](https://www.mat.univie.ac.at/~gerald/ftp/book-schroe/schroe.pdf). A [quantum system](quantum-system.md) need not have a ladder of discrete [energy eigenvalues](energy-eigenvalue.md): a whole-line [free particle](quantum-mechanics.md#free-particle) has [continuous spectrum](linear-operator-theory.md#continuous-spectrum). A [plane wave](wave-function.md#plane-wave) used for a [free particle](quantum-mechanics.md#free-particle) is a generalized [eigenfunction](linear-operator-theory.md#eigenfunction) of the [Hamiltonian operator](quantum-system.md#hamiltonian-quantum-mechanics), rather than a normalized vector in the physical [Hilbert space](hilbert-space.md). [Barton Zwiebach, MIT 8.05 Wave Mechanics, sections 2 and 4](https://live.ocw.mit.edu/courses/8-05-quantum-physics-ii-fall-2013/61bc31b8d8bf0680c322733910a71aa0_MIT8_05F13_Chap_01.pdf).

For the [infinite square well](quantum-mechanics.md#infinite-square-well) $0<x<L$, the [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition) give

$$
\phi_n(x)=\sqrt{\frac2L}\sin\frac{n\pi x}{L},\qquad E_n=\frac{\hbar^2\pi^2 n^2}{2mL^2},\qquad n=1,2,\ldots.
$$

Substitution into $H\phi_n=E_n\phi_n$ and [wavefunction normalization](wave-function.md#wavefunction-normalization) verify these statements directly. Here $E_1$ is the [ground-state energy](quantum-mechanics.md#ground-state-energy), even though its index is one; the labeling convention does not determine which [quantum state](quantum-system.md#quantum-state) is lowest. Equal populations of $\phi_1$ and $\phi_2$ have [energy](energy.md) [expectation value](quantum-system.md#expectation-value) $(E_1+E_2)/2=5E_1/2$, but an [energy measurement](wave-function.md#energy-measurement) returns $E_1$ or $4E_1$, each with probability $1/2$. An average of allowed [energy eigenvalues](energy-eigenvalue.md) need not itself be an [energy eigenvalue](energy-eigenvalue.md).

**Table of contents**

- [Energy eigenstate](#energy-eigenstate)
  - [Energy eigenfunction](#energy-eigenfunction)
  - [Energy eigenvector](#energy-eigenvector)
- [Energy eigenspace](#energy-eigenspace)
- [Excited state](#excited-state)
  - [Intersystem crossing](#intersystem-crossing)
  - [Franck-Hertz experiment](#franck-hertz-experiment)
    - [Franck-Hertz energy-loss model](#franck-hertz-energy-loss-model)
      - [Franck-Hertz retarding collector transfer](#franck-hertz-retarding-collector-transfer)
      - [Franck-Hertz repeated-loss collection model](#franck-hertz-repeated-loss-collection-model)
      - [Franck-Hertz spacing fit and contact offset](#franck-hertz-spacing-fit-and-contact-offset)
  - [First excited state](#first-excited-state)
- [Eigenstate](#eigenstate)
  - [Momentum eigenstate](#momentum-eigenstate)

## Energy eigenstate

↑ **Parent:** [Energy eigenvalue](energy-eigenvalue.md)

An [energy eigenstate](#energy-eigenstate) is a [quantum state](quantum-system.md#quantum-state) represented by an [eigenvector](linear-operator-theory.md#eigenvector) of the [Quantum Hamiltonian](quantum-system.md#hamiltonian-quantum-mechanics). For a time-independent [Quantum Hamiltonian](quantum-system.md#hamiltonian-quantum-mechanics), a normalized [eigenfunction](linear-operator-theory.md#eigenfunction) $\phi$ with [energy eigenvalue](energy-eigenvalue.md) $E$ evolves according to the [Schrödinger equation](mathematical-physics.md#schrodinger-equation) as

$$
\psi(x,t)=\phi(x)e^{-iEt/\hbar},\qquad |\psi(x,t)|^2=|\phi(x)|^2.
$$

Here $\hbar=h/(2\pi)$ is the reduced [Planck constant](quantum-mechanics.md#planck-constant). The changing factor is a [global phase](quantum-system.md#global-phase), so this is a [stationary state](quantum-system.md#stationary-state): its position [probability density](wave-function.md#probability-density) is constant. For example, the second [infinite square well](quantum-mechanics.md#infinite-square-well) mode has two density lobes separated by a [node of a standing wave](wave-equation.md#node-physics) at $x=L/2$; both lobes stay fixed while its [quantum phase](quantum-system.md#quantum-phase) rotates. An ideal [energy measurement](wave-function.md#energy-measurement) returns $E$ with probability one, but a [position measurement](quantum-measurement.md#position-measurement) still has a distribution. Stationary density does not describe a particle sitting at the peak of a lobe. Distinct [energy eigenvalues](energy-eigenvalue.md) accumulate different [quantum phases](quantum-system.md#quantum-phase), making their [quantum superposition](quantum-system.md#quantum-superposition) behave differently.

### Energy eigenfunction

↑ **Parent:** [Energy eigenstate](#energy-eigenstate)

A nonzero position-space [wavefunction](wave-function.md) representing an [energy eigenstate](#energy-eigenstate). For a time-independent [Quantum Hamiltonian](quantum-system.md#hamiltonian-quantum-mechanics), its time evolution is a [global phase](quantum-system.md#global-phase), so its position [probability density](wave-function.md#probability-density) is stationary.

### Energy eigenvector

↑ **Parent:** [Energy eigenstate](#energy-eigenstate)

A nonzero [eigenvector](linear-operator-theory.md#eigenvector) of the [Quantum Hamiltonian](quantum-system.md#hamiltonian-quantum-mechanics).

## Energy eigenspace

↑ **Parent:** [Energy eigenvalue](energy-eigenvalue.md)

The energy eigenspace at $E$ is the [vector subspace](vector-space.md#vector-subspace)

$$
\mathcal E_E=\ker(H-EI)=\{\psi\in D(H):H\psi=E\psi\},
$$

where $H$ is the [Hamiltonian operator](quantum-system.md#hamiltonian-quantum-mechanics) and $I$ is the [identity operator](vector-space.md#identity-operator). It is nonzero exactly when $E$ is an [energy eigenvalue](energy-eigenvalue.md). Its [dimension](vector-space.md#dimension-vector-space) is the multiplicity of that [energy eigenvalue](energy-eigenvalue.md); [degenerate energy levels](quantum-mechanics.md#degenerate-energy-levels) have multiplicity greater than one. The [ground-state subspace](quantum-mechanics.md#ground-state-subspace) is $\mathcal E_{E_0}$, and its [dimension](vector-space.md#dimension-vector-space) is the [ground-state degeneracy](quantum-mechanics.md#ground-state-degeneracy). A vector in an [energy eigenspace](#energy-eigenspace) need not be one of a specially chosen [orthonormal basis](inner-product.md#orthonormal-basis) of [energy eigenstates](#energy-eigenstate).

[Linearity](vector-space.md#linearity) makes the useful point immediate: if $H\phi_1=E\phi_1$ and $H\phi_2=E\phi_2$, then $H(a\phi_1+b\phi_2)=E(a\phi_1+b\phi_2)$. Every normalized nonzero combination stays in the same [energy eigenspace](#energy-eigenspace). For a time-independent [Hamiltonian operator](quantum-system.md#hamiltonian-quantum-mechanics), its evolution is multiplication by the common [global phase](quantum-system.md#global-phase) $e^{-iEt/\hbar}$, so it is a [stationary state](quantum-system.md#stationary-state). A [quantum superposition](quantum-system.md#quantum-superposition) within a degenerate [energy eigenspace](#energy-eigenspace) can change spatial shape when its coefficients are chosen differently, but its density does not subsequently beat under this unchanged [Hamiltonian operator](quantum-system.md#hamiltonian-quantum-mechanics).

Across distinct [energy eigenspaces](#energy-eigenspace), relative [quantum phases](quantum-system.md#quantum-phase) evolve. For orthonormal [eigenfunctions](linear-operator-theory.md#eigenfunction) $\phi_1,\phi_2$ of the [Hamiltonian operator](quantum-system.md#hamiltonian-quantum-mechanics) with [energy eigenvalues](energy-eigenvalue.md) $E_1\ne E_2$, an equal-weight [quantum superposition](quantum-system.md#quantum-superposition) has

$$
\psi(x,t)=\frac{e^{-iE_1t/\hbar}\phi_1(x)+e^{-iE_2t/\hbar}\phi_2(x)}{\sqrt2},
$$

and position [probability density](wave-function.md#probability-density)

$$
|\psi(x,t)|^2=\frac{|\phi_1(x)|^2+|\phi_2(x)|^2}{2}+\operatorname{Re}\!\left[\phi_1(x)^*\phi_2(x)e^{-i(E_2-E_1)t/\hbar}\right].
$$

The interference term can change local probabilities even though the [Born rule](wave-function.md#born-rule) assigns the same time-independent probability $1/2$ to each [energy measurement](wave-function.md#energy-measurement) outcome. [Orthogonality](inner-product.md#orthogonal-vectors) makes its integral zero, preserving [wavefunction normalization](wave-function.md#wavefunction-normalization). This [pure state](quantum-theory.md#pure-state) is not a [stationary state](quantum-system.md#stationary-state); some particular measurement distributions may nevertheless remain constant. An incoherent [mixed state](density-matrix.md#mixed-state) with the same energy populations has no such interference term.

<a id="image-an-excited-energy-eigenstate-can-be-stationary-while-a-two-energy-superposition-beats"></a>
![](ground-excited-states-stationary-density.png)

**[Figure 1](#image-an-excited-energy-eigenstate-can-be-stationary-while-a-two-energy-superposition-beats). An excited energy eigenstate can be stationary while a two-energy superposition beats**. Exact [infinite square well](quantum-mechanics.md#infinite-square-well) densities, not measured data, with $u=x/L$ and $\theta=(E_2-E_1)t/\hbar$. The left panel shows the unchanged density of the second [energy eigenstate](#energy-eigenstate) at three times. The right panel shows a coherent equal-weight [quantum superposition](quantum-system.md#quantum-superposition) at $\theta=0,\pi/2,\pi$; its energy populations remain $1/2,1/2$. The dashed curve is the density of the corresponding incoherent [mixed state](density-matrix.md#mixed-state).

For the pictured [infinite square well](quantum-mechanics.md#infinite-square-well), $\theta=3E_1t/\hbar$ and the interference repeats after $T=2\pi\hbar/(3E_1)$. At $t=0$, direct integration gives $\langle x\rangle=L/2-16L/(9\pi^2)$; halfway through the period it is $L/2+16L/(9\pi^2)$. This is a moving [expectation value](quantum-system.md#expectation-value), rather than a trajectory of an individual particle. The distinction between an [energy eigenspace](#energy-eigenspace) and a combination of different [energy eigenspaces](#energy-eigenspace) is what makes the different behavior possible.

## Excited state

↑ **Parent:** [Energy eigenvalue](energy-eigenvalue.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Excited_state)

In the stationary-state terminology used here, an excited state is a normalized [energy eigenstate](#energy-eigenstate) with [energy eigenvalue](energy-eigenvalue.md) $E>E_0$, where $E_0$ is an attained [ground-state energy](quantum-mechanics.md#ground-state-energy). Its excitation cost above the [ground state](quantum-mechanics.md#ground-state) is $\Delta E=E-E_0>0$. Several [energy eigenstates](#energy-eigenstate) can share one excited [energy eigenvalue](energy-eigenvalue.md) through [degenerate energy levels](quantum-mechanics.md#degenerate-energy-levels). An arbitrary [quantum superposition](quantum-system.md#quantum-superposition) with [energy](energy.md) [expectation value](quantum-system.md#expectation-value) above $E_0$ need not be a single stationary [excited state](#excited-state); its energy content is described by its [Born rule](wave-function.md#born-rule) probabilities or, for a continuum, its [scalar spectral measure](hilbert-space.md#scalar-spectral-measure).

An [excited state](#excited-state) can be a [stationary state](quantum-system.md#stationary-state): the second [infinite square well](quantum-mechanics.md#infinite-square-well) mode is an immediate example. Spontaneous [photon emission](quantum-mechanics.md#photon-emission) is a transition caused by coupling matter to the [electromagnetic field](electromagnetism.md#electromagnetic-field); it is absent from an isolated matter-only [Hamiltonian operator](quantum-system.md#hamiltonian-quantum-mechanics). The relevant [energy eigenstate](#energy-eigenstate) of that isolated model is therefore not automatically an [energy eigenstate](#energy-eigenstate) of the full interacting system. This distinction explains how an ideal stationary [excited state](#excited-state) can approximate a state with a finite experimental lifetime. See [electric-dipole interaction](quantum-mechanics.md#electric-dipole-interaction) for the coupling used in the simplest optical model.

For a one-photon transition between stationary internal states, neglecting recoil, [conservation of energy](mathematical-physics.md#conservation-of-energy) requires

$$
h\nu=E_f-E_i\quad\text{for absorption},\qquad h\nu=E_i-E_f\quad\text{for emission}.
$$

Here $h$ is the [Planck constant](quantum-mechanics.md#planck-constant) and $\nu$ is the [photon](quantum-mechanics.md#photon) [frequency](wave.md#frequency). Energy matching alone does not guarantee a transition: in the [electric-dipole interaction](quantum-mechanics.md#electric-dipole-interaction) approximation its strength also involves the [matrix element](vector-space.md#matrix-element) $\langle f|\mathbf d\cdot\boldsymbol\epsilon|i\rangle$, where $\mathbf d$ is the [electric dipole moment](electrostatics.md#electric-dipole-moment) operator and $\boldsymbol\epsilon$ specifies [photon polarization](quantum-mechanics.md#photon-polarization). A zero [matrix element](vector-space.md#matrix-element) gives an [electric-dipole selection rule](quantum-mechanics.md#electric-dipole-selection-rule). Thus an absent optical line does not prove the corresponding [energy eigenvalue](energy-eigenvalue.md) is absent; a different interaction can couple different states. [Richard Fitzpatrick, Quantum Mechanics, Selection Rules](https://farside.ph.utexas.edu/teaching/qmech/lectures/node121.html). The [Franck-Hertz experiment](#franck-hertz-experiment) gives a particularly instructive comparison between collision excitation and [photon emission](quantum-mechanics.md#photon-emission).

The [first excited state](#first-excited-state) terminology assumes a least [energy eigenvalue](energy-eigenvalue.md) above $E_0$. Such a next level is not guaranteed by [quantum mechanics](quantum-mechanics.md): a [continuous spectrum](linear-operator-theory.md#continuous-spectrum) can start immediately above the spectral bottom, or [energy eigenvalues](energy-eigenvalue.md) can accumulate there. For example, a [Hamiltonian operator](quantum-system.md#hamiltonian-quantum-mechanics) with [energy eigenvalues](energy-eigenvalue.md) $0,\varepsilon,\varepsilon/2,\varepsilon/3,\ldots$, where $\varepsilon>0$, has a [ground-state energy](quantum-mechanics.md#ground-state-energy) zero but no least positive [energy eigenvalue](energy-eigenvalue.md): every candidate $\varepsilon/n$ is exceeded downward by $\varepsilon/(n+1)$. A [free particle](quantum-mechanics.md#free-particle) on the whole line has neither a [ground state](quantum-mechanics.md#ground-state) nor a first stationary [excited state](#excited-state). Each use of a discrete excitation ladder therefore needs a specified [Hamiltonian operator](quantum-system.md#hamiltonian-quantum-mechanics) and its [boundary conditions](differential-equation.md#boundary-condition).

### Intersystem crossing

↑ **Parent:** [Excited state](#excited-state)

A nonradiative transition between electronic states of different [spin multiplicity](angular-momentum-operator.md#spin-multiplicity), enabled by interactions such as spin–orbit coupling. A constant intersystem-crossing channel contributes to the unquenched excited-state lifetime.

### Franck-Hertz experiment

↑ **Parent:** [Excited state](#excited-state)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Franck–Hertz_experiment)

The Franck-Hertz experiment connects a reproducible loss of [electron](physics.md#electron) [kinetic energy](energy.md#kinetic-energy) with excitation of a [chemical atom](physics.md#atom-physics). The original mercury-vapor experiments were performed during 1912–1914 while investigating [ionization](atomic-physics.md#ionization); they were not designed as a test of the [Bohr model](mathematical-physics.md#bohr-model). Their later interpretation distinguished internal excitation from removal of an [electron](physics.md#electron). [KIT physics laboratory, H23 Franck-Hertz-Versuch, Motivation](https://labs.physik.kit.edu/prakt-klass-physik-manuals/P2/Franck_Hertz_Versuch/).

In a modern mercury tube, a heated [cathode](electrochemistry.md#cathode) emits [electrons](physics.md#electron) and a positive perforated grid accelerates them through Hg vapor. A collector slightly below the grid's [electric potential](electric-field.md#electric-potential) rejects slow [electrons](physics.md#electron). The oven controls vapor density and hence the [mean free path](ideal-gas.md#mean-free-path). Keep heating and retarding settings fixed, sweep the accelerating [electric potential difference](electric-field.md#electric-potential-difference) $V$, and record collector [electric current](electric-charge.md#electric-current) $I(V)$. These measured quantities indirectly probe atomic excitation. [Shah, Alam and Anwar, Electron energy loss investigated through the Franck-Hertz Experiment, sections 3–4](https://physlab.org/wp-content/uploads/2016/03/Franck_exp_v12015.pdf).

The curve shows repeated current minima, typically about $4.9\,\mathrm V$ apart. In the collision model, an [electron](physics.md#electron) gains approximately $eV$ of [kinetic energy](energy.md#kinetic-energy), with $e$ the positive [elementary charge](electric-charge.md#elementary-charge). An [inelastic collision](classical-mechanics.md#inelastic-collision) transfers about $4.9\,\mathrm{eV}$ to internal excitation. Near the grid, this can prevent the [electron](physics.md#electron) crossing the retarding region, lowering collected [electric current](electric-charge.md#electric-current). Further acceleration restores collection; repeated excitation losses produce further minima. These represent multiple collisions, rather than equally spaced atomic [energy eigenvalues](energy-eigenvalue.md). Contact potentials shift the first minimum, so compare several successive spacings instead of identifying the first dip's voltage with the excitation cost. [Shah, Alam and Anwar, sections 3.1–4 and Figure 3](https://physlab.org/wp-content/uploads/2016/03/Franck_exp_v12015.pdf).

The optical comparison supplies a second observable: mercury radiation at a [wavelength](wave-equation.md#wavelength) near $253.6\,\mathrm{nm}$ was detected through a window in the tube. Its inferred [photon](quantum-mechanics.md#photon) [energy](energy.md) $hc/\lambda\approx4.89\,\mathrm{eV}$ agrees with the characteristic collision loss, with $c$ the [speed of light](special-relativity.md#speed-of-light). This agreement supports the interpretation as a transition between internal atomic energies. It does not make the collector trace a complete spectrum. In particular, the lowest excited mercury level, labeled $6\,{}^3P_0$, is metastable because an [electric-dipole selection rule](quantum-mechanics.md#electric-dipole-selection-rule) forbids its direct transition to the [ground state](quantum-mechanics.md#ground-state); the nearby $6\,{}^3P_1$ level emits the quoted [ultraviolet](optics.md#ultraviolet) line. Collision excitation and optical detection therefore have different sensitivities to the available [excited states](#excited-state). [MIT Junior Lab, The Franck-Hertz Experiment, section VI and the discussion following Figure 6](https://ocw.mit.edu/courses/8-13-14-experimental-physics-i-ii-junior-lab-fall-2016-spring-2017/afdfff9f8bbe067239af19c8b178a764_MIT8_13-14F16-S17exp7.pdf).

Initial [electron](physics.md#electron) [kinetic energy](energy.md#kinetic-energy) spread and varying collision positions broaden real minima. Repeat traces at different retarding settings and oven temperatures to distinguish excitation from collection effects. This probes a discrete energy-transfer channel, rather than every [energy eigenspace](#energy-eigenspace), its [dimension](vector-space.md#dimension-vector-space), or an absolute [ground-state energy](quantum-mechanics.md#ground-state-energy). [MIT Junior Lab, sections IV and VI](https://ocw.mit.edu/courses/8-13-14-experimental-physics-i-ii-junior-lab-fall-2016-spring-2017/afdfff9f8bbe067239af19c8b178a764_MIT8_13-14F16-S17exp7.pdf).

[James Franck](physicist.md#james-franck) and [Gustav Ludwig Hertz](physicist.md#gustav-ludwig-hertz) presented their paper on 24 April 1914. Its heated [platinum](chemical-substance.md#platinum) wire sat inside a cylindrical [platinum](chemical-substance.md#platinum) mesh, with a collector 1–2 mm beyond it. A heated bath and pumping prepared the vapor; guard rings suppressed leakage. They differentiated retarding-[electric current](electric-charge.md#electric-current) scans to study outgoing [energies](energy.md).[1914, pp. 457, 459–461, Figs. 1–2](physics-bibliography.md#uber-zusammenstosse-zwischen-elektronen-und-den-molekulen-des-quecksilberdampfes-und-die-ionisierungsspannung-desselben-by-james-franck-and-gustav-ludwig-hertz)

Their 1925 Nobel Prize preceded their lectures of 11 December 1926. [James Franck](physicist.md#james-franck) described choosing [pressure](pressure.md) for many [collisions](classical-mechanics.md#collision) before the mesh but few afterward.[Nobel Lectures, Physics 1922–1941; pp. 98, 100–101](physics-bibliography.md#nobel-lectures-physics-1922-1941/transformations-of-kinetic-energy-of-free-electrons-into-excitation-energy-of-atoms-by-impacts-by-james-franck) [Gustav Ludwig Hertz](physicist.md#gustav-ludwig-hertz) explained how a field-free collision region narrowed excitation thresholds.[Nobel Lectures, Physics 1922–1941; pp. 112, 119–120](physics-bibliography.md#nobel-lectures-physics-1922-1941/the-results-of-the-electron-impact-tests-in-the-light-of-bohr’s-theory-of-atoms-by-gustav-ludwig-hertz)

#### Franck-Hertz energy-loss model

↑ **Parent:** [Franck-Hertz experiment](#franck-hertz-experiment)

A useful [Franck-Hertz energy-loss model](#franck-hertz-energy-loss-model) separates three operations: accelerating an [electron](physics.md#electron), losing a discrete [energy](energy.md) $\Delta$ in an [inelastic collision](classical-mechanics.md#inelastic-collision), and selecting the surviving [electrons](physics.md#electron) with a retarding collector. The collector measures an accepted fraction of an outgoing [energy](energy.md) distribution. This makes the experiment a small [inverse problem](inverse-problem.md): the [electric current](electric-charge.md#electric-current) depends on both the collision physics and the readout.

For a deliberately simple one-channel model, let $u\geq0$ be the incoming [kinetic energy](energy.md#kinetic-energy), and let $p(u)$ be the [probability](probability-theory.md#probability) that one encounter excites the [chemical atom](physics.md#atom-physics). Set $p(u)=0$ for $u<\Delta$ and $0\leq p(u)\leq1$ otherwise. The conditional [probability distribution](probability-distribution.md) of outgoing [kinetic energy](energy.md#kinetic-energy) $E$ is the discrete loss kernel

$$
K(E\mid u)=[1-p(u)]\delta(E-u)+p(u)\delta(E-u+\Delta).
$$

Here $\delta$ is the [Dirac delta function](distribution-theory.md#dirac-delta-function). The kernel has unit [integral](integral.md), no negative outgoing [energy](energy.md), and mean outgoing [kinetic energy](energy.md#kinetic-energy) $u-p(u)\Delta$. It neglects the small recoil loss in an [elastic collision](classical-mechanics.md#elastic-collision), other excitation channels and [ionization](atomic-physics.md#ionization). The threshold permits excitation; it does not require $p(u)=1$ above threshold. In particular, choosing a single $\Delta=4.9\,\mathrm{eV}$ here isolates the characteristic channel discussed above without claiming it is mercury's lowest possible excitation.

##### Franck-Hertz retarding collector transfer

↑ **Parent:** [Franck-Hertz energy-loss model](#franck-hertz-energy-loss-model)

For [electrons](physics.md#electron) directed normally toward an ideal planar collector, a retarding [electric potential difference](electric-field.md#electric-potential-difference) $V_r>0$ imposes the barrier $eV_r$. Write its transfer as $T(E)=H(E-eV_r)$, where $H$ is the [Heaviside step function](integral-transform.md#heaviside-step-function) and $e$ the positive [elementary charge](electric-charge.md#elementary-charge). Thus a perfectly sharp loss need not produce a sharp drop in [electric current](electric-charge.md#electric-current): the drop also depends on where the outgoing [energy](energy.md) lies relative to the barrier. For an oblique incident [electron](physics.md#electron) at angle $\theta$ to the normal, the same planar model instead tests $E\cos^2\theta>eV_r$; angular scattering can change collection even at unchanged total [kinetic energy](energy.md#kinetic-energy).

<a id="image-franck-hertz-energy-loss-model-separate-acceleration-loss-and-collection"></a>
![](franck-hertz-collector-threshold.png)

**[Figure 2](#image-franck-hertz-energy-loss-model-separate-acceleration-loss-and-collection). Franck-Hertz energy-loss model: separate acceleration, loss and collection**. [Source](franck-hertz-collector-threshold.py). Original functional schematic, not a scale reconstruction of a historical tube. The lower panel applies an ideal normally incident retarder to the explicitly chosen one-collision example. Equal vertical strokes mark outgoing [energies](energy.md); their labeled weights give [probabilities](probability-theory.md#probability).

For example, choose a monoenergetic incoming beam with $u=5.6\,\mathrm{eV}$, $p=0.75$ and $\Delta=4.9\,\mathrm{eV}$. After one encounter, $25\%$ have $5.6\,\mathrm{eV}$ and $75\%$ have $0.7\,\mathrm{eV}$. A $1.0\,\mathrm V$ retarder collects only $0.25I_0$, whereas a $0.5\,\mathrm V$ retarder collects $I_0$; here $I_0$ is the incident [electric current](electric-charge.md#electric-current) with fixed geometrical acceptance and no background. The mean outgoing [kinetic energy](energy.md#kinetic-energy) is $1.925\,\mathrm{eV}$, independently checked by $5.6-0.75(4.9)$. These are chosen inputs and calculated fractions, not historical measurements.

More generally, let $f(E;V)$ be the normalized outgoing [probability density function](continuous-probability-distribution.md#probability-density-function) at a fixed accelerating [electric potential difference](electric-field.md#electric-potential-difference) $V$, for the normally incident idealization. A retarding scan gives

$$
\frac{I(V,V_r)}{I_0}=\int_{eV_r}^{\infty}f(E;V)\,dE,\qquad
f(eV_r;V)=-\frac{1}{eI_0}\frac{\partial I}{\partial V_r}.
$$

The second equation follows by differentiating the lower integration limit, with [Dirac delta functions](distribution-theory.md#dirac-delta-function) understood for sharp beams. It explains why an integrated collector readout can reveal an [energy](energy.md) distribution. With angles present it probes the distribution of normal [kinetic energy](energy.md#kinetic-energy); finite instrumental resolution smooths it, and numerical [differentiation](calculus.md#differentiation) amplifies noise. Keep the incoming beam fixed during this scan. A scan of $V$ changes $f$ itself and cannot be differentiated by the same inversion formula.

##### Franck-Hertz repeated-loss collection model

↑ **Parent:** [Franck-Hertz energy-loss model](#franck-hertz-energy-loss-model)

Define a signed offset $V_c$ so that the accelerating region adds [kinetic energy](energy.md#kinetic-energy) $e(V-V_c)$. This convention concerns this gap; collector contact fields belong in the effective $V_r$. An [electron](physics.md#electron) emitted with initial [kinetic energy](energy.md#kinetic-energy) $E_0$ and undergoing $n$ identical excitation losses reaches the grid with

$$
E_n=E_0+e(V-V_c)-n\Delta.
$$

Each loss excites a fresh [chemical atom](physics.md#atom-physics) initially in its [ground state](quantum-mechanics.md#ground-state). These are repeated payments of the same excitation cost. The index $n$ counts events along an [electron](physics.md#electron) trajectory, not the ordinal number of an atomic [excited state](#excited-state). The outgoing [energy](energy.md) also does not locate the last collision: after an early collision an [electron](physics.md#electron) can regain enough [kinetic energy](energy.md#kinetic-energy) to cross the barrier.

At fixed $V$, let $g(E_0)$ be the normalized initial-[energy](energy.md) [probability density function](continuous-probability-distribution.md#probability-density-function) within the ensemble of [electrons](physics.md#electron) reaching the grid, and $w_n(E_0,V)$ the [conditional probabilities](probability-theory.md#conditional-probability) for $n$ losses within that ensemble. Then the ideal collection law is

$$
\frac{I(V,V_r)}{I_0}=\int_0^\infty g(E_0)\sum_{n=0}^\infty w_n(E_0,V)H\bigl(E_0+e(V-V_c)-n\Delta-eV_r\bigr)\,dE_0.
$$

Take $\sum_n w_n=1$ and exclude paths with insufficient [kinetic energy](energy.md#kinetic-energy) for a loss at its actual collision position. The weights contain collision positions and rates, [mean free paths](ideal-gas.md#mean-free-path) and angular acceptance. This equation is a bookkeeping model, not a derivation of those weights. Multiplying all incident particles by one constant transmission is an additional approximation; real transmission and $I_0$ can vary with $V$.

One analytical extreme assumes $E_0=0$, one-dimensional motion and an immediate loss whenever the [kinetic energy](energy.md#kinetic-energy) reaches $\Delta$. With $d=\Delta/e$, $x=V-V_c\geq0$ and $0<V_r<d$, the number of losses and remaining [kinetic energy](energy.md#kinetic-energy) are

$$
n=\left\lfloor\frac{x}{d}\right\rfloor,\qquad \frac{E_n}{e}=r=x-d\left\lfloor\frac{x}{d}\right\rfloor,\qquad \frac{I}{I_0}=H(r-V_r).
$$

Here $\lfloor\cdot\rfloor$ is the [floor function](calculus.md#floor-function). Collection switches off for an interval of width $V_r$ after each reset, then recovers; the pattern repeats every $d$. For $d=4.9\,\mathrm V$, $V_c=1.2\,\mathrm V$ and $V_r=1.0\,\mathrm V$, an applied $V=11.4\,\mathrm V$ gives $n=2$, $r=0.4\,\mathrm V$ and rejection, whereas $V=12.2\,\mathrm V$ gives $n=2$, $r=1.2\,\mathrm V$ and collection. With $V_r=0$ the dips disappear in this idealization. With no collisions, there is only a single collection onset. Both limits expose the separate roles of loss and filtering.

To draw a smooth illustrative curve, extend this periodic rule mathematically to all $x$ and convolve it with a chosen [normal distribution](probability-distribution.md#normal-distribution) of voltage jitter, of [standard deviation](variance.md#standard-deviation) $\sigma$:

$$
C_\sigma(x)=\sum_{k\in\mathbb Z}\left[\Phi\!\left(\frac{x-kd-V_r}{\sigma}\right)-\Phi\!\left(\frac{x-(k+1)d}{\sigma}\right)\right].
$$

Here $\Phi$ is the [standard normal cumulative distribution function](probability-distribution.md#standard-normal-distribution-function). Each summand is the smoothed indicator of the accepted interval $kd+V_r<x<(k+1)d$. The result satisfies $0\leq C_\sigma\leq1$ and has period $d$. For the figure choose $\sigma=0.18\,\mathrm V$ and plot only well beyond the startup region. This is a chosen phenomenological curve, not a [Boltzmann equation](boltzmann-equation.md) transport prediction or a fit to measured [electric current](electric-charge.md#electric-current). Its symmetric troughs center on $V_c+nd+V_r/2$, rather than the reset voltages $V_c+nd$. Finite excitation rates, several loss channels, [space charge](electric-charge.md#space-charge), initial angular and [energy](energy.md) spreads, and real electrode geometry can change the trough shape and phase; a single convolution does not solve these effects.

<a id="image-illustrative-repeated-loss-collection-and-an-independent-synthetic-spacing-fit"></a>
![](franck-hertz-repeated-loss-spacing-fit.png)

**[Figure 3](#image-illustrative-repeated-loss-collection-and-an-independent-synthetic-spacing-fit). Illustrative repeated-loss collection and an independent synthetic spacing fit**. [Source](franck-hertz-repeated-loss-spacing-fit.py). Left: the chosen Gaussian-smoothed threshold model, with $d=4.9\,\mathrm V$, $V_c=1.2\,\mathrm V$, $V_r=1.0\,\mathrm V$ and $\sigma=0.18\,\mathrm V$. Right: separately chosen synthetic trough positions, their [ordinary least squares](normal-linear-model.md#ordinary-least-squares) fit and residuals. The points are not extracted from the left curve or a historical trace.

##### Franck-Hertz spacing fit and contact offset

↑ **Parent:** [Franck-Hertz energy-loss model](#franck-hertz-energy-loss-model)

Fit the positions of successive, consistently defined troughs by [linear regression](linear-regression.md), $V_n=b+nd+\epsilon_n$. A constant intercept $b$ absorbs the [contact potential difference](quantum-mechanics.md#contact-potential-difference), collection phase and initial [energy](energy.md) effects; $d$ estimates the repeated loss expressed as a voltage. Subtracting successive positions cancels $b$. A line fit uses every position and leaves residuals that can reveal curvature or a misidentified trough. It still assumes that the phase is constant over the fitted range and that all troughs belong to the same loss channel.

For an original numerical example, choose $n=1,2,3,4,5$ and synthetic positions $V_n=(6.62,11.46,16.48,21.30,26.14)\,\mathrm V$. Their successive spacings are $(4.84,5.02,4.82,4.84)\,\mathrm V$. The [ordinary least squares](normal-linear-model.md#ordinary-least-squares) formulas give

$$
\widehat d=\frac{\sum_n(n-\bar n)(V_n-\bar V)}{\sum_n(n-\bar n)^2}=4.888\,\mathrm V,\qquad
\widehat b=\bar V-\widehat d\,\bar n=1.736\,\mathrm V.
$$

The fitted residuals are $(-0.004,-0.052,0.080,0.012,-0.036)\,\mathrm V$, with zero sum and zero index-weighted sum. Their [residual sum of squares](linear-regression.md#residual-sum-of-squares) is $0.01056\,\mathrm V^2$. If independent, equal-[variance](variance.md), zero-mean errors describe these positions, the residual variance estimate is $s^2=0.01056/(5-2)=0.00352\,\mathrm V^2$ and the slope [standard error](statistical-inference.md#standard-error) is $s/\sqrt{10}=0.01876\,\mathrm V$. Thus the inferred model loss is $4.888\,\mathrm{eV}$ with conditional [standard error](statistical-inference.md#standard-error) $0.01876\,\mathrm{eV}$. These errors summarize only the chosen position scatter; a voltage-scale error or a drifting collection phase is not included. Adjacent spacings share a position error and are therefore correlated even when position errors are independent.

The offset has a sharper [identifiability](statistical-model.md#identifiability) limitation. Even if a constant-phase model were exact, an initial beam [kinetic energy](energy.md#kinetic-energy) $E_0$ shifts the troughs by $-E_0/e$. For the symmetric illustrative curve, $b=V_c-E_0/e+V_r/2$. The transformation $V_c\mapsto V_c+\alpha$, $E_0\mapsto E_0+e\alpha$ leaves every trough position unchanged. Measuring $b$ alone therefore cannot determine the [contact potential difference](quantum-mechanics.md#contact-potential-difference). Relabeling $n\mapsto n+m$ also changes $b$ by $-md$ without changing $d$. An independent offset calibration and a justified collection model are needed before turning a first trough into an excitation threshold. Varying $V_r$ tests this model's predicted half-voltage shift of the trough centers; it is a diagnostic prediction of this chosen curve, not a universal correction for experimental minima.

### First excited state

↑ **Parent:** [Excited state](#excited-state)

The first excited state has the smallest energy strictly above the ground-state energy.

## Eigenstate

↑ **Parent:** [Energy eigenvalue](energy-eigenvalue.md)

An eigenstate of an observable is a [quantum state](quantum-system.md#quantum-state) represented by an [eigenvector](linear-operator-theory.md#eigenvector) of that observable.

### Momentum eigenstate

↑ **Parent:** [Eigenstate](#eigenstate)

A momentum eigenstate is an eigenstate of the [momentum operator](quantum-mechanics.md#momentum-operator). In one dimension it is a [plane wave](wave-function.md#plane-wave) $e^{ikx}$ with momentum eigenvalue $\hbar k$.

## ↑ Ancestors (4)

1. [Quantum mechanics](quantum-mechanics.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (101)

- [Basis permutation of a quantum Hamiltonian matrix](quantum-system.md#basis-permutation-of-a-quantum-hamiltonian-matrix)
- [Berry-phase interference with a reference path](quantum-mechanics.md#berry-phase-interference-with-a-reference-path)
- [Berry phase of a Bloch-sphere latitude](quantum-mechanics.md#berry-phase-of-a-bloch-sphere-latitude)
- [Centrifugal distortion](molecule.md#centrifugal-distortion)
- [Chern insulator](topological-quantum-matter.md#chern-insulator)
- [Dynamical phase](quantum-system.md#dynamical-phase)
- [Einstein solid](heat.md#einstein-solid)
- [Energy eigenspace](#energy-eigenspace)
- [Energy eigenstate](#energy-eigenstate)
- [Energy eigenvalue](energy-eigenvalue.md)
- [Energy populations and evolving relative phases](quantum-system.md#energy-populations-and-evolving-relative-phases)
- [Erwin Schrödinger](physicist.md#erwin-schrodinger)
- [Excited state](#excited-state)
- [Exciton binding energy](quantum-mechanics.md#exciton-binding-energy)
- [Exciton optical transition](quantum-mechanics.md#exciton-optical-transition)
- [Finite-system analyticity](statistical-physics.md#finite-system-analyticity)
- [Franck-Hertz experiment](#franck-hertz-experiment)
- [Ground state](quantum-mechanics.md#ground-state)
- [Ground-state degeneracy](quantum-mechanics.md#ground-state-degeneracy)
- [Ground-state energy](quantum-mechanics.md#ground-state-energy)
- [Haldane model](topological-quantum-matter.md#haldane-model)
- [Half-line square-root potential well](energy.md#half-line-square-root-potential-well)
- [Harmonic vibrational energy levels](molecule.md#harmonic-vibrational-energy-levels)
- [Hyperfine structure](quantum-mechanics.md#hyperfine-structure)
- [Infinite square well](quantum-mechanics.md#infinite-square-well)
- [Isotope scaling of diatomic vibration](classical-mechanics.md#isotope-scaling-of-diatomic-vibration)
- [Linear rigid rotor](molecule.md#linear-rigid-rotor)
- [Linear Stark effect in the first excited hydrogen eigenspace](mathematical-physics.md#linear-stark-effect-in-the-first-excited-hydrogen-eigenspace)
- [Molecular rotation](molecule.md#molecular-rotation)
- [Molecular vibration](molecule.md#molecular-vibration)
- [Nondegenerate energy eigenvalue](quantum-mechanics.md#nondegenerate-energy-eigenvalue)
- [Nuclear energy level](quantum-mechanics.md#nuclear-energy-level)
- [One-magnon Bloch states on a ring](statistical-physics.md#one-magnon-bloch-states-on-a-ring)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2012/paper-1.md#2/a/solution)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2017.md#3/solution)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2021.md#section-a/2/solution)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2021.md#section-b/6/d/solution)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2022.md#section-a/1/solution)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2022.md#section-a/3/solution)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2022.md#section-b/4/c/solution)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2022.md#section-b/4/d/solution)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2022.md#section-b/4/e/solution)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2022.md#section-b/5/a/solution)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2022.md#section-b/5/b/solution)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2022.md#section-b/6/e/solution)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2021/paper-1.md#a1/b/iv/solution)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2021/paper-1.md#a2/a/ii/solution)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2022/paper-1.md#a1/b/ii/solution)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2023/paper-1.md#a1/a/solution)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2024/paper-1.md#a1/a/iii/solution)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2024/paper-1.md#a1/b/i/solution)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2024/paper-1.md#a2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-1.md#9a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-3.md#20a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-2.md#19d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-2.md#8d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-1.md#15g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1.md#33b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4.md#32b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3.md#33a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-1.md#14c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1.md#34b/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1.md#35b/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-2.md#15b/a/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2010/paper-2.md#section-a/1/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-1.md#section-b/b7/a/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-1.md#section-b/b7/a/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-1.md#section-b/b8/a/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2021/paper-1.md#section-b/b7/b/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2021/paper-2.md#section-c/c8/a/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2022/paper-1.md#section-a/1/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2022/paper-1.md#section-b/b6/b/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2022/paper-1.md#section-d/d9/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1.md#section-d/d13/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022.md#section-b/9/a/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1.md#section-a/a1/solution)
- [Solution](past-exam-of-the-theoretical-physics-ii-course-of-the-university-of-cambridge/2017.md#1/c/solution)
- [Pure rotational electric-dipole selection rules](molecule.md#pure-rotational-electric-dipole-selection-rules)
- [Quantum harmonic oscillator](quantum-harmonic-oscillator.md)
- [Quantum mechanics](quantum-mechanics.md)
- [Quantum quench](quantum-mechanics.md#quantum-quench)
- [Quantum state continuity at a finite Hamiltonian step](quantum-mechanics.md#quantum-state-continuity-at-a-finite-hamiltonian-step)
- [Quantum variational principle](quantum-mechanics.md#quantum-variational-principle)
- [Rotational energy](molecule.md#rotational-energy)
- [Rotational partition functions of hydrogen](molecule.md#rotational-partition-functions-of-hydrogen)
- [Rotational Raman spectroscopy](molecule.md#rotational-raman-spectroscopy)
- [Rotational state populations](molecule.md#rotational-state-populations)
- [Spin isomers of hydrogen](molecule.md#spin-isomers-of-hydrogen)
- [Stark effect](mathematical-physics.md#stark-effect)
- [Stark effect of the hydrogen ground state](mathematical-physics.md#stark-effect-of-the-hydrogen-ground-state)
- [Stern-Gerlach force and flight model](angular-momentum-operator.md#stern-gerlach-force-and-flight-model)
- [Stipulated bond dissociation model](chemical-bond.md#stipulated-bond-dissociation-model)
- [Three-level observable and missing spectral line](quantum-mechanics.md#three-level-observable-and-missing-spectral-line)
- [Three spin-one-half angular-momentum decomposition](angular-momentum-operator.md#three-spin-one-half-angular-momentum-decomposition)
- [Time-independent Schrödinger equation](mathematical-physics.md#time-independent-schrodinger-equation)
- [Two-level sudden quench](quantum-mechanics.md#two-level-sudden-quench)
- [University of Florida HCl and DCl FTIR experiment](molecule.md#university-of-florida-hcl-and-dcl-ftir-experiment)
- [Variational method](quantum-theory.md#variational-method)
- [Wannier-Mott exciton](quantum-mechanics.md#wannier-mott-exciton)
- [Weyl Hamiltonian](relativistic-quantum-field.md#weyl-hamiltonian)
- [Zeeman populations from an unpolarized angular-momentum multiplet](atomic-physics.md#zeeman-populations-from-an-unpolarized-angular-momentum-multiplet)
