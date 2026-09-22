# Spin model

↑ **Parent:** [Statistical physics](statistical-physics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spin_model)

A spin model assigns a discrete or continuous spin variable to each site of a [lattice](mathematical-logic.md#lattice) or vertex of a graph and gives interacting configurations a [Boltzmann factor](canonical-ensemble.md#boltzmann-factor). Spin models describe collective order and phase transitions in magnetic and other many-body systems.

**Table of contents**

- [Spin configuration](#spin-configuration)
- [Spin glass](#spin-glass)
  - [Frustrated Ising triangle](#frustrated-ising-triangle)
  - [Edwards-Anderson model](#edwards-anderson-model)
  - [Edwards-Anderson order parameter](#edwards-anderson-order-parameter)
  - [Spin overlap](#spin-overlap)
  - [Replica symmetry breaking](#replica-symmetry-breaking)
  - [Sherrington-Kirkpatrick model](#sherrington-kirkpatrick-model)
  - [Gold-iron alloy susceptibility experiment](#gold-iron-alloy-susceptibility-experiment)
  - [Origin of the replica approach to spin glasses](#origin-of-the-replica-approach-to-spin-glasses)
- [Annealed disorder](#annealed-disorder)
- [Quenched disorder](#quenched-disorder)
  - [Two-spin quenched and annealed free energies](#two-spin-quenched-and-annealed-free-energies)
  - [Replica trick](#replica-trick)
- [Potts model](#potts-model)
- [Blume–Emery–Griffiths model](#blume-emery-griffiths-model)
- [Transfer matrix for a classical spin chain](#transfer-matrix-for-a-classical-spin-chain)
  - [Classical Ising chain as a quantum particle](#classical-ising-chain-as-a-quantum-particle)
    - [Auxiliary-field transfer operator for an Ising chain](#auxiliary-field-transfer-operator-for-an-ising-chain)
    - [Double-well threshold of an auxiliary Ising potential](#double-well-threshold-of-an-auxiliary-ising-potential)
- [Spin magnetization](#spin-magnetization)
- [Spin inversion symmetry](#spin-inversion-symmetry)
- [Ising model](#ising-model)
  - [Ising-chain domain-wall energy convention](#ising-chain-domain-wall-energy-convention)
  - [Four-spin Ising ring](#four-spin-ising-ring)
    - [Ising ring bond correlation](#ising-ring-bond-correlation)
    - [Ising ring magnetization fluctuations](#ising-ring-magnetization-fluctuations)
  - [Exponentially coupled Ising inverse kernel](#exponentially-coupled-ising-inverse-kernel)
    - [Open-chain endpoint corrections for an exponential Ising kernel](#open-chain-endpoint-corrections-for-an-exponential-ising-kernel)
  - [Ising boundary condition](#ising-boundary-condition)
    - [Extremal infinite-volume Ising measures](#extremal-infinite-volume-ising-measures)
  - [Antiferromagnetic Ising model](#antiferromagnetic-ising-model)
    - [Two-sublattice Ising mean-field approximation](#two-sublattice-ising-mean-field-approximation)
      - [Uniform response of a two-sublattice Ising antiferromagnet](#uniform-response-of-a-two-sublattice-ising-antiferromagnet)
      - [Two-sublattice Ising variational free energy](#two-sublattice-ising-variational-free-energy)
  - [Ferromagnetic Ising lattice inequality](#ferromagnetic-ising-lattice-inequality)
  - [Ising spin variable](#ising-spin-variable)
  - [Mean-field theory of the Ising model](#mean-field-theory-of-the-ising-model)
    - [Mean-field Ising critical bifurcation](#mean-field-ising-critical-bifurcation)
    - [Bragg-Williams free energy of the Ising model](#bragg-williams-free-energy-of-the-ising-model)
    - [Ising auxiliary mean-field free energy](#ising-auxiliary-mean-field-free-energy)
  - [Curie–Weiss model](#curie-weiss-model)
  - [Transfer matrix for the one-dimensional Ising model](#transfer-matrix-for-the-one-dimensional-ising-model)
    - [Analyticity of the one-dimensional Ising free energy](#analyticity-of-the-one-dimensional-ising-free-energy)
    - [Ising-chain magnetization with spin-half normalization](#ising-chain-magnetization-with-spin-half-normalization)
  - [Blume–Capel model](#blume-capel-model)
    - [Blume-Capel mean-field transition at zero single-ion anisotropy](#blume-capel-mean-field-transition-at-zero-single-ion-anisotropy)
    - [Blume–Capel mean-field tricritical parameters](#blume-capel-mean-field-tricritical-parameters)
  - [Glauber dynamics](#glauber-dynamics)
  - [Free boundary condition](#free-boundary-condition)
  - [Plus boundary condition](#plus-boundary-condition)
  - [Peierls contour](#peierls-contour)
  - [One-dimensional Ising correlation function](#one-dimensional-ising-correlation-function)
  - [Spontaneous magnetization](#spontaneous-magnetization)
  - [Random-bond Ising model](#random-bond-ising-model)
  - [Transverse-field Ising model](#transverse-field-ising-model)
    - [Ising-chain quantum critical point](#ising-chain-quantum-critical-point)
    - [Ising-chain Bogoliubov diagonalization](#ising-chain-bogoliubov-diagonalization)
      - [Ising-chain ground-state energy](#ising-chain-ground-state-energy)
        - [Ising-chain field derivative and transverse polarization](#ising-chain-field-derivative-and-transverse-polarization)
          - [Critical transverse polarization of an Ising chain](#critical-transverse-polarization-of-an-ising-chain)
      - [Ising-chain quasiparticle dispersion](#ising-chain-quasiparticle-dispersion)
        - [Finite-ring parity qualification of an Ising quasiparticle gap](#finite-ring-parity-qualification-of-an-ising-quasiparticle-gap)

## Spin configuration

↑ **Parent:** [Spin model](spin-model.md)

A [spin configuration](#spin-configuration) specifies the [spin](angular-momentum-operator.md#spin) variable at every site of a [spin model](spin-model.md). For $N$ [Ising spins](#ising-spin-variable), it is a member of $\{-1,1\}^N$.

## Spin glass

↑ **Parent:** [Spin model](spin-model.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spin_glass)

A [spin glass](#spin-glass) has frozen, irregular local [spin magnetization](#spin-magnetization) without the periodic magnetic order of a simple [ferromagnet](electromagnetism.md#ferromagnet) or [antiferromagnet](electromagnetism.md#antiferromagnetism). Competing interactions and [quenched disorder](#quenched-disorder) make the distinction important: zero average [magnetization](electromagnetism.md#magnetization) need not mean that every [spin](angular-momentum-operator.md#spin) is freely fluctuating.[pp. 1792–1794, introduction and interpretation of the frozen-moment order parameter](physics-bibliography.md#solvable-model-of-a-spin-glass-by-david-sherrington-and-scott-kirkpatrick)

The [frustrated Ising triangle](#frustrated-ising-triangle) gives a small example of incompatible local preferences. The [Edwards-Anderson order parameter](#edwards-anderson-order-parameter) and [spin overlap](#spin-overlap) then ask a different question: how can one describe persistent local order when averaging the [spins](angular-momentum-operator.md#spin) themselves hides it? These concepts also connect interacting magnets to the [energy](energy.md) minima used by a [Hopfield network](statistical-learning.md#hopfield-network) to retrieve a memory. The triangle below illustrates frustration, without establishing a macroscopic [spin glass](#spin-glass) phase.

### Frustrated Ising triangle

↑ **Parent:** [Spin glass](#spin-glass)

Take three [Ising spins](#ising-spin-variable) $s_i\in\{-1,1\}$, with an [antiferromagnetic](electromagnetism.md#antiferromagnetism) interaction of [energy](energy.md) scale $J$ on each [edge](graph-theory.md#edge-of-a-graph) of a triangle. An individually satisfied bond has $s_is_j=-1$. But multiplying all three bond products gives $(s_1s_2)(s_2s_3)(s_3s_1)=1$, whereas three satisfied bonds would give $-1$. At least one bond must therefore remain unsatisfied. This is an exactly finite example of [geometrical frustration](statistical-physics.md#geometrical-frustration).

There are six [ground states](quantum-mechanics.md#ground-state) with one unsatisfied bond and **ground-state energy $-J$**. The two all-aligned [microstates](statistical-physics.md#microstate) have [energy](energy.md) $3J$. No interaction is switched off in a [ground state](quantum-mechanics.md#ground-state): the system minimizes their sum by accepting one local disappointment. Allowing continuous three-component [spins](angular-momentum-operator.md#spin) instead of [Ising spins](#ising-spin-variable) changes this optimization problem and permits the $120$-degree arrangement described under [geometrical frustration](statistical-physics.md#geometrical-frustration).

<a id="image-an-antiferromagnetic-ising-triangle-and-its-complete-finite-energy-spectrum"></a>
![](frustrated-ising-triangle-states.png)

**[Figure 1](#image-an-antiferromagnetic-ising-triangle-and-its-complete-finite-energy-spectrum). An antiferromagnetic Ising triangle and its complete finite energy spectrum**. [Source](frustrated-ising-triangle-states.py). The blue solid bonds are satisfied and the orange dashed bonds are unsatisfied. The histogram counts all eight configurations of the stipulated three-spin model. It contains no experimental measurements.

Writing $\beta=1/(k_BT)$ for [inverse temperature](temperature.md#inverse-temperature), the exact [partition function](canonical-ensemble.md#canonical-partition-function) and mean [internal energy](internal-energy.md) are

$$
Z=6e^{\beta J}+2e^{-3\beta J},\qquad
\langle H\rangle=\frac{-6Je^{\beta J}+6Je^{-3\beta J}}{6e^{\beta J}+2e^{-3\beta J}}.
$$

At $T>0$ these expressions are smooth: **a finite triangle has no thermodynamic phase transition**. In zero [magnetic field](magnetic-field.md), [spin inversion symmetry](#spin-inversion-symmetry) also gives $\langle s_i\rangle=0$ at every site, even as the [Boltzmann distribution](thermodynamics.md#boltzmann-distribution) concentrates on the six frustrated [ground states](quantum-mechanics.md#ground-state).

### Edwards-Anderson model

↑ **Parent:** [Spin glass](#spin-glass)

A common Ising version of the [Edwards-Anderson model](#edwards-anderson-model) places [Ising spins](#ising-spin-variable) on a [lattice](mathematical-logic.md#lattice) with short-range, fixed random interactions $J_{ij}$. The displayed sum counts each interacting pair once; positive $J_{ij}$ favors equal [spins](angular-momentum-operator.md#spin), negative $J_{ij}$ favors opposite [spins](angular-momentum-operator.md#spin). Different samples retain different couplings. [Quenched disorder](#quenched-disorder) describes this fixed-sample averaging.[§III, equation (1), nearest-neighbour random-coupling model; the pair-counting and field conventions here are stated explicitly](physics-bibliography.md#nobel-lecture-multiple-equilibria-by-giorgio-parisi)

### Edwards-Anderson order parameter

↑ **Parent:** [Spin glass](#spin-glass)

The [Edwards-Anderson order parameter](#edwards-anderson-order-parameter) measures squared local [spin magnetization](#spin-magnetization) within a selected equilibrium state $\alpha$. Squaring prevents opposite local orientations from cancelling. The state selection and limits matter: the full finite, zero-field [canonical ensemble](canonical-ensemble.md) has $\langle s_i\rangle=0$ by [spin inversion symmetry](#spin-inversion-symmetry), so substituting that average would miss broken-state order.[p. 1, replica and squared-local-moment order parameter; finite-system state selection is distinguished explicitly here](physics-bibliography.md#50-years-of-spin-glass-theory-by-david-sherrington-and-scott-kirkpatrick)

### Spin overlap

↑ **Parent:** [Spin glass](#spin-glass)

For two [spin configurations](#spin-configuration) $s,t$ on the same $N$ sites, their [spin overlap](#spin-overlap) is $+1$ when they agree everywhere and $-1$ when they are opposite everywhere. Two independent [canonical ensemble](canonical-ensemble.md) draws must use the same [quenched disorder](#quenched-disorder). Otherwise their comparison mixes changes of thermal state with changes of material sample.

An original finite example uses the six equally weighted [ground states](quantum-mechanics.md#ground-state) of the [frustrated Ising triangle](#frustrated-ising-triangle). For each first configuration, the second has one identical choice, one fully reversed choice, two choices differing at one site and two differing at two sites. Thus the [probability distribution](probability-distribution.md) of [spin overlap](#spin-overlap) is

$$
P(q=1)=P(q=-1)=\frac16,\qquad
P(q=1/3)=P(q=-1/3)=\frac13.
$$

It is symmetric, with $\langle q\rangle=0$ but $\langle q^2\rangle=11/27$. At infinite [temperature](temperature.md), all eight [microstates](statistical-physics.md#microstate) are equally probable and instead $\langle q^2\rangle=1/3$. This computable change in similarity statistics is a finite-model fact, not evidence for [replica symmetry breaking](#replica-symmetry-breaking).

### Replica symmetry breaking

↑ **Parent:** [Spin glass](#spin-glass)

[Giorgio Parisi](physicist.md#giorgio-parisi)'s 1979 work replaced a single replica [order parameter](critical-phenomenon.md#order-parameter) by an infinite hierarchy in the [mean-field theory](statistical-physics.md#mean-field-theory) of [spin glasses](#spin-glass). The claim concerns a thermodynamic model, rather than inequivalence of the labels attached to two finite laboratory copies.[Abstract, 3 December 1979: an infinite number of order parameters in mean-field replica theory](physics-bibliography.md#infinite-number-of-order-parameters-for-spin-glasses-by-giorgio-parisi)

For equilibrium states with weights $w_\alpha$ and local means $m_i^\alpha$, define $Q_{\alpha\gamma}=N^{-1}\sum_i m_i^\alpha m_i^\gamma$. The distribution $P_J(q)=\sum_{\alpha,\gamma}w_\alpha w_\gamma\delta(q-Q_{\alpha\gamma})$ records their similarities. This state-based overlap distribution is distinct from the finite instantaneous [spin overlap](#spin-overlap) used in the triangle example.[§V, equations (12)–(14), overlaps between equilibrium states and their sample-dependent distribution](physics-bibliography.md#nobel-lecture-multiple-equilibria-by-giorgio-parisi)

### Sherrington-Kirkpatrick model

↑ **Parent:** [Spin glass](#spin-glass)

The [Sherrington-Kirkpatrick model](#sherrington-kirkpatrick-model) couples every distinct pair of [Ising spins](#ising-spin-variable) using independent standard [normal random variables](probability-distribution.md#gaussian-random-variable) $z_{ij}$ for $i<j$, with $J_{ji}=J_{ij}$. Here $J_0$ and $\mathcal J$ have units of [energy](energy.md). [David Sherrington](physicist.md#david-sherrington) and [Scott Kirkpatrick](computer-science.md#scott-kirkpatrick) introduced this scaling in 1975; their original replica-symmetric calculation gave an unphysical negative low-temperature [entropy](entropy.md). The model and that initial proposed solution must be distinguished.[pp. 1793 and 1795, coupling scaling (2), replica-symmetric assumption and acknowledged negative entropy](physics-bibliography.md#solvable-model-of-a-spin-glass-by-david-sherrington-and-scott-kirkpatrick)

### Gold-iron alloy susceptibility experiment

↑ **Parent:** [Spin glass](#spin-glass)

[V. Cannella](physicist.md#vincent-cannella) and [J. A. Mydosh](physicist.md#john-a-mydosh) measured low-field [magnetic susceptibility](statistical-physics.md#magnetic-susceptibility) of [gold](chemical-substance.md#gold)-[iron](chemical-substance.md#iron) [alloys](chemical-substance.md#alloy) using a [mutual inductance](electromagnetism.md#mutual-inductance) bridge. Moving samples into and out of the pickup arrangement separated their signal from the background. Cooling revealed sharp susceptibility cusps; changing concentration, sample shape and applied [magnetic field](magnetic-field.md) tested their interpretation. Larger fields rounded the peaks. Their 1972 paper interpreted low-concentration ordering in antiferromagnetic terms: the cusp alone did not demonstrate Parisi's later theory.[§III, p. 4224, mutual-inductance method; §V, pp. 4228–4230, figures 9–12 and field/shape comparisons; abstract for the authors' contemporary interpretation](physics-bibliography.md#magnetic-ordering-in-gold-iron-alloys-by-vincent-cannella-and-john-a-mydosh)

This experiment measures a response to a small applied perturbation, rather than directly photographing frozen [spins](angular-momentum-operator.md#spin). Comparing field strengths is essential because the probing [magnetic field](magnetic-field.md) itself changes the response.[§V.A, pp. 4229–4230, weak-field cusp rounding](physics-bibliography.md#magnetic-ordering-in-gold-iron-alloys-by-vincent-cannella-and-john-a-mydosh)

### Origin of the replica approach to spin glasses

↑ **Parent:** [Spin glass](#spin-glass)

In his 1985 recollection, [Sam Edwards](physicist.md#sam-edwards) traced his work with [Philip Warren Anderson](physicist.md#philip-warren-anderson) to Saturday discussions and an analogy with randomly crosslinked polymers. He adapted methods from rubber theory during train journeys while chairing the Science Research Council.[Edwards, commentary dated 17 July 1985, published 16 September 1985, collaboration and train journeys](physics-bibliography.md#citation-classic-commentary-on-theory-of-spin-glasses-by-sam-edwards)

## Annealed disorder

↑ **Parent:** [Spin model](spin-model.md)

[Annealed disorder](#annealed-disorder) allows the variables representing disorder to equilibrate along with the [spins](angular-momentum-operator.md#spin). With a specified normalized prior measure over couplings, its [partition function](canonical-ensemble.md#canonical-partition-function) is the average $\mathbb E_J Z_J$. This differs from preparing samples with fixed couplings and averaging their measured thermodynamics, as in [quenched disorder](#quenched-disorder).[§4.2, pp. 83–86, fixed disorder versus annealed partition-function averaging](physics-bibliography.md#out-of-equilibrium-dynamics-of-complex-systems-by-leticia-fernanda-cugliandolo)

## Quenched disorder

↑ **Parent:** [Spin model](spin-model.md)

[Quenched disorder](#quenched-disorder) is randomness held fixed while the other degrees of freedom equilibrate. For a sample with couplings $J$, first compute its [partition function](canonical-ensemble.md#canonical-partition-function) $Z_J$ and [Helmholtz free energy](thermodynamic-potential.md#helmholtz-free-energy) $-k_BT\log Z_J$, then average over samples. One must not silently replace $\mathbb E_J\log Z_J$ by $\log\mathbb E_J Z_J$.[§4.2, pp. 83–86, averaging the free energy after computing each fixed-disorder partition function](physics-bibliography.md#out-of-equilibrium-dynamics-of-complex-systems-by-leticia-fernanda-cugliandolo)

### Two-spin quenched and annealed free energies

↑ **Parent:** [Quenched disorder](#quenched-disorder)

Choose two [Ising spins](#ising-spin-variable) with [Hamiltonian](hamiltonian-mechanics.md#hamiltonian) $H=-Js_1s_2$, where $J$ independently takes $J_0$ or $2J_0$ with equal prior [probabilities](probability-theory.md#probability) and $J_0>0$. This original finite example has no [geometrical frustration](statistical-physics.md#geometrical-frustration) and no [phase transition](critical-phenomenon.md#phase-transition). Its four spin assignments give $Z_J=4\cosh(\beta J)$. Therefore

$$
F_{\rm q}=-\frac{k_BT}{2}\left\{\log[4\cosh(\beta J_0)]+\log[4\cosh(2\beta J_0)]\right\},\qquad
F_{\rm a}=-k_BT\log\left\{2[\cosh(\beta J_0)+\cosh(2\beta J_0)]\right\}.
$$

The [concave function](real-analysis.md#concave-function) $\log$ puts $F_{\rm a}\leq F_{\rm q}$. For this two-value case the claim is just $(Z_1+Z_2)/2\geq\sqrt{Z_1Z_2}$, obtained by squaring $\sqrt{Z_1}-\sqrt{Z_2}$. Thus no formal continuation of replicas is needed to see the distinction.

<a id="image-exact-quenched-and-annealed-averages-for-a-stipulated-two-spin-system"></a>
![](quenched-annealed-two-spin-free-energy.png)

**[Figure 2](#image-exact-quenched-and-annealed-averages-for-a-stipulated-two-spin-system). Exact quenched and annealed averages for a stipulated two-spin system**. [Source](quenched-annealed-two-spin-free-energy.py). The same two bond strengths and equal prior weights are used in both ensembles. The right panel shows that annealed equilibrium reweights the bond strengths, whereas a quenched collection keeps half its samples at each strength. All curves are exact finite-model calculations, not alloy measurements.

In the [annealed disorder](#annealed-disorder) ensemble, the stronger bond has probability $Z_{2J_0}/(Z_{J_0}+Z_{2J_0})$, approaching one at low [temperature](temperature.md). A [quenched disorder](#quenched-disorder) collection instead retains one half at each coupling. As $T\to0$, **$F_{\rm q}\to-3J_0/2$ and $F_{\rm a}\to-2J_0$**: averaging samples and allowing the material variables to equilibrate describe different physics.

### Replica trick

↑ **Parent:** [Quenched disorder](#quenched-disorder)

For positive $Z$, the displayed identity follows by differentiating $Z^n=e^{n\log Z}$ at zero.

Integer powers of a [partition function](canonical-ensemble.md#canonical-partition-function) represent independent copies with the same disorder. Integer moments alone do not justify [analytic continuation](holomorphic-function.md#analytic-continuation) or interchanging disorder averages and [thermodynamic limits](statistical-physics.md#thermodynamic-limit).[Edwards, 1985 commentary, replica averaging and acknowledged mathematical limitations](physics-bibliography.md#citation-classic-commentary-on-theory-of-spin-glasses-by-sam-edwards)

## Potts model

↑ **Parent:** [Spin model](spin-model.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Potts_model)

The ferromagnetic [Potts model](#potts-model) on a finite [graph](graph.md) assigns $q$ possible states to each [graph vertex](graph.md#vertex-graph-theory) and rewards neighbouring equal states by the displayed weight, for $\beta\geq0$. The interaction sum counts each unoriented edge once. The [Edwards-Sokal coupling](site-percolation.md#edwards-sokal-coupling) identifies its spin clusters with the [random-cluster model](site-percolation.md#random-cluster-model) at $p=1-e^{-\beta}$ and integer $q\geq2$.

<h2 id="blume-emery-griffiths-model">Blume–Emery–Griffiths model</h2>

↑ **Parent:** [Spin model](spin-model.md)

The classical Blume–Emery–Griffiths model uses spins $\sigma_i\in\{-1,0,1\}$ with both bilinear $\sigma_i\sigma_j$ and biquadratic $\sigma_i^2\sigma_j^2$ nearest-neighbour interactions, together with a single-site term proportional to $\sigma_i^2$. One convention is $H=-J\sum\sigma_i\sigma_j-L\sum\sigma_i^2\sigma_j^2-D\sum\sigma_i^2-h\sum\sigma_i$. Signs of the single-site parameter vary across conventions. Setting $L=0$ gives a [Blume–Capel model](#blume-capel-model) after matching that sign convention. The one-dimensional version admits an exact [spin-chain transfer matrix](#transfer-matrix-for-a-classical-spin-chain).

## Transfer matrix for a classical spin chain

↑ **Parent:** [Spin model](spin-model.md)

For a nearest-neighbour classical chain with finitely many spin states and dimensionless bond energy $E(s,t)$, its transfer [matrix](vector-space.md#matrix) is $W_{st}=e^{-E(s,t)}$. On-site energies are divided between adjacent bonds. [Periodic boundary conditions](differential-equation.md#periodic-boundary-conditions) give [partition function](canonical-ensemble.md#canonical-partition-function) $Z_N=\operatorname{tr}W^N$ by direct multiplication and summation over spin labels. For a strictly positive [symmetric matrix](linear-algebra.md#symmetric-matrix), the [Perron–Frobenius theorem](vector-space.md#perron-frobenius-theorem) gives $\lim_{N\to\infty}N^{-1}\log Z_N=\log\lambda_{\max}$. A diagonal local observable $O$ has [expectation](expected-value.md) $\operatorname{tr}(OW^N)/Z_N$, tending to $v_{\max}^TOv_{\max}$ for a normalized dominant [eigenvector](linear-operator-theory.md#eigenvector).

### Classical Ising chain as a quantum particle

↑ **Parent:** [Transfer matrix for a classical spin chain](#transfer-matrix-for-a-classical-spin-chain)

Hubbard-Stratonovich decoupling of an exponentially coupled Ising chain gives a scalar-field action with a nearest-neighbor [gradient](multivariable-calculus.md#gradient) term and $U(m)=\tanh(\kappa/2)m^2/J-\log[2\cosh(2m+h)]$. Its continuum [partition function](canonical-ensemble.md#canonical-partition-function) is the [Euclidean path integral](quantum-field-theory.md#euclidean-path-integral) of the displayed quantum particle. At zero field the potential can have two wells, but a finite barrier still permits [quantum tunnelling](quantum-mechanics.md#quantum-tunnelling) and gives a unique symmetric [ground state](quantum-mechanics.md#ground-state). The excitation gap produces a finite classical [correlation length](critical-phenomenon.md#correlation-length), so there is no finite-temperature spontaneous magnetization for fixed positive $\kappa$. One classical spatial coordinate becomes imaginary time; a $d$-dimensional classical model corresponds to a quantum model with $d-1$ spatial dimensions.

#### Auxiliary-field transfer operator for an Ising chain

↑ **Parent:** [Classical Ising chain as a quantum particle](#classical-ising-chain-as-a-quantum-particle)

For a nearest-neighbor auxiliary-field representation of an [Ising model](#ising-model), sharing each local potential between adjacent bonds gives the displayed symmetric [integral operator](functional-analysis.md#integral-operator). Its periodic [partition function](canonical-ensemble.md#canonical-partition-function) is the trace of its $N$th power, up to Gaussian normalization constants. In the slowly varying continuum limit, a slice of length $\epsilon$ has kernel $[M/(2\pi\epsilon)]^{1/2}\exp[-M(m'-m)^2/(2\epsilon)-\epsilon\{U(m')+U(m)\}/2]$. Expanding its action on a smooth function gives $1-\epsilon\widehat H+O(\epsilon^2)$, with $\widehat H=-(2M)^{-1}\partial_m^2+U$. Thus fixed endpoints give an imaginary-time transition kernel and periodic endpoints give a [Euclidean path integral](quantum-field-theory.md#euclidean-path-integral) trace. The finite-spacing integral operator and the continuum differential operator need not have identical high-energy spectra.

#### Double-well threshold of an auxiliary Ising potential

↑ **Parent:** [Classical Ising chain as a quantum particle](#classical-ising-chain-as-a-quantum-particle)

The zero-field [Hubbard–Stratonovich transformation](quantum-field-theory.md#hubbard-stratonovich-transformation) of an exponentially coupled [Ising model](#ising-model) produces $U(m)=Am^2-\log[2\cosh(2m)]$, where $A=\tanh(\kappa/2)/J>0$. Since $U''(0)=2A-4$ and $U$ tends to positive infinity, a symmetric double well exists exactly when $A<2$. Its nonzero stationary points solve $Am=\tanh(2m)$; the ratio $\tanh(2m)/m$ decreases from 2 to 0 for $m>0$, proving that there is exactly one positive minimum. At $A=2$ the minimum is a single quartic minimum. A small conjugate field adds $-h\tanh(2m)+O(h^2)$ and tilts the wells, while a sufficiently large field can remove the metastable well. A finite barrier permits [quantum tunnelling](quantum-mechanics.md#quantum-tunnelling); two classical minima alone do not establish [spontaneous symmetry breaking](quantum-field-theory.md#spontaneous-symmetry-breaking).

## Spin magnetization

↑ **Parent:** [Spin model](spin-model.md)

The spin magnetization is the average signed spin of a discrete spin system. For $S_i\in\{-1,1\}$, $k$ positive spins give $M=-1+2k/n$. Multiplying by the magnetic moment per spin and the spin density relates this dimensionless average to physical [magnetization](electromagnetism.md#magnetization).

## Spin inversion symmetry

↑ **Parent:** [Spin model](spin-model.md)

Spin inversion symmetry means that simultaneous reversal of every spin leaves the [probability distribution](probability-distribution.md) or [energy](energy.md) unchanged. For a finite spin model with this symmetry, the weights of opposite configurations pair up, so every observable that changes sign under the reversal has zero [expected value](expected-value.md). An applied magnetic field generally breaks this symmetry.

## Ising model

↑ **Parent:** [Spin model](spin-model.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ising_model)

The [Ising model](#ising-model) is a [spin model](spin-model.md) with an [Ising spin](#ising-spin-variable) $\sigma_v\in\{-1,1\}$ at every [graph vertex](graph.md#vertex-graph-theory) $v$. For a finite [graph](graph.md) with vertex set $V$ and edge set $E$, a uniform coupling $J$ and field parameter $h$ give the [Hamiltonian](hamiltonian-mechanics.md#hamiltonian)

$$
H(\sigma)=-J\sum_{\{v,w\}\in E}\sigma_v\sigma_w-h\sum_{v\in V}\sigma_v,\qquad
\beta=\frac{1}{k_BT}.
$$

Each [edge](graph-theory.md#edge-of-a-graph) is counted once. Here $T>0$ is [temperature](temperature.md), $k_B$ is the [Boltzmann constant](thermodynamics.md#boltzmann-constant), and $\beta$ is [inverse temperature](temperature.md#inverse-temperature); $J$ and $h$ have units of [energy](energy.md). For magnetic applications, $h$ includes the [magnetic moment](electromagnetism.md#magnetic-dipole-moment) multiplying the applied [magnetic field](magnetic-field.md). The [canonical ensemble](canonical-ensemble.md) assigns the [Boltzmann distribution](thermodynamics.md#boltzmann-distribution)

$$
P(\sigma)=\frac{e^{-\beta H(\sigma)}}{Z},\qquad
Z=\sum_{\tau\in\{-1,1\}^{V}}e^{-\beta H(\tau)}.
$$

The [partition function](canonical-ensemble.md#canonical-partition-function) $Z$ makes the [probabilities](probability-theory.md#probability) sum to one. Positive $J$ rewards equal neighboring [Ising spins](#ising-spin-variable), modeling [ferromagnetism](electromagnetism.md#ferromagnetism); negative $J$ rewards opposite neighbors, giving an [antiferromagnetic Ising model](#antiferromagnetic-ising-model). Positive $h$ rewards $+1$, while negative $h$ rewards $-1$.[§5.2, equations (5.192)–(5.194), nearest-neighbor energy, field convention and canonical partition function](physics-bibliography.md#statistical-physics-by-david-tong)

A single local rule can organize a whole [graph](graph.md): rewarding agreement on each [edge](graph-theory.md#edge-of-a-graph) makes all-equal [Ising spin](#ising-spin-variable) patterns favorable even though no [edge](graph-theory.md#edge-of-a-graph) directly couples distant vertices. The [four-spin Ising ring](#four-spin-ising-ring) makes this visible with only sixteen [microstates](statistical-physics.md#microstate). It also separates three different questions: whether neighbors agree, whether the mean [spin magnetization](#spin-magnetization) is nonzero, and how large its [thermal fluctuations](statistical-physics.md#thermal-fluctuation) are.

A motivating experiment is the University of Colorado Boulder's Curie-temperature demonstration. An [iron](chemical-substance.md#iron) rod suspended from a twisting wire on a stand is initially held near a permanent magnet by [ferromagnetism](electromagnetism.md#ferromagnetism). A gas burner supplied from a propane cylinder heats the rod; the readout is its motion away from the magnet, followed by return as it cools. Repeated cooling supplies a reversible comparison on the same sample. The source explicitly calls for heating the rod while keeping the magnet cool, since heating the magnet can reduce its strength. The inference is that warming the sample weakens its magnetic attraction across the [Curie temperature](electromagnetism.md#curie-temperature). This is a qualitative [force](force.md) readout, with no calibrated [temperature](temperature.md) or [magnetization](electromagnetism.md#magnetization) trace supplied: it motivates competition between alignment and [thermal fluctuations](statistical-physics.md#thermal-fluctuation), but does not identify $J$, measure individual [Ising spins](#ising-spin-variable), or realize a [four-spin Ising ring](#four-spin-ising-ring).[Curie Temperature, Purpose, apparatus Figure 1, and Magnet Positioning: suspended iron rod, propane burner, cooling return, and keeping the magnet cool](physics-bibliography.md#curie-temperature-university-of-colorado-boulder-physics-undergraduate-labs)

[Ernst Ising](physicist.md#ernst-ising)'s 1925 paper examined a linear chain of two-orientation magnetic elements with neighboring interactions. In its calculation for a large chain, the zero-field mean [magnetization](electromagnetism.md#magnetization) vanishes and the model has no [spontaneous magnetization](#spontaneous-magnetization). The inspected English translation states this immediately after equation (8) in §2. This historical result concerns the chain; it does not establish the behavior of a two-dimensional [Ising model](#ising-model).[Beitrag zur Theorie des Ferromagnetismus by Ernst Ising (1925), English translation, §2 The simple linear chain, energy (3′) and the paragraph immediately after equation (8)](physics-bibliography.md#beitrag-zur-theorie-des-ferromagnetismus-by-ernst-ising)

### Ising-chain domain-wall energy convention

↑ **Parent:** [Ising model](#ising-model)

For $J>0$ and $S_i^z=\pm1/2$, a parallel bond has energy $-J/2$ while an antiparallel bond has $+J/2$. A wall therefore costs J, rather than the $2J$ of a differently normalized $-J\sum s_is_{i+1}$ model. At zero field its density is $[1-\tanh(\beta J/2)]/2$, positive at every nonzero [temperature](temperature.md). Walls occur in pairs on a periodic ring, but that global parity restriction does not remove their nonzero density in the [thermodynamic limit](statistical-physics.md#thermodynamic-limit). The low-temperature [correlation length](critical-phenomenon.md#correlation-length) is approximately $ae^{\beta J}/2$.

### Four-spin Ising ring

↑ **Parent:** [Ising model](#ising-model)

Take a [cycle graph](graph-theory.md#cycle-graph) with four labeled [graph vertices](graph.md#vertex-graph-theory) and four distinct [edges](graph-theory.md#edge-of-a-graph) $\{1,2\},\{2,3\},\{3,4\},\{4,1\}$. Set $h=0$, $J>0$, and impose [periodic boundary conditions](differential-equation.md#periodic-boundary-conditions) by writing $\sigma_5=\sigma_1$. The square drawing represents a one-dimensional ring: it has no diagonal interactions and is not a two-dimensional [lattice](mathematical-logic.md#lattice).

Call an [edge](graph-theory.md#edge-of-a-graph) between opposite [Ising spins](#ising-spin-variable) a [domain wall](critical-phenomenon.md#domain-wall). If $d$ is their number, the four bond products sum to $4-2d$, so the [energy](energy.md) is

$$
H=-4J+2Jd.
$$

Each [domain wall](critical-phenomenon.md#domain-wall) costs $2J$ relative to an aligned bond. Returning around the ring must return to the starting [Ising spin](#ising-spin-variable), so $d$ is even: equivalently, $\prod_{i=1}^{4}(\sigma_i\sigma_{i+1})=1$. Choosing an even set of $d$ wall [edges](graph-theory.md#edge-of-a-graph) and then choosing $\sigma_1$ determines the entire pattern. The [state degeneracy](statistical-physics.md#state-degeneracy) is therefore $g_d=2\binom{4}{d}$, using a [binomial coefficient](binomial-coefficient.md).

| [Domain walls](critical-phenomenon.md#domain-wall) $d$ | [State degeneracy](statistical-physics.md#state-degeneracy) $g_d$ | [Energy](energy.md) $H$ | Total [Boltzmann factor](canonical-ensemble.md#boltzmann-factor) weight |
| --- | --- | --- | --- |
| $0$ | $2$ | $-4J$ | $2e^{4\beta J}$ |
| $2$ | $12$ | $0$ | $12$ |
| $4$ | $2$ | $4J$ | $2e^{-4\beta J}$ |

The twelve middle [microstates](statistical-physics.md#microstate) consist of eight patterns with one exceptional [Ising spin](#ising-spin-variable) and four patterns with two adjacent $+1$ [Ising spins](#ising-spin-variable) and two adjacent $-1$ [Ising spins](#ising-spin-variable). The two alternating patterns have four [domain walls](critical-phenomenon.md#domain-wall). All $2+12+2=16$ [microstates](statistical-physics.md#microstate) are shown below.

<a id="image-all-sixteen-configurations-of-the-four-spin-ising-ring-grouped-by-domain-walls-and-energy"></a>
![](ising-four-spin-ring-configurations.png)

**[Figure 3](#image-all-sixteen-configurations-of-the-four-spin-ising-ring-grouped-by-domain-walls-and-energy). All sixteen configurations of the four-spin Ising ring, grouped by domain walls and energy**. Original enumeration of the four distinct ring [edges](graph-theory.md#edge-of-a-graph). Blue vertices denote $+1$ [Ising spins](#ising-spin-variable), orange vertices denote $-1$ [Ising spins](#ising-spin-variable), and dashed red [edges](graph-theory.md#edge-of-a-graph) mark [domain walls](critical-phenomenon.md#domain-wall). These are exact model configurations.

Writing $K=\beta J$, the [partition function](canonical-ensemble.md#canonical-partition-function) and the [probability](probability-theory.md#probability) of each [energy](energy.md) class are

$$
Z=2e^{4K}+12+2e^{-4K}=4\cosh(4K)+12,\qquad
P(d)=\frac{g_de^{K(4-2d)}}{Z}.
$$

For an original exact example, choose $K=(\ln2)/4$. Then $e^{4K}=2$, $Z=17$, and $P(d=0)=4/17$, $P(d=2)=12/17$, $P(d=4)=1/17$. Each aligned [microstate](statistical-physics.md#microstate) has [probability](probability-theory.md#probability) $2/17$, each middle [microstate](statistical-physics.md#microstate) $1/17$, and each alternating [microstate](statistical-physics.md#microstate) $1/34$: multiply by [state degeneracy](statistical-physics.md#state-degeneracy) before comparing whole classes. As $K\to0$, all sixteen [microstates](statistical-physics.md#microstate) become equally likely, but the class [probabilities](probability-theory.md#probability) approach $1/8,3/4,1/8$. As $K\to\infty$, the two all-aligned [microstates](statistical-physics.md#microstate) each have limiting [probability](probability-theory.md#probability) $1/2$.

#### Ising ring bond correlation

↑ **Parent:** [Four-spin Ising ring](#four-spin-ising-ring)

The [Ising ring bond correlation](#ising-ring-bond-correlation) is the neighboring [two-point correlation function](critical-phenomenon.md#two-point-correlation-function) $c_1=\langle\sigma_i\sigma_{i+1}\rangle$ in the [four-spin Ising ring](#four-spin-ising-ring). All four [edges](graph-theory.md#edge-of-a-graph) are equivalent. At zero field each mean [Ising spin](#ising-spin-variable) is zero by [spin inversion symmetry](#spin-inversion-symmetry), so $c_1$ also equals the [connected correlation function](critical-phenomenon.md#connected-correlation-function). Agreement gives bond product $+1$ and disagreement $-1$; thus $P(\sigma_i=\sigma_{i+1})=(1+c_1)/2$.

Differentiating the finite [partition function](canonical-ensemble.md#canonical-partition-function) with respect to $K=\beta J$ inserts the sum of four bond products. Therefore

$$
c_1=\frac14\frac{d\log Z}{dK}
=\frac{\sinh(4K)}{\cosh(4K)+3},\qquad
U=\langle H\rangle=-4Jc_1.
$$

Here $U$ is [internal energy](internal-energy.md). At $K=(\ln2)/4$, the class-weight calculation gives $c_1=(4-1)/17=3/17$ and $U=-12J/17$. The agreement [probability](probability-theory.md#probability) for a selected bond is $10/17$, despite the exactly zero mean [spin magnetization](#spin-magnetization).

A second [derivative](calculus.md#derivative) gives the [energy](energy.md) [variance](variance.md), and hence the [heat capacity](heat.md#heat-capacity) $C_H=dU/dT$ at fixed $J$ and $h=0$:

$$
\frac{\operatorname{Var}(H)}{J^2}
=\frac{d^2\log Z}{dK^2}
=\frac{16[1+3\cosh(4K)]}{[\cosh(4K)+3]^2},\qquad
\frac{C_H}{k_B}=K^2\frac{\operatorname{Var}(H)}{J^2}.
$$

To see the [variance](variance.md) identity directly, a [derivative](calculus.md#derivative) of an [expected value](expected-value.md) under weights $e^{KS}$ inserts $S-\langle S\rangle$, where $S=\sum_i\sigma_i\sigma_{i+1}=-H/J$. The factor $K^2$ follows from $dK/dT=-K/T$. At the same exact example, $\operatorname{Var}(H)/J^2=1216/289$. The [heat capacity](heat.md#heat-capacity) vanishes both as $K\to0$ and as $K\to\infty$: at high [temperature](temperature.md) its dimensionless factor $K^2$ vanishes, while at low [temperature](temperature.md) excited [microstates](statistical-physics.md#microstate) become exponentially rare.

#### Ising ring magnetization fluctuations

↑ **Parent:** [Four-spin Ising ring](#four-spin-ising-ring)

Define the instantaneous [spin magnetization](#spin-magnetization) $m=\frac14\sum_i\sigma_i$. Global reversal sends $m$ to $-m$ without changing the zero-field [energy](energy.md). Pairing every [microstate](statistical-physics.md#microstate) with its reversed partner proves $\langle m\rangle=0$ at every positive [temperature](temperature.md), even when almost all [probability](probability-theory.md#probability) lies on the two fully aligned patterns. A vanishing mean does not imply weak alignment: the limiting [probability distribution](probability-distribution.md) is half at $m=+1$ and half at $m=-1$.

The [Ising ring magnetization fluctuations](#ising-ring-magnetization-fluctuations) measure this distinction through [variance](variance.md). In the $d=0$ class, both patterns have $m^2=1$. Among the $d=2$ patterns, eight have $m^2=1/4$ and four have $m^2=0$; the two $d=4$ patterns also have $m^2=0$. Consequently

$$
\operatorname{Var}(m)=\langle m^2\rangle
=\frac{2e^{4K}+2}{Z}.
$$

It equals $6/17$ at $K=(\ln2)/4$, approaches $1/4$ for four independent fair [Ising spins](#ising-spin-variable) at $K\to0$, and approaches $1$ as $K\to\infty$. Unlike the [energy](energy.md) [variance](variance.md), the [spin magnetization](#spin-magnetization) [variance](variance.md) remains large in the low-[temperature](temperature.md) symmetric mixture.

<a id="image-exact-bond-correlation-magnetization-variance-and-heat-capacity-of-the-four-spin-ising-ring"></a>
![](ising-four-spin-ring-correlations.png)

**[Figure 4](#image-exact-bond-correlation-magnetization-variance-and-heat-capacity-of-the-four-spin-ising-ring). Exact bond correlation, magnetization variance and heat capacity of the four-spin Ising ring**. Original exact finite-ring calculations at $h=0$ and $J>0$, plotted against $K=\beta J$; increasing $K$ means cooling at fixed $J$. The marked point has $K=(\ln2)/4$, [Ising ring bond correlation](#ising-ring-bond-correlation) $3/17$ and [spin magnetization](#spin-magnetization) [variance](variance.md) $6/17$. These smooth curves are model predictions.

The same [thermal fluctuation](statistical-physics.md#thermal-fluctuation) controls the field response. Allow $h$ to vary before setting it to zero; differentiating the [Boltzmann distribution](thermodynamics.md#boltzmann-distribution) inserts $\beta\sum_i\sigma_i=4\beta m$, giving

$$
\left.\frac{\partial\langle m\rangle}{\partial h}\right|_{h=0}
=4\beta\operatorname{Var}(m).
$$

This is a spin-normalized [magnetic susceptibility](statistical-physics.md#magnetic-susceptibility) with respect to the [energy](energy.md)-valued parameter $h$; conversion to physical [magnetization](electromagnetism.md#magnetization) and [magnetic field](magnetic-field.md) requires the [magnetic moment](electromagnetism.md#magnetic-dipole-moment) and sample [volume](geometry-and-topology.md#volume) factors.

For finite $N$, $Z$ is a finite positive sum of [exponential functions](calculus.md#exponential-function). Its [free energy](thermodynamic-potential.md#thermodynamic-free-energy) $-k_BT\log Z$ is a [real analytic function](analysis.md#real-analytic-function) for $T>0$, so the smooth [heat capacity](heat.md#heat-capacity) peak here is not a critical [phase transition](critical-phenomenon.md#phase-transition). [Spontaneous magnetization](#spontaneous-magnetization) concerns the order of limits: first a [thermodynamic limit](statistical-physics.md#thermodynamic-limit), then removal of a symmetry-breaking field. The [four-spin Ising ring](#four-spin-ising-ring) alone establishes neither that limit nor any two-dimensional [Ising model](#ising-model) result.[§5.2.3, paragraph beginning with the analytic finite partition sum: phase transitions require the thermodynamic limit](physics-bibliography.md#statistical-physics-by-david-tong)

### Exponentially coupled Ising inverse kernel

↑ **Parent:** [Ising model](#ising-model)

For the infinite one-dimensional coupling [matrix](vector-space.md#matrix) $J_{ij}=Je^{-\kappa|i-j|}$ with $J,\kappa>0$, its Fourier symbol is $J\sinh\kappa/(\cosh\kappa-\cos q)$. Its inverse is nearest-neighbor even though the original interaction is not. The inverse quadratic form equals $[2J\sinh\kappa]^{-1}\sum_j(m_j-m_{j+1})^2+[\tanh(\kappa/2)/J]\sum_jm_j^2$. Finite open chains add endpoint corrections; a periodized coupling gives the same translation-invariant formula.

#### Open-chain endpoint corrections for an exponential Ising kernel

↑ **Parent:** [Exponentially coupled Ising inverse kernel](#exponentially-coupled-ising-inverse-kernel)

For $N\ge2$, the open-chain [Ising model](#ising-model) coupling $[J_N]_{ij}=J\rho^{|i-j|}$, $0<\rho<1$, has a tridiagonal inverse. Its endpoint diagonal entries are $1/[J(1-\rho^2)]$, its interior diagonal entries are $(1+\rho^2)/[J(1-\rho^2)]$, and adjacent off-diagonal entries are $-\rho/[J(1-\rho^2)]$. Direct [matrix multiplication](vector-space.md#matrix-multiplication) verifies the inverse because the geometric sequences cancel in every interior row. The displayed [quadratic form](quadratic-form.md) follows with $D=\rho/[J(1-\rho^2)]$, $A=(1-\rho)/[J(1+\rho)]$ and $B=\rho/[J(1+\rho)]$. For $\rho=e^{-\kappa}$, $D=(2J\sinh\kappa)^{-1}$ and $A=\tanh(\kappa/2)/J$. Omitting the endpoint term requires an infinite chain, a correctly periodized coupling, or a bulk [thermodynamic limit](statistical-physics.md#thermodynamic-limit).

### Ising boundary condition

↑ **Parent:** [Ising model](#ising-model)

A fixed [Ising boundary condition](#ising-boundary-condition) pins the [Ising spins](#ising-spin-variable) on a specified boundary, leaving the interior distributed with the original interaction weights. The boundary can be the inner [graph vertex](graph.md#vertex-graph-theory) boundary of a finite box, or an exterior neighboring set if that convention is explicitly chosen. Conditioning on pinned [Ising spins](#ising-spin-variable) preserves the [FKG lattice condition](probability-inequality.md#fkg-lattice-condition) of a ferromagnetic [Ising model](#ising-model). The [FKG inequality](probability-inequality.md#fkg-inequality) then makes interior expectations of [increasing observables](set.md#increasing-function-on-a-partially-ordered-set) nondecreasing in the pinned boundary [Ising spins](#ising-spin-variable).

#### Extremal infinite-volume Ising measures

↑ **Parent:** [Ising boundary condition](#ising-boundary-condition)

For the ferromagnetic binary [Ising model](#ising-model), all-zero boundary measures increase and all-one boundary measures decrease as boxes exhaust the [lattice](mathematical-logic.md#lattice), in [stochastic domination](probability-and-statistics.md#stochastic-domination-of-probability-measures). The nearest-neighbor spatial conditional [probability distribution](probability-distribution.md) reduces each domain comparison to a mixture of boundary conditions for the smaller box. [Probabilities](probability-theory.md#probability) that a specified finite set is all one consequently converge; [inclusion-exclusion](combinatorics.md#inclusion-exclusion-principle) gives convergence of every finite [Ising spin](#ising-spin-variable) pattern. Their consistent limits define the two extreme infinite-volume measures. Existence does not assert that the two limits coincide.

### Antiferromagnetic Ising model

↑ **Parent:** [Ising model](#ising-model)

With the convention $H=J\sum_{\langle ij\rangle}\sigma_i\sigma_j-h\sum_i\sigma_i$, positive $J$ favors opposite neighboring [Ising spins](#ising-spin-variable). On a [bipartite graph](bipartite-graph.md), the [Néel order parameter](statistical-physics.md#neel-order-parameter) measures opposite sublattice [magnetizations](electromagnetism.md#magnetization); it is distinct from the uniform [magnetization](electromagnetism.md#magnetization). Changing the signs of spins on one sublattice maps the zero-field model to the ferromagnetic [Ising model](#ising-model).

#### Two-sublattice Ising mean-field approximation

↑ **Parent:** [Antiferromagnetic Ising model](#antiferromagnetic-ising-model)

On a regular [bipartite graph](bipartite-graph.md) with coordination number $q$, replace each bond product by $\sigma_B\sigma_W\simeq M_W\sigma_B+M_B\sigma_W-M_BM_W$. For $N$ sites there are $Nq/2$ bonds, so the constant in the effective [Hamiltonian](hamiltonian-mechanics.md#hamiltonian) is $-NqJM_BM_W/2$. The [mean-field self-consistency equations](critical-phenomenon.md#self-consistency-equation) are $M_B=\tanh\beta(h+g-qJM_W)$ and $M_W=\tanh\beta(h-g-qJM_B)$. At zero fields the antisymmetric branch has a continuous [mean-field Ising critical bifurcation](#mean-field-ising-critical-bifurcation) at $k_BT_c=qJ$.

##### Uniform response of a two-sublattice Ising antiferromagnet

↑ **Parent:** [Two-sublattice Ising mean-field approximation](#two-sublattice-ising-mean-field-approximation)

On the stable zero-field branch $M_B=-M_W=M$, put $a=\beta(1-M^2)$. Differentiating the [two-sublattice Ising mean-field approximation](#two-sublattice-ising-mean-field-approximation) with respect to the uniform field gives $\chi_B=a(1-qJ\chi_W)$ and $\chi_W=a(1-qJ\chi_B)$. Thus $\chi_+=a/(1+qJa)$ and $\partial M_-/\partial h=0$. The true staggered [magnetic susceptibility](statistical-physics.md#magnetic-susceptibility), $\partial M_-/\partial g=a/(1-qJa)$, is a different response and diverges at the continuous transition. The factor $1-M^2$ is essential: the uniform response vanishes when the spins saturate at zero temperature.

##### Two-sublattice Ising variational free energy

↑ **Parent:** [Two-sublattice Ising mean-field approximation](#two-sublattice-ising-mean-field-approximation)

Here $s(m)=\frac{1+m}{2}\ln\frac{1+m}{2}+\frac{1-m}{2}\ln\frac{1-m}{2}$. This [free-energy density](statistical-physics.md#free-energy-density) is the [energy](energy.md) minus temperature times [entropy](entropy.md) of independent sublattice [Ising spins](#ising-spin-variable). Since $s'(m)=\operatorname{atanh}m$, stationarity yields the [two-sublattice Ising mean-field approximation](#two-sublattice-ising-mean-field-approximation). Writing $M_\pm=(M_B\pm M_W)/2$, the quadratic coefficients are $(k_BT+qJ)/2$ for $M_+^2$ and $(k_BT-qJ)/2$ for $M_-^2$. The positive quartic coefficient $k_BT/12$ in the staggered direction stabilizes the continuous transition. Unlike a log-cosh auxiliary potential, this variational expression can be minimized away from self-consistency.

### Ferromagnetic Ising lattice inequality

↑ **Parent:** [Ising model](#ising-model)

For $H(\sigma)=\sum_{xy}J_{xy}\sigma_x\sigma_y+\sum_xh_x\sigma_x$ on a finite graph, assume $J_{xy}\ge0$. Let $U=\{x:\sigma_x=1,\tau_x=-1\}$ and $W=\{x:\sigma_x=-1,\tau_x=1\}$. The displayed difference is $4\sum_{xy:\,x\in U,y\in W\text{ or conversely}}J_{xy}$: all other edge terms and all field terms cancel. Exponentiating proves the [FKG lattice condition](probability-inequality.md#fkg-lattice-condition) and hence [positive association of random variables](probability-theory.md#positive-association-of-random-variables) for this [Ising model](#ising-model).

### Ising spin variable

↑ **Parent:** [Ising model](#ising-model)

An Ising [Ising spin](#ising-spin-variable) variable is a classical two-state degree of freedom. Its thermal mean can lie anywhere in $[-1,1]$ even though each microscopic value is $-1$ or $1$. It should not be confused with an arbitrary quantum-spin operator. Products of neighbouring [Ising spins](#ising-spin-variable) supply the pair interactions of the [Ising model](#ising-model), and their average defines [spin magnetization](#spin-magnetization).

### Mean-field theory of the Ising model

↑ **Parent:** [Ising model](#ising-model)

The [mean-field approximation](critical-phenomenon.md#mean-field-approximation) neglects products of [Ising spin](#ising-spin-variable) deviations, replacing each [Ising spin](#ising-spin-variable)'s neighbours by the common [spin magnetization](#spin-magnetization). With [coordination number of a lattice](statistical-physics.md#coordination-number-of-a-lattice) $q$, the effective field is $h+qJm$. The [self-consistency equation](critical-phenomenon.md#self-consistency-equation) equates the assumed mean [Ising spin](#ising-spin-variable) with its independent-spin expectation in that effective field. It predicts $k_BT_c=qJ$ and the usual quartic [mean-field critical exponents](critical-phenomenon.md#mean-field-critical-exponent), while neglecting spatially correlated fluctuations.

#### Mean-field Ising critical bifurcation

↑ **Parent:** [Mean-field theory of the Ising model](#mean-field-theory-of-the-ising-model)

For a ferromagnetic [Ising model](#ising-model) with [coordination number of a lattice](statistical-physics.md#coordination-number-of-a-lattice) $z$, its [mean-field self-consistency equation](critical-phenomenon.md#self-consistency-equation) is $M=\tanh(zJM/(k_BT))$. Put $A=T_c/T$. For $A\leq1$, the only solution is zero. For $A>1$, [strict concavity](real-analysis.md#strict-concavity) of $\tanh(AM)-M$ on $M>0$ gives one positive solution and its spin-reversed partner. Expanding $\tanh(AM)=AM-(AM)^3/3+O(M^5)$ gives $M^2=3(A-1)/A^3+O((A-1)^2)$, proving a continuous onset with [order-parameter critical exponent](critical-phenomenon.md#order-parameter-critical-exponent) $\beta=1/2$. The [Bragg-Williams free energy of the Ising model](#bragg-williams-free-energy-of-the-ising-model) has a positive quartic coefficient at $T_c$, so these are the stable ordered minima rather than a first-order jump.

#### Bragg-Williams free energy of the Ising model

↑ **Parent:** [Mean-field theory of the Ising model](#mean-field-theory-of-the-ising-model)

A product trial distribution with actual mean [Ising spin](#ising-spin-variable) $m$ gives

$$
\frac{A_{\rm BW}}N=-\frac{qJ}{2}m^2-hm+k_BT\left[\frac{1+m}{2}\log\frac{1+m}{2}+\frac{1-m}{2}\log\frac{1-m}{2}\right].
$$

Its [entropy](entropy.md) is the sum of independent-spin entropies, with $0\log0=0$. Differentiation gives $k_BT\operatorname{arctanh}m=qJm+h$, the [self-consistency equation](critical-phenomenon.md#self-consistency-equation). The variational mean parameter is distinct from the assumed field parameter of the [Ising auxiliary mean-field free energy](#ising-auxiliary-mean-field-free-energy) until the equilibrium condition is imposed.

#### Ising auxiliary mean-field free energy

↑ **Parent:** [Mean-field theory of the Ising model](#mean-field-theory-of-the-ising-model)

The approximate [partition function](canonical-ensemble.md#canonical-partition-function) obtained by decoupling each Ising bond has this [free energy](thermodynamic-potential.md#thermodynamic-free-energy). The quadratic constant compensates double counting. Its stationary condition is the [self-consistency equation](critical-phenomenon.md#self-consistency-equation); away from stationarity $m$ parametrizes the assumed effective field and need not equal that distribution's mean [Ising spin](#ising-spin-variable). It agrees at [stationary points](calculus-of-variations.md#stationary-point) with the [Bragg-Williams free energy of the Ising model](#bragg-williams-free-energy-of-the-ising-model), although their off-equilibrium expansions differ.

<h3 id="curie-weiss-model">Curie–Weiss model</h3>

↑ **Parent:** [Ising model](#ising-model)

The zero-field ferromagnetic Curie–Weiss model is an [Ising model](#ising-model) on $n$ spins with an equal interaction between every pair. For $s_i\in\{-1,1\}$ and $\beta>0$, its normalized [probability mass function](probability-distribution.md#probability-mass-function) is $Z_{n,\beta}^{-1}\exp[\beta(\sum_is_i)^2/(2n)]$. The [partition function](canonical-ensemble.md#canonical-partition-function) $Z_{n,\beta}$ sums these weights over all configurations. The square includes constant diagonal terms; these affect only normalization. [Spin inversion symmetry](#spin-inversion-symmetry) makes every spin's [expected value](expected-value.md) zero, while grouping configurations by their [spin magnetization](#spin-magnetization) gives

$$
\mathbb P(M=m)=Z_{n,\beta}^{-1}\binom{n}{n(1+m)/2}e^{\beta nm^2/2}.
$$

Here $m=-1+2k/n$, $0\leq k\leq n$.

### Transfer matrix for the one-dimensional Ising model

↑ **Parent:** [Ising model](#ising-model)

For nearest-neighbour interactions, a two-by-two transfer matrix assigns one [Boltzmann factor](canonical-ensemble.md#boltzmann-factor) to every adjacent spin pair. With periodic boundary conditions, summing all spin configurations gives the [partition function](canonical-ensemble.md#canonical-partition-function) as the trace of a power of this matrix.

#### Analyticity of the one-dimensional Ising free energy

↑ **Parent:** [Transfer matrix for the one-dimensional Ising model](#transfer-matrix-for-the-one-dimensional-ising-model)

At real field and nonzero [temperature](temperature.md), every entry of the finite-range Ising transfer matrix is positive. Its largest eigenvalue is simple by the [Perron–Frobenius theorem](vector-space.md#perron-frobenius-theorem) and depends smoothly on field and temperature. The thermodynamic [free energy](thermodynamic-potential.md#thermodynamic-free-energy) per site is its negative logarithm times $k_BT$. In the nearest-neighbour chain it is analytic and the zero-field [magnetization](electromagnetism.md#magnetization) vanishes, despite exponentially long low-temperature correlations. Finite-volume spin-inversion symmetry alone would not suffice to exclude spontaneous thermodynamic order.

#### Ising-chain magnetization with spin-half normalization

↑ **Parent:** [Transfer matrix for the one-dimensional Ising model](#transfer-matrix-for-the-one-dimensional-ising-model)

For $H=-2J\sum S_i^zS_{i+1}^z-g\mu_BB\sum S_i^z$, with dimensionless $S_i^z=\pm1/2$, define $K=\beta J/2$ and $b=\beta g\mu_BB/2$. The [transfer matrix for the one-dimensional Ising model](#transfer-matrix-for-the-one-dimensional-ising-model) has largest eigenvalue $e^K[\cosh b+\sqrt{\sinh^2b+e^{-4K}}]$. Differentiating its logarithm gives the displayed moment per site. In particular the zero-field susceptibility per site is $(g\mu_B)^2e^{\beta J}/(4k_BT)$. Factors of two differ from a model whose spin variables themselves take values $\pm1$.

<h3 id="blume-capel-model">Blume–Capel model</h3>

↑ **Parent:** [Ising model](#ising-model)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Blume–Capel_model)

The Blume–Capel model is a [spin model](spin-model.md) with $\sigma_i\in\{-1,0,1\}$ and Hamiltonian

$$
H=-J\sum_{\langle i,j\rangle}\sigma_i\sigma_j+D\sum_i\sigma_i^2-h\sum_i\sigma_i.
$$

Competition between the [Ising interaction](#ising-model) and the single-ion anisotropy $D$ produces a [tricritical point](critical-phenomenon.md#tricritical-point) in its phase diagram.

#### Blume-Capel mean-field transition at zero single-ion anisotropy

↑ **Parent:** [Blume–Capel model](#blume-capel-model)

For spins $s_i\in\{-1,0,1\}$ with ferromagnetic nearest-neighbour exchange and no single-ion anisotropy, a homogeneous [mean-field approximation](critical-phenomenon.md#mean-field-approximation) gives

$$
\frac{F_{\rm MF}}N=\frac{zJ}{2}S^2-\frac1\beta\log[1+2\cosh\beta(zJS+B)].
$$

The [self-consistency equation](critical-phenomenon.md#self-consistency-equation) is $S=2\sinh h/(1+2\cosh h)$ with $h=\beta(zJS+B)$. Its small-$h$ expansion is $2h/3-h^3/9+O(h^5)$. Hence $k_BT_c=2zJ/3$ and, with $t=T/T_c-1$, the nonzero branches satisfy $S^2=(8/3)(-t)+O(t^2)$. The [critical exponent](critical-phenomenon.md#critical-exponent) is the mean-field value $1/2$, not an exact two-dimensional exponent. At zero source the finite-system equilibrium magnetization is zero by [spin inversion symmetry](#spin-inversion-symmetry); the broken branches describe the thermodynamic limit with a phase selected by a vanishing source.

<h4 id="blume-capel-mean-field-tricritical-parameters">Blume–Capel mean-field tricritical parameters</h4>

↑ **Parent:** [Blume–Capel model](#blume-capel-model)

For ferromagnetic exchange $J$ and coordination $z$, the [mean-field approximation](critical-phenomenon.md#mean-field-approximation) has $f=zJM^2/2-k_BT\log[1+2e^{-g/(k_BT)}\cosh(zJM/(k_BT))]$. With $K=zJ/(k_BT)$ and $q=2e^{-g/(k_BT)}/[1+2e^{-g/(k_BT)}]$, its quadratic and quartic coefficients vanish at $q=1/3$, $K=3$. The sextic coefficient of $f/(k_BT)$ is $9/40>0$. Hence $T_{\mathrm{TCP}}=zJ/(3k_B)$ and $g_{\mathrm{TCP}}=k_BT_{\mathrm{TCP}}\log4$; these are not exact finite-dimensional lattice values.

### Glauber dynamics

↑ **Parent:** [Ising model](#ising-model)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Glauber_dynamics)

Glauber dynamics is a local Markov chain for a spin system. In its heat-bath form, each step chooses one vertex and resamples that spin from its conditional Gibbs distribution given all other spins.

### Free boundary condition

↑ **Parent:** [Ising model](#ising-model)

A free boundary condition retains only interactions whose endpoints both lie in the finite volume and imposes no exterior spin values.

### Plus boundary condition

↑ **Parent:** [Ising model](#ising-model)

A plus boundary condition fixes every exterior spin adjacent to the finite volume to $+1$. The increasing-volume limit selects the maximal infinite-volume Gibbs state.

### Peierls contour

↑ **Parent:** [Ising model](#ising-model)

A Peierls contour is a dual-lattice boundary separating clusters of opposite Ising spins. Flipping the spins inside a contour of size $m$ changes its Boltzmann weight by the factor $e^{-2\beta m}$.

### One-dimensional Ising correlation function

↑ **Parent:** [Ising model](#ising-model)

For the zero-field nearest-neighbour Ising model on $\mathbb Z$,

$$
\langle\sigma_x\sigma_y\rangle=(\tanh\beta)^{|x-y|}.
$$

More generally, an even ordered product factors over alternating gaps.

### Spontaneous magnetization

↑ **Parent:** [Ising model](#ising-model)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spontaneous_magnetization)

Spontaneous magnetization is the magnetization that remains after taking the thermodynamic limit and then sending a symmetry-breaking external field to zero.

### Random-bond Ising model

↑ **Parent:** [Ising model](#ising-model)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Random-bond_Ising_model)

A random-bond Ising model has couplings whose signs or magnitudes vary between edges according to quenched disorder. Negative bonds frustrate neighboring spins that would otherwise align.

### Transverse-field Ising model

↑ **Parent:** [Ising model](#ising-model)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Transverse-field_Ising_model)

The transverse-field Ising model is a quantum spin model with competing Ising exchange and a perpendicular field, for example $H=-J\sum_iX_iX_{i+1}-h\sum_iZ_i$. In one dimension its ordered and paramagnetic phases meet at $|h/J|=1$.

#### Ising-chain quantum critical point

↑ **Parent:** [Transverse-field Ising model](#transverse-field-ising-model)

For positive ferromagnetic exchange and nonnegative transverse field, the [Ising-chain quasiparticle dispersion](#ising-chain-quasiparticle-dispersion) closes its gap at $g=1$, with $\epsilon_k\sim2J|k|$. This is the [quantum phase transition](critical-phenomenon.md#quantum-phase-transition) between the model's ordered and field-polarized regimes. The exact dispersion identifies the gapless scale; computing its order parameter additionally requires ground-state correlations.

#### Ising-chain Bogoliubov diagonalization

↑ **Parent:** [Transverse-field Ising model](#transverse-field-ising-model)

For a paired non-self-conjugate [momentum](momentum.md), rotate the [Ising-chain Nambu spinor](quantum-field-theory.md#ising-chain-nambu-spinor) by an angle with $\cos\theta=(g-\cos k)/r_k$, $\sin\theta=-\sin k/r_k$ and $r_k=\sqrt{1+g^2-2g\cos k}$. Opposite angles at $k,-k$ preserve the [canonical anticommutation relations](supersymmetric-quantum-mechanics.md#canonical-anticommutation-relations). The result is $H=\sum_k\epsilon_k(\gamma_k^\dagger\gamma_k-1/2)$. Self-paired [momenta](momentum.md) have no pairing and are handled directly as number levels. Periodic spin-chain sectors additionally constrain [fermion parity](topological-quantum-matter.md#fermion-parity) and allowed mode quantization.

##### Ising-chain ground-state energy

↑ **Parent:** [Ising-chain Bogoliubov diagonalization](#ising-chain-bogoliubov-diagonalization)

The vacuum of the diagonal [Bogoliubov quasiparticles](quantum-mechanics.md#bogoliubov-quasiparticle) has the displayed energy. In the thermodynamic bulk, $E_0/N=-J(2\pi)^{-1}\int_{-\pi}^{\pi}\sqrt{1+g^2-2g\cos k}\,dk$. The [Hellmann–Feynman theorem](quantum-mechanics.md#hellmann-feynman-theorem) then gives the field [magnetization](electromagnetism.md#magnetization) $\sum_n\langle S_n^z\rangle=\sum_kJ(g-\cos k)/\epsilon_k$. Sector-dependent finite-chain boundary terms must be restored when exact finite-size levels are needed.

###### Ising-chain field derivative and transverse polarization

↑ **Parent:** [Ising-chain ground-state energy](#ising-chain-ground-state-energy)

For a [Transverse-field Ising model](#transverse-field-ising-model) whose field term is $-2Jg\sum_nS_n^z$, the [Hellmann–Feynman theorem](quantum-mechanics.md#hellmann-feynman-theorem) gives the displayed relation. Differentiating $E_0=-J\sum_k\sqrt{1+g^2-2g\cos k}$ gives $\sum_n\langle S_n^z\rangle=\sum_k(g-\cos k)/(2\sqrt{1+g^2-2g\cos k})$. This is polarization along the imposed field, not spontaneous order along the exchange axis. In the thermodynamic limit it is zero per site at g=0, tends to1/2 at large positive g and equals $1/\pi$ at g=1.

###### Critical transverse polarization of an Ising chain

↑ **Parent:** [Ising-chain field derivative and transverse polarization](#ising-chain-field-derivative-and-transverse-polarization)

##### Ising-chain quasiparticle dispersion

↑ **Parent:** [Ising-chain Bogoliubov diagonalization](#ising-chain-bogoliubov-diagonalization)

For nonnegative field $g$, the bulk [quasiparticle](quantum-mechanics.md#quasiparticle) gap is $2J|g-1|$. At $g=0$ the dispersion is flat, $2J$; at large $g$ it is $2Jg-2J\cos k+O(J/g)$. At $g=1$ it becomes $4J|\sin(k/2)|$, linear near the gapless point. The finite periodic spin chain has additional global excitation constraints; a single isolated domain wall is not an allowed closed-chain spin configuration.

###### Finite-ring parity qualification of an Ising quasiparticle gap

↑ **Parent:** [Ising-chain quasiparticle dispersion](#ising-chain-quasiparticle-dispersion)

A bulk [quasiparticle](quantum-mechanics.md#quasiparticle) energy is not automatically the first excitation gap of a finite periodic [spin](angular-momentum-operator.md#spin) chain. The [Jordan–Wigner transformation](angular-momentum-operator.md#jordan-wigner-transformation) fixes a boundary condition through [fermion parity](topological-quantum-matter.md#fermion-parity) and restricts occupations to that same parity. At zero transverse field an Ising domain wall costs 2J, but periodic spin configurations contain an even number of walls; the first wall-pair excitation costs 4J. An ordered finite chain also has a distinct small symmetry-sector splitting at nonzero field. The thermodynamic dispersion and these finite-system scales answer different questions.

## ↑ Ancestors (4)

1. [Statistical physics](statistical-physics.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (3)

- [Blume–Capel model](#blume-capel-model)
- [Ising model](#ising-model)
- [Spin configuration](#spin-configuration)
