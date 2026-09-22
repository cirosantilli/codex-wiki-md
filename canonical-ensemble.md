# Canonical ensemble

↑ **Parent:** [Statistical physics](statistical-physics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Canonical_ensemble)

The [canonical ensemble](canonical-ensemble.md) is the [probability distribution](probability-distribution.md) for a system in [thermal equilibrium](thermal-equilibrium.md) with a [heat bath](thermal-equilibrium.md#heat-bath) at fixed [temperature](temperature.md) $T$, with fixed particle number and external parameters. It allows [energy](energy.md) exchange, so individual [energy](energy.md) measurements fluctuate. With [Boltzmann constant](thermodynamics.md#boltzmann-constant) $k_B$ and [inverse temperature](temperature.md#inverse-temperature) $\beta=1/(k_BT)$,

$$
p_s=\frac{e^{-\beta E_s}}{Z},\qquad Z=\sum_s e^{-\beta E_s}.
$$

The [heat bath](thermal-equilibrium.md#heat-bath) is idealized as large enough that exchanges barely change its [temperature](temperature.md); coupling must permit equilibration while contributing negligible interaction [energy](energy.md). A finite [heat bath](thermal-equilibrium.md#heat-bath) approximates this description only when its [temperature](temperature.md) change is negligible over the relevant exchanges. Strong coupling or a small [heat bath](thermal-equilibrium.md#heat-bath) can require a different description.

For one [two-level system](#two-level-system) at positive [temperature](temperature.md), the [Boltzmann weights](#boltzmann-factor) are $1,e^{-\beta\Delta}$, hence

$$
Z_1=1+e^{-\beta\Delta},\qquad p=\frac{e^{-\beta\Delta}}{Z_1}=\frac1{1+e^{\beta\Delta}}.
$$

At $\beta\Delta=\ln3$, $Z_1=4/3$ and $p=1/4$. This is a probabilistic thermal [mixed state](density-matrix.md#mixed-state). For quantum levels, its [density matrix](density-matrix.md) is $\rho=(1-p)|0\rangle\langle0|+p|1\rangle\langle1|$. The [pure state](quantum-theory.md#pure-state) $\sqrt{1-p}|0\rangle+\sqrt p|1\rangle$ has the same [energy measurement](wave-function.md#energy-measurement) [probabilities](probability-theory.md#probability), but also has [quantum coherence](density-matrix.md#quantum-coherence-in-a-specified-basis) between the [energy eigenstates](energy-eigenvalue.md#energy-eigenstate). Matching those [probabilities](probability-theory.md#probability) does not make the states equivalent.

**Table of contents**

- [Translational and two-level energy variance](#translational-and-two-level-energy-variance)
- [Canonical entropy formula](#canonical-entropy-formula)
- [Canonical energy variance](#canonical-energy-variance)
- [Quantum Gibbs state](#quantum-gibbs-state)
- [Noninteracting subsystems](#noninteracting-subsystems)
- [Two-level system](#two-level-system)
  - [Equal-degeneracy two-level energy and heat capacity](#equal-degeneracy-two-level-energy-and-heat-capacity)
  - [Binomial entropy of independent two-level particles](#binomial-entropy-of-independent-two-level-particles)
  - [Additive-volume two-level system](#additive-volume-two-level-system)
  - [Saturation parameter](#saturation-parameter)
    - [Saturation intensity](#saturation-intensity)
- [Canonical partition function](#canonical-partition-function)
  - [Gibbs paradox](#gibbs-paradox)
  - [Molecular partition function](#molecular-partition-function)
    - [Energy reference in molecular partition functions](#energy-reference-in-molecular-partition-functions)
    - [Molecular partition function density](#molecular-partition-function-density)
  - [Electronic partition function](#electronic-partition-function)
  - [Vibrational partition function](#vibrational-partition-function)
    - [Vibrational entropy](#vibrational-entropy)
  - [Rotational partition function](#rotational-partition-function)
    - [Rotational entropy](#rotational-entropy)
  - [Translational partition function](#translational-partition-function)
  - [Thermal trace](#thermal-trace)
    - [Parity-twisted oscillator thermal trace](#parity-twisted-oscillator-thermal-trace)
  - [Thermodynamic derivatives of the canonical partition function](#thermodynamic-derivatives-of-the-canonical-partition-function)
    - [Canonical energy fluctuation](#canonical-energy-fluctuation)
      - [Relative energy fluctuation of a monatomic ideal gas](#relative-energy-fluctuation-of-a-monatomic-ideal-gas)
  - [Particle in a finite two-dimensional harmonic trap](#particle-in-a-finite-two-dimensional-harmonic-trap)
    - [Hard-wall correction to harmonic equipartition](#hard-wall-correction-to-harmonic-equipartition)
  - [Classical ideal-gas partition function](#classical-ideal-gas-partition-function)
    - [Classical ideal gas in a spherical linear trap](#classical-ideal-gas-in-a-spherical-linear-trap)
      - [Quantum degeneracy threshold in a spherical linear trap](#quantum-degeneracy-threshold-in-a-spherical-linear-trap)
      - [Isentropic decompression of a spherical linear trap](#isentropic-decompression-of-a-spherical-linear-trap)
    - [Classical ideal gas in a homogeneous soft trap](#classical-ideal-gas-in-a-homogeneous-soft-trap)
    - [Thermal de Broglie wavelength](#thermal-de-broglie-wavelength)
      - [Degeneracy onset from thermal wavelength](#degeneracy-onset-from-thermal-wavelength)
      - [Quantum concentration](#quantum-concentration)
    - [Canonical partition function for an ultrarelativistic gas in a power-law trap](#canonical-partition-function-for-an-ultrarelativistic-gas-in-a-power-law-trap)
      - [Most likely radius in an isotropic power-law trap](#most-likely-radius-in-an-isotropic-power-law-trap)
    - [Sackur-Tetrode equation](#sackur-tetrode-equation)
- [Independent spin-one-half two-level system](#independent-spin-one-half-two-level-system)
- [Spin-1 paramagnet](#spin-1-paramagnet)
  - [Independent symmetric three-level system](#independent-symmetric-three-level-system)
    - [Magnetic moment from a Schottky heat-capacity tail](#magnetic-moment-from-a-schottky-heat-capacity-tail)
- [Negative temperature](#negative-temperature)
  - [Magnetic-field reversal and negative temperature](#magnetic-field-reversal-and-negative-temperature)
  - [Heat flow from negative to positive temperature](#heat-flow-from-negative-to-positive-temperature)
- [Equipartition theorem](#equipartition-theorem)
  - [Rotational equipartition in a rough-ball gas](#rotational-equipartition-in-a-rough-ball-gas)
    - [Effective mechanical temperature of released rough balls](#effective-mechanical-temperature-of-released-rough-balls)
  - [Equipartition for a homogeneous potential](#equipartition-for-a-homogeneous-potential)
- [Nonrelativistic equilibrium number density](#nonrelativistic-equilibrium-number-density)
- [Boltzmann factor](#boltzmann-factor)

## Translational and two-level energy variance

↑ **Parent:** [Canonical ensemble](canonical-ensemble.md)

For a dilute classical [ideal gas](ideal-gas.md) whose atoms carry independent nondegenerate internal levels $0,\epsilon$, the [canonical partition function](#canonical-partition-function) factorizes into translation and $(1+e^{-\beta\epsilon})^N$. The upper-level [probability](probability-theory.md#probability) is $p=(1+e^{\beta\epsilon})^{-1}$. Taking two derivatives of its logarithm gives the title sum of independent [variances](variance.md). The internal contribution freezes exponentially at low [temperature](temperature.md) and tends to $N\epsilon^2/4$ at high [temperature](temperature.md). The translational classical result cannot be continued through [quantum degeneracy](quantum-mechanics.md#degenerate-energy-levels) without changing the model.

## Canonical entropy formula

↑ **Parent:** [Canonical ensemble](canonical-ensemble.md)

For $Z=\sum_i e^{-\beta E_i}$ and $U=\langle E\rangle$, the [entropy](entropy.md) is $S=k_B\ln Z+U/T$. It follows directly by substituting canonical probabilities into $S=-k_B\sum_i p_i\ln p_i$.

## Canonical energy variance

↑ **Parent:** [Canonical ensemble](canonical-ensemble.md)

Differentiating the [canonical partition function](#canonical-partition-function) at fixed external parameters gives $\langle E\rangle=-\partial_\beta\ln Z$ and $\partial_\beta^2\ln Z=\langle E^2\rangle-\langle E\rangle^2$. Consequently the [heat capacity](heat.md#heat-capacity) is

$$
C_V=\frac{\operatorname{Var}(E)}{k_{\rm B}T^2}\ge0.
$$

The identity assumes an [energy](energy.md) spectrum independent of [temperature](temperature.md) and the appropriate fixed-volume [canonical ensemble](canonical-ensemble.md). It relates a thermal response to equilibrium [variance](variance.md).

## Quantum Gibbs state

↑ **Parent:** [Canonical ensemble](canonical-ensemble.md)

A [quantum Gibbs state](#quantum-gibbs-state) is the [density operator](density-matrix.md) of a [canonical ensemble](canonical-ensemble.md) with inverse [temperature](temperature.md) $\beta=1/(k_BT)$. It exists when the [canonical partition function](#canonical-partition-function) $Z=\operatorname{Tr}(e^{-\beta H})$ is finite. The [spectral theorem](hilbert-space.md#spectral-theorem) assigns [probabilities](probability-theory.md#probability) $e^{-\beta E_j}/Z$ to an [orthonormal eigenbasis](linear-operator-theory.md#orthonormal-eigenbasis) of the [Hamiltonian](hamiltonian-mechanics.md#hamiltonian). An additive constant in the [Hamiltonian](hamiltonian-mechanics.md#hamiltonian) cancels between numerator and denominator. For $H=-\mu B\sigma_z$, the [exponential of a Pauli vector](algebra.md#exponential-of-a-pauli-vector), continued to an imaginary argument, gives $\rho_\beta=[I+\tanh(\beta\mu B)\sigma_z]/2$.

## Noninteracting subsystems

↑ **Parent:** [Canonical ensemble](canonical-ensemble.md)

Two independently available parts of a [thermodynamic system](thermodynamics.md#thermodynamic-system) are noninteracting in the canonical description when their [state space](dynamical-systems.md#state-space) is a [Cartesian product](set-theory.md#cartesian-product) and their [energy](energy.md) is additive, $E(a,b)=E_A(a)+E_B(b)$. Both conditions are needed for the [canonical partition function](#canonical-partition-function) to factor:

$$
Z=\sum_{a,b}e^{-\beta[E_A(a)+E_B(b)]}
=\left(\sum_a e^{-\beta E_A(a)}\right)\left(\sum_b e^{-\beta E_B(b)}\right)=Z_AZ_B.
$$

An additive expression on a constrained set of allowed state pairs need not give this factorization. Relabeling the states to make their allowed labels independent can instead introduce an interaction into the [energy](energy.md). For two two-state labels, an additive [energy](energy.md) necessarily satisfies the rectangular identity $E_{11}+E_{22}=E_{12}+E_{21}$.

## Two-level system

↑ **Parent:** [Canonical ensemble](canonical-ensemble.md)

### Equal-degeneracy two-level energy and heat capacity

↑ **Parent:** [Two-level system](#two-level-system)

For N [independent](random-variable.md#independent-random-variables) units with nondegenerate levels 0 and $\Delta>0$, the [canonical partition function](#canonical-partition-function) is $(1+e^{-\beta\Delta})^N$. Its [energy](energy.md) is $N\Delta/(1+e^{\beta\Delta})$ and [heat capacity](heat.md#heat-capacity) is $Nk_Bx^2e^x/(1+e^x)^2$, with $x=\Delta/(k_BT)$. Both are activated at low [temperature](temperature.md). At high [temperature](temperature.md) the [energy](energy.md) saturates at $N\Delta/2$ and [heat capacity](heat.md#heat-capacity) decays as $T^{-2}$. The equal-degeneracy Schottky peak is at $x\simeq2.39936$ and height $0.43923Nk_B$. A common [energy](energy.md) shift leaves [heat capacity](heat.md#heat-capacity) unchanged; unequal level degeneracies require a different [partition function](#canonical-partition-function).

### Binomial entropy of independent two-level particles

↑ **Parent:** [Two-level system](#two-level-system)

For independently labelled particles with nondegenerate levels, choosing which $N_+$ particles occupy the upper level gives a binomial [multiplicity](polynomial.md#multiplicity-mathematics). With $x=(N_+-N_-)/N$, its large-number [entropy](entropy.md) is $Nk_B[\ln2-(1+x)\ln(1+x)/2-(1-x)\ln(1-x)/2]$. This counting assumes distinguishable or localized degrees of freedom, not indistinguishable particles sharing one pair of quantum orbitals.

### Additive-volume two-level system

↑ **Parent:** [Two-level system](#two-level-system)

A model in which each excitation changes volume by a fixed increment $v$. If the all-ground configuration has volume $V_0$, then $V=V_0+v\langle N_{\rm ex}\rangle$. Energies and statistical weights must be specified under the relevant mechanical constraint; volume endpoints alone do not define arbitrary intermediate configurations.

### Saturation parameter

↑ **Parent:** [Two-level system](#two-level-system)

For a specified optical transition, the on-resonance [saturation parameter](#saturation-parameter) is the [light intensity](wave.md#light-intensity) divided by the [saturation intensity](#saturation-intensity). The independent-beam [Doppler cooling force](atomic-physics.md#doppler-cooling-force) model assumes weak total excitation and defines $s$ separately for each beam.

#### Saturation intensity

↑ **Parent:** [Saturation parameter](#saturation-parameter)

The [saturation intensity](#saturation-intensity) is the characteristic [light intensity](wave.md#light-intensity) used to normalize the on-resonance [saturation parameter](#saturation-parameter) of a specified optical transition. Its value depends on the transition and the stated illumination convention.

## Canonical partition function

↑ **Parent:** [Canonical ensemble](canonical-ensemble.md)

The [partition function](#canonical-partition-function) $Z(\beta)=\sum_s e^{-\beta E_s}$ is the sum of the [Boltzmann weights](#boltzmann-factor) over individual [microstates](statistical-physics.md#microstate). Dividing by it makes their [probabilities](probability-theory.md#probability) sum to one. When summing distinct [energies](energy.md) instead, include the [state degeneracy](statistical-physics.md#state-degeneracy): $Z=\sum_E g(E)e^{-\beta E}$. For two independent distinguishable [two-level systems](#two-level-system),

$$
Z_2=1+2e^{-\beta\Delta}+e^{-2\beta\Delta}=Z_1^2.
$$

The middle coefficient counts two [microstates](statistical-physics.md#microstate), exactly as in the preceding figure. For $N$ such units, $Z_N=Z_1^N$; this factorization requires additive [energy](energy.md) and [independence](random-variable.md#independent-random-variables), and generally fails with interactions.

The usefulness goes beyond normalization. For fixed [energies](energy.md), [derivatives](calculus.md#derivative) of the [natural logarithm](calculus.md#natural-logarithm) of the [partition function](#canonical-partition-function) yield measurable quantities:

$$
U=\langle E\rangle=-\partial_\beta\ln Z,\qquad
\operatorname{Var}(E)=\partial_\beta^2\ln Z,\qquad
S=k_B(\ln Z+\beta U).
$$

Here $U$ is [internal energy](internal-energy.md), the second expression is the [energy](energy.md) [variance](variance.md), and $S$ is [Gibbs entropy](statistical-physics.md#gibbs-entropy). For one [two-level system](#two-level-system) at fixed $\Delta$, its [heat capacity](heat.md#heat-capacity) $C=\partial U/\partial T$ and [entropy](entropy.md) are

$$
U=\Delta p,\qquad \frac{C}{k_B}=\frac{(\beta\Delta)^2e^{\beta\Delta}}{(1+e^{\beta\Delta})^2},\qquad
\frac{S}{k_B}=\ln(1+e^{-\beta\Delta})+\beta\Delta p.
$$

At $\beta\Delta=\ln3$, these give $U/\Delta=0.25$, $C/k_B\simeq0.2263$ and $S/k_B\simeq0.5623$. For independent units, all three quantities add.

The figure shows why [heat capacity](heat.md#heat-capacity) peaks. At low [temperature](temperature.md), the excited [energy](energy.md) is rarely occupied; at high [temperature](temperature.md), the [probabilities](probability-theory.md#probability) are almost equal and further warming barely changes [internal energy](internal-energy.md). The largest response lies between these limits, at $k_BT/\Delta\simeq0.4168$, where $C/k_B\simeq0.4392$. Meanwhile [entropy](entropy.md) rises from zero toward $k_B\ln2$, reflecting two equally likely alternatives. This high-[temperature](temperature.md) limit belongs to the stipulated [two-level system](#two-level-system); extra accessible [energy eigenstates](energy-eigenvalue.md#energy-eigenstate) would change it.

<a id="image-population-heat-capacity-and-entropy-of-one-two-level-system-as-temperature-increases"></a>
![](two-level-thermal-response.png)

**[Figure 1](#image-population-heat-capacity-and-entropy-of-one-two-level-system-as-temperature-increases). Population, heat capacity and entropy of one two-level system as temperature increases**.

### Gibbs paradox

↑ **Parent:** [Canonical partition function](#canonical-partition-function)

Counting permutations of identical classical [particles](physics.md#particle-physics) as different states produces a spurious [entropy of mixing](mixture.md#entropy-of-mixing) when otherwise identical gases are combined. The dilute [ideal gas](ideal-gas.md) [partition function](#canonical-partition-function) $Z_N=Z_1^N/N!$ removes that label multiplicity and gives an extensive [entropy](entropy.md) in the thermodynamic limit. For different species, genuinely distinct composition information still produces a [entropy of mixing](mixture.md#entropy-of-mixing). [quantum statistics](quantum-ideal-gas-statistics.md) supplies the underlying identical-particle counting.

### Molecular partition function

↑ **Parent:** [Canonical partition function](#canonical-partition-function)

The single-molecule state sum $q=\sum_s e^{-\beta E_s}$ for specified energy references and external constraints. In a dilute classical ideal gas, indistinguishability gives $Q_N=q^N/N!$; translation supplies the factor proportional to volume.

#### Energy reference in molecular partition functions

↑ **Parent:** [Molecular partition function](#molecular-partition-function)

If energies are measured upward from a species reference $\varepsilon_0$, its absolute single-particle sum is $q_{\rm abs}=e^{-\beta\varepsilon_0}q$. The ideal-gas [chemical potential](chemical-potential.md) is then $\varepsilon_0-k_BT\ln(q/N)$. A zero-point factor can be included either in $q$ or in the reference energy, but not both.

#### Molecular partition function density

↑ **Parent:** [Molecular partition function](#molecular-partition-function)

For a free molecule in a uniform ideal gas, $q_i$ is proportional to volume. The ratio $f_i=q_i/V$ is independent of the container volume at fixed temperature and has units of inverse volume.

### Electronic partition function

↑ **Parent:** [Canonical partition function](#canonical-partition-function)

The [electronic partition function](#electronic-partition-function) includes electronic excitation energies and degeneracies $g_i$. If only an exactly degenerate ground manifold of size $g$ is populated, $q_{\rm el}=g$ and its molar [entropy](entropy.md) is $R\log g$. Resolved splittings require a state sum rather than replacing all components by one degeneracy.

### Vibrational partition function

↑ **Parent:** [Canonical partition function](#canonical-partition-function)

A [vibrational partition function](#vibrational-partition-function) sums over molecular vibrational [energy levels](quantum-mechanics.md#energy-level). A single [quantum harmonic oscillator](quantum-harmonic-oscillator.md), with energies measured relative to its ground level and vibrational temperature $\theta_v=h\nu/k$, has $q_{\rm vib}=(1-e^{-\theta_v/T})^{-1}$. Retaining its absolute [zero-point energy](quantum-harmonic-oscillator.md#zero-point-energy) multiplies this by $e^{-\theta_v/(2T)}$. That factor shifts the [internal energy](internal-energy.md) but contributes no [entropy](entropy.md).

#### Vibrational entropy

↑ **Parent:** [Vibrational partition function](#vibrational-partition-function)

The harmonic-oscillator [entropy](entropy.md) contribution for one vibrational coordinate, with $x=\theta_{\rm vib}/T$. Contributions from independent [normal modes](wave-equation.md#normal-mode) add, with one term for each component of a degenerate mode. A temperature-independent [zero-point energy](quantum-harmonic-oscillator.md#zero-point-energy) does not change this [entropy](entropy.md).

### Rotational partition function

↑ **Parent:** [Canonical partition function](#canonical-partition-function)

The [rotational partition function](#rotational-partition-function) sums [Boltzmann factors](#boltzmann-factor) over rotational [energy levels](quantum-mechanics.md#energy-level), including their degeneracies and the appropriate indistinguishability convention. For a linear [rigid rotor](molecule.md#rigid-rotor) at high temperature, $q_{\rm rot}=8\pi^2IkT/(\sigma h^2)$, with [moment of inertia](rigid-body-dynamics.md#moment-of-inertia) $I$ and [rotational symmetry number](molecule.md#rotational-symmetry-number) $\sigma$.

#### Rotational entropy

↑ **Parent:** [Rotational partition function](#rotational-partition-function)

The [entropy](entropy.md) contribution from populated molecular rotational states. A nonlinear [rigid rotor](molecule.md#rigid-rotor) has $q_{\rm rot}\propto T^{3/2}$ at high [temperature](temperature.md), giving $S_{\rm rot,m}=R(\ln q_{\rm rot}+3/2)$. Its [rotational symmetry number](molecule.md#rotational-symmetry-number) removes redundant orientations.

### Translational partition function

↑ **Parent:** [Canonical partition function](#canonical-partition-function)

For a free molecule of mass $m$ in a large three-dimensional volume $V$, replacing the translational state sum by an integral gives the displayed [partition function](#canonical-partition-function). For identical classical molecules the many-molecule [canonical partition function](#canonical-partition-function) is $q_{\rm trans}^N/N!$, not simply $q_{\rm trans}^N$. Differentiating its [Helmholtz free energy](thermodynamic-potential.md#helmholtz-free-energy) at fixed volume gives the ideal-gas translational [entropy](entropy.md).

### Thermal trace

↑ **Parent:** [Canonical partition function](#canonical-partition-function)

The [trace](linear-algebra.md#matrix-trace) of imaginary-time evolution is the [canonical partition function](#canonical-partition-function) of a quantum system. In a coordinate basis it is the integral of the diagonal [Euclidean path integral](quantum-field-theory.md#euclidean-path-integral) kernel. Inserting a symmetry operator instead gives a weighted thermal [trace](linear-algebra.md#matrix-trace).

#### Parity-twisted oscillator thermal trace

↑ **Parent:** [Thermal trace](#thermal-trace)

For two equal-frequency [quantum harmonic oscillators](quantum-harmonic-oscillator.md), the ordinary [thermal trace](#thermal-trace) is $r/(1-r)^2$ and the [trace](linear-algebra.md#matrix-trace) with the [parity operator](quantum-mechanics.md#parity-operator) is $r/(1+r)^2$, where $r=e^{-\beta\omega}$. Total excitation $N$ has degeneracy $N+1$ and parity $(-1)^N$. Therefore the traces expand as $\sum_{n\ge1}(\pm1)^{n-1}nr^n$. The alternating weights come from parity insertion in a bosonic state space, not fermionic statistics.

### Thermodynamic derivatives of the canonical partition function

↑ **Parent:** [Canonical partition function](#canonical-partition-function)

Canonical differentiation gives

$$
F=-\beta^{-1}\log Z,\qquad
\langle E\rangle=-\partial_\beta\log Z,
\qquad
(\Delta E)^2=\partial_\beta^2\log Z.
$$

#### Canonical energy fluctuation

↑ **Parent:** [Thermodynamic derivatives of the canonical partition function](#thermodynamic-derivatives-of-the-canonical-partition-function)

Canonical energy variance equals $\partial_\beta^2\log Z=k_BT^2C_V$.

##### Relative energy fluctuation of a monatomic ideal gas

↑ **Parent:** [Canonical energy fluctuation](#canonical-energy-fluctuation)

At fixed [particle number](physics.md#particle-number) and [volume](geometry-and-topology.md#volume), a classical monatomic [ideal gas](ideal-gas.md) has $U=3Nk_BT/2$ and $C_V=3Nk_B/2$. The [canonical energy fluctuation](#canonical-energy-fluctuation) identity $\operatorname{Var}(E)=k_BT^2C_V$ therefore gives $\sigma_U/U=\sqrt{2/(3N)}$. Absolute fluctuations grow as $\sqrt N$, while relative fluctuations decrease as $N^{-1/2}$. A particle reservoir changes the fluctuation problem because [energy](energy.md) and particle-number fluctuations are then correlated.

### Particle in a finite two-dimensional harmonic trap

↑ **Parent:** [Canonical partition function](#canonical-partition-function)

For

$$
H=\frac{p_x^2+p_y^2}{2m}+\frac\kappa2(x^2+y^2),
\qquad x^2+y^2<R^2,
$$

put $a=\kappa R^2/2$. The normalized classical one-particle partition function is

$$
Z_1=\frac{4\pi^2m}{h^2\beta^2\kappa}
\left(1-e^{-\beta a}\right).
$$

Its mean total and potential energies are

$$
\langle E\rangle=\frac2\beta-\frac a{e^{\beta a}-1},
\qquad
\langle V\rangle=\frac1\beta-\frac a{e^{\beta a}-1}.
$$

#### Hard-wall correction to harmonic equipartition

↑ **Parent:** [Particle in a finite two-dimensional harmonic trap](#particle-in-a-finite-two-dimensional-harmonic-trap)

If $a\gg k_BT$, the wall is thermally inaccessible and $\langle E\rangle\sim2k_BT$, as four quadratic terms predict. If $a\ll k_BT$, the spatial distribution is nearly uniform in the disk and

$$
\langle E\rangle
=k_BT+\frac{\kappa R^2}{4}+O\left(\frac{\kappa^2R^4}{k_BT}\right),
$$

so only the two kinetic quadratic terms contribute at leading order.

### Classical ideal-gas partition function

↑ **Parent:** [Canonical partition function](#canonical-partition-function)

For $N$ indistinguishable noninteracting classical particles, $Z_N=z_1^N/N!$, where $z_1$ is the normalized one-particle phase-space integral.

#### Classical ideal gas in a spherical linear trap

↑ **Parent:** [Classical ideal-gas partition function](#classical-ideal-gas-partition-function)

For a structureless particle with [Hamiltonian](hamiltonian-mechanics.md#hamiltonian) $p^2/(2m)+ar$, $a>0$, the classical [phase space](hamiltonian-mechanics.md#phase-space) integral gives the displayed one-particle [partition function](#canonical-partition-function). Its spatial integral is $4\pi\int_0^\infty r^2e^{-ar/(k_BT)}dr=8\pi(k_BT/a)^3$, while the momentum integral gives $\lambda_T^{-3}$. For $N$ indistinguishable dilute particles, $Z_N=Z_1^N/N!$, $F\simeq-Nk_BT[\ln(Z_1/N)+1]$, $U=(9/2)Nk_BT$ and $S\simeq Nk_B[\ln(Z_1/N)+11/2]$. These thermodynamic formulas use leading Stirling accuracy; the classical phase-space integral additionally requires temperatures above the discrete trap level scale.

##### Quantum degeneracy threshold in a spherical linear trap

↑ **Parent:** [Classical ideal gas in a spherical linear trap](#classical-ideal-gas-in-a-spherical-linear-trap)

For a dilute classical trapped gas, $\mu\simeq k_BT\ln(N/Z_1)$ with energy zero at the potential minimum. Thus $z=e^{\mu/(k_BT)}=N/Z_1$. Quantum occupation effects begin when $z$ is no longer small, giving the displayed order-of-magnitude particle threshold. Equivalently, the central density $n(0)=N/[8\pi(k_BT/a)^3]$ satisfies $n(0)\lambda_T^3\sim1$. This is a degeneracy crossover criterion rather than an exact Bose condensation threshold. In the continuum approximation, spinless bosons have excited-state saturation $N_c=\zeta(9/2)Z_1$, from the trap density of states proportional to $E^{7/2}$. A quantum ground energy should be subtracted consistently when discreteness matters.

##### Isentropic decompression of a spherical linear trap

↑ **Parent:** [Classical ideal gas in a spherical linear trap](#classical-ideal-gas-in-a-spherical-linear-trap)

At fixed atom number, the [entropy](entropy.md) of the [classical ideal gas in a spherical linear trap](#classical-ideal-gas-in-a-spherical-linear-trap) depends on temperature and strength through $Z_1\propto T^{9/2}a^{-3}$. Reversible adiabatic change therefore holds this product constant, giving the displayed relation. Reducing trap strength lowers the temperature while increasing cloud size. Its peak classical phase-space occupation $N/Z_1$ remains constant, so this cooling alone does not make the gas more quantum degenerate. Heat exchange, particle loss or irreversible entropy production would change this relation.

#### Classical ideal gas in a homogeneous soft trap

↑ **Parent:** [Classical ideal-gas partition function](#classical-ideal-gas-partition-function)

For the potential $U=r^{2n}/V^{2n/3}$, rescaling $r=V^{1/3}(kT)^{1/(2n)}u$ in the classical one-particle [partition function](#canonical-partition-function) gives the formula above. The parameter-conjugate force is $P=NkT/V$, the [internal energy](internal-energy.md) is $(3/2+3/(2n))NkT$, and $C_P-C_V=Nk$. The kinetic term contributes $3NkT/2$, while the potential term contributes $3NkT/(2n)$. For indistinguishable particles the $N!$ [factor](statistical-modelling.md#regression-factor) changes [free energy](thermodynamic-potential.md#thermodynamic-free-energy) and [entropy](entropy.md) but not these force and heat-capacity formulas.

#### Thermal de Broglie wavelength

↑ **Parent:** [Classical ideal-gas partition function](#classical-ideal-gas-partition-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Thermal_de_Broglie_wavelength)

The three-dimensional translational momentum integral is $1/\lambda^3$ per unit volume, where

$$
\lambda=\sqrt{\frac{2\pi\hbar^2}{mk_BT}}.
$$

##### Degeneracy onset from thermal wavelength

↑ **Parent:** [Thermal de Broglie wavelength](#thermal-de-broglie-wavelength)

Equating [thermal de Broglie wavelength](#thermal-de-broglie-wavelength) $h/\sqrt{2\pi mk_BT}$ to mean particle spacing $n^{-1/3}$ gives the displayed quantum-degeneracy scale. It is an onset estimate rather than a universal phase-transition [temperature](temperature.md). Different typical-momentum conventions change its order-one factor; [density](fluid-mechanics.md#density), [mass](classical-mechanics.md#mass), spin degeneracy and interactions determine the detailed crossover or condensation criterion.

##### Quantum concentration

↑ **Parent:** [Thermal de Broglie wavelength](#thermal-de-broglie-wavelength)

The translational concentration scale for a nonrelativistic particle in three dimensions, per internal state. It is the inverse cube of the [thermal de Broglie wavelength](#thermal-de-broglie-wavelength). A classical component with number density $n$ and external one-particle energy $U$ has [chemical potential](chemical-potential.md) $\mu=k_BT\ln(n/n_Q)+U$. An additional internal degeneracy must be included explicitly; it is not hidden in this definition. The dilute classical condition is $n/n_Q\ll1$ for each occupied internal component.

#### Canonical partition function for an ultrarelativistic gas in a power-law trap

↑ **Parent:** [Classical ideal-gas partition function](#classical-ideal-gas-partition-function)

For energy $pc+U(x)$,

$$
Z_1=\frac{(k_BT)^3}{\pi^2(\hbar c)^3}
\int e^{-U(x)/(k_BT)}d^3x.
$$

If $U(r)=r^{2n}/V^{2n/3}$, then

$$
Z_1=\frac4{\pi(\hbar c)^3}
V(k_BT)^{3+3/(2n)}I_n,
\qquad
I_n=\int_0^\infty u^2e^{-u^{2n}}du.
$$

Consequently $pV=Nk_BT$, while the mean energy and variance are $NAk_BT$ and $NA(k_BT)^2$ with $A=3+3/(2n)$.

##### Most likely radius in an isotropic power-law trap

↑ **Parent:** [Canonical partition function for an ultrarelativistic gas in a power-law trap](#canonical-partition-function-for-an-ultrarelativistic-gas-in-a-power-law-trap)

The radial density is proportional to $r^2e^{-r^{2n}/(V^{2n/3}k_BT)}$, whose mode is

$$
r=V^{1/3}\left(\frac{k_BT}{n}\right)^{1/(2n)}.
$$

#### Sackur-Tetrode equation

↑ **Parent:** [Classical ideal-gas partition function](#classical-ideal-gas-partition-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sackur–Tetrode_equation)

In the classical dilute regime, a monatomic ideal gas has entropy

$$
S=Nk_B\left[\log\left(\frac{V}{N\lambda^3}\right)+\frac52\right].
$$

## Independent spin-one-half two-level system

↑ **Parent:** [Canonical ensemble](canonical-ensemble.md)

For $N$ distinguishable noninteracting spins, let a fraction $\alpha$ occupy the level $+\epsilon$ and the remainder occupy $-\epsilon$. The [Stirling formula](real-analysis.md#stirling-formula) gives

$$
S=-Nk_B\bigl[\alpha\log\alpha+(1-\alpha)\log(1-\alpha)\bigr],
\qquad
E=N\epsilon(2\alpha-1).
$$

The relation $1/T=\partial S/\partial E$ yields

$$
\alpha=\frac1{1+e^{2\epsilon/(k_BT)}},
\qquad
E=-N\epsilon\tanh\left(\frac\epsilon{k_BT}\right).
$$

Positive temperature corresponds to $0\leq\alpha<1/2$; a population inversion $1/2<\alpha\leq1$ has [negative temperature](#negative-temperature).

## Spin-1 paramagnet

↑ **Parent:** [Canonical ensemble](canonical-ensemble.md)

For $N$ independent spins with $s_z\in\{-1,0,1\}$ and one-spin Hamiltonian $-\mu Bs_z$,

$$
Z=\left(1+2\cosh(\beta\mu B)\right)^N.
$$

Writing $x=\beta\mu B$, its heat capacity is

$$
C=Nk_Bx^2\frac{2(\cosh x+2)}
{(1+2\cosh x)^2}.
$$

### Independent symmetric three-level system

↑ **Parent:** [Spin-1 paramagnet](#spin-1-paramagnet)

For $N$ noninteracting units with energies $-\epsilon,0,\epsilon$, put $x=\beta\epsilon$. Then

$$
Z=(1+2\cosh x)^N,
\qquad
E=-\frac{2N\epsilon\sinh x}{1+2\cosh x},
$$

and

$$
S=Nk_B\left[
\log(1+2\cosh x)
-\frac{2x\sinh x}{1+2\cosh x}
\right].
$$

#### Magnetic moment from a Schottky heat-capacity tail

↑ **Parent:** [Independent symmetric three-level system](#independent-symmetric-three-level-system)

For one three-level unit with energies $-\mu B,0,\mu B$, the high-temperature [heat capacity](heat.md#heat-capacity) is $C\simeq2\mu^2B^2/(3k_BT^2)$. A measured coefficient $C=a/T^2$ therefore gives the displayed magnetic moment. If the [heat capacity](heat.md#heat-capacity) instead represents $N$ independent units, replace $a$ by $a/N$; the normalization must be established before extracting a single-unit moment.

## Negative temperature

↑ **Parent:** [Canonical ensemble](canonical-ensemble.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Negative_temperature)

Negative absolute temperature can occur only for a system with an energy spectrum bounded above. Since $\beta=\partial S/\partial E<0$, higher-energy states are more populated than lower-energy states.

### Magnetic-field reversal and negative temperature

↑ **Parent:** [Negative temperature](#negative-temperature)

Instantaneously reversing a Hamiltonian $H(B)$ satisfying $H(-B)=-H(B)$ leaves populations unchanged but rewrites them as a canonical distribution with $\beta'=-\beta$. When the partition function is unchanged, the free energy changes sign and the heat capacity is unchanged.

### Heat flow from negative to positive temperature

↑ **Parent:** [Negative temperature](#negative-temperature)

A negative-temperature system is hotter than every positive-temperature system. If heat $\delta Q$ passes from it to a positive-temperature body, the total entropy change is

$$
\delta S_{\rm total}
=\delta Q(\beta_{\rm positive}-\beta_{\rm negative})>0.
$$

## Equipartition theorem

↑ **Parent:** [Canonical ensemble](canonical-ensemble.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Equipartition_theorem)

The [equipartition theorem](#equipartition-theorem) says that each independent quadratic term in a [Hamiltonian](hamiltonian-mechanics.md#hamiltonian) described by [classical mechanics](classical-mechanics.md) has mean [energy](energy.md) $k_BT/2$ in a [canonical ensemble](canonical-ensemble.md). Here $k_B$ is the [Boltzmann constant](thermodynamics.md#boltzmann-constant) and $T>0$ the absolute [temperature](temperature.md). Count terms in the [energy](energy.md), rather than vaguely counting everything that can move: one [harmonic oscillator](classical-mechanics.md#simple-harmonic-motion) has one position [degree of freedom](classical-mechanics.md#degree-of-freedom) but TWO quadratic terms, one in [momentum](momentum.md) and one in [displacement](classical-mechanics.md#displacement).

A precise sufficient setting is $H(y,\xi)=ay^2/2+H_0(\xi)$ with $a>0$, where $y$ is one of the [canonical variables](hamiltonian-mechanics.md#canonical-variables), $\xi$ denotes all remaining variables, and the [phase space](hamiltonian-mechanics.md#phase-space) integration measure factors as $dy\,d\xi$. The range of $y$ is the whole [real line](real-analysis.md#real-line), independently of $\xi$; there is no [constraint](classical-mechanics.md#constraint-mechanics) coupling its allowed values to other variables. The [partition function](#canonical-partition-function) must be finite, and the relevant [expected values](expected-value.md) must exist. The [Boltzmann factor](#boltzmann-factor) then gives

$$
\beta=\frac{1}{k_BT},\qquad
\rho_y(y)=\sqrt{\frac{\beta a}{2\pi}}e^{-\beta ay^2/2},\qquad
\left\langle\frac{ay^2}{2}\right\rangle=\frac{k_BT}{2}.
$$

The [probability density function](continuous-probability-distribution.md#probability-density-function) $\rho_y$ is a [normal distribution](probability-distribution.md#normal-distribution) with [variance](variance.md) $k_BT/a$. A larger coefficient narrows the fluctuations enough to cancel its greater [energy](energy.md) cost. This is why the mean contribution is independent of [mass](classical-mechanics.md#mass) or [spring constant](elasticity-physics.md#spring-constant).[equations 7.124–7.135](physics-bibliography.md#thermodynamics-and-statistical-mechanics-by-richard-fitzpatrick/equipartition-theorem)

For a proof outline, the one-variable [Gaussian integral](integral.md#gaussian-integral) is $Z_y=\int_{-\infty}^{\infty}e^{-\beta ay^2/2}\,dy=\sqrt{2\pi/(\beta a)}$, so $-\partial_\beta\ln Z_y=1/(2\beta)$. More generally, [integration by parts](calculus.md#integration-by-parts) in a canonical variable gives $\langle y\,\partial_yH\rangle=k_BT$ when its boundary term $[y e^{-\beta H}]$ vanishes and the integrals converge. For $ay^2/2$ this is twice its mean [energy](energy.md). At a finite hard boundary the boundary term need not vanish; [hard-wall correction to harmonic equipartition](#hard-wall-correction-to-harmonic-equipartition) illustrates the resulting departure. A [constraint](classical-mechanics.md#constraint-mechanics), a nonquadratic [potential energy](energy.md#potential-energy), or a noncanonical integration measure therefore requires its own calculation. The theorem is an [ensemble average](expected-value.md), not equality of instantaneous [energies](energy.md), and applying it to a recorded trajectory requires equilibration and sufficient sampling.

For a classical one-dimensional [harmonic oscillator](classical-mechanics.md#simple-harmonic-motion), with positive [mass](classical-mechanics.md#mass) $m$ and [spring constant](elasticity-physics.md#spring-constant) $k$,

$$
H=\frac{p^2}{2m}+\frac{kx^2}{2},\qquad
\frac{\langle p^2\rangle}{2m}=\frac{k\langle x^2\rangle}{2}=\frac{k_BT}{2},\qquad
\langle H\rangle=k_BT.
$$

The origin is the [equilibrium](dynamical-systems.md#equilibrium-point-of-a-dynamical-system) position. Its [heat capacity](heat.md#heat-capacity) is $k_B$ at fixed $m,k$, not $k_B/2$. Although the two mean [energies](energy.md) agree, their measured amplitudes do not: $\langle p^2\rangle=mk_BT$ and $\langle x^2\rangle=k_BT/k$. In a [harmonic optical trap](optics.md#harmonic-optical-trap), the position measurement observes the [potential energy](energy.md#potential-energy) contribution; it does not measure both contributions by observing $x$ alone.[equations 7.136–7.139](physics-bibliography.md#thermodynamics-and-statistical-mechanics-by-richard-fitzpatrick/harmonic-oscillators)

For $N$ particles in a three-dimensional classical [monatomic gas](ideal-gas.md#monatomic-gas), neglect interactions and thermally accessible internal excitations. Its three translational [momentum](momentum.md) terms give [internal energy](internal-energy.md) $U=3Nk_BT/2$, [heat capacity at constant volume](heat.md#heat-capacity-at-constant-volume) $C_V=3Nk_B/2$, and [heat capacity at constant pressure](enthalpy.md#heat-capacity-at-constant-pressure) $C_p=C_V+Nk_B=5Nk_B/2$. Per mole, replace $Nk_B$ by the [molar gas constant](ideal-gas.md#molar-gas-constant) $R$. For example, using stipulated $R=8.314\,\mathrm{J\,mol^{-1}\,K^{-1}}$, the [molar heat capacity](heat.md#molar-heat-capacity) at fixed [volume](thermodynamics.md#volume-thermodynamics) is $12.471\,\mathrm{J\,mol^{-1}\,K^{-1}}$. These results assume a dilute, nonrelativistic [ideal gas](ideal-gas.md) with classical translational statistics, rather than a [quantum degeneracy](quantum-mechanics.md#degenerate-energy-levels) regime.

For an [ideal gas](ideal-gas.md) of diatomic [molecules](molecule.md), modeled as two [chemical atoms](physics.md#atom-physics) with a bond, there are three translational quadratic terms, two accessible [rotational kinetic energy](energy.md#rotational-kinetic-energy) terms for changes of bond orientation, and one bond-stretching [harmonic oscillator](classical-mechanics.md#simple-harmonic-motion) with two quadratic terms. Rotation about the bond axis is not an additional active mode in this linear-molecule model. The three familiar limits of [heat capacity at constant volume](heat.md#heat-capacity-at-constant-volume) are

$$
\frac{C_V}{Nk_B}\simeq
\begin{cases}
3/2,&\text{rotations and vibrations frozen},\\
5/2,&\text{rotations active, vibrations frozen},\\
7/2,&\text{rotations and vibrations classical}.
\end{cases}
$$

Corresponding [molar heat capacities](heat.md#molar-heat-capacity) are $3R/2$, $5R/2$ and $7R/2$. Counting the stretching [harmonic oscillator](classical-mechanics.md#simple-harmonic-motion) only once as $k_BT/2$ would give the wrong last value.[§§2.2.1](physics-bibliography.md#statistical-physics-by-david-tong/2-classical-gases)

The frozen regimes require [quantum mechanics](quantum-mechanics.md). In the simple molecular rotation model, $E_j=k_B\theta_r j(j+1)$ with [state degeneracy](statistical-physics.md#state-degeneracy) $2j+1$, $\theta_r=\hbar^2/(2Ik_B)$, and [moment of inertia](rigid-body-dynamics.md#moment-of-inertia) $I$. For the bond-stretching [quantum harmonic oscillator](quantum-harmonic-oscillator.md), $\theta_v=\hbar\omega/k_B$ with [angular frequency](lagrangian-mechanics.md#angular-frequency) $\omega$ and $\hbar=h/(2\pi)$ from the [Planck constant](quantum-mechanics.md#planck-constant). When $\theta_r\ll\theta_v$, the three limits above correspond to $T\ll\theta_r$, $\theta_r\ll T\ll\theta_v$, and $T\gg\theta_v$, provided translational motion remains classical. They are smooth crossovers, not abrupt switches. Real [molecules](molecule.md) can have different allowed rotational populations; at high [temperature](temperature.md), [thermal dissociation](chemical-reaction.md#thermal-dissociation), internal excitations and nonharmonic bond motion can invalidate the fixed-molecule model before its last limit is reached.[§3.4](physics-bibliography.md#statistical-physics-by-david-tong/3-quantum-gases)

For a [quantum harmonic oscillator](quantum-harmonic-oscillator.md) with fixed $\omega$, put $z=\theta_v/T$. Its exact mean [energy](energy.md) and [heat capacity](heat.md#heat-capacity) are

$$
\langle H\rangle=\frac{\hbar\omega}{2}+\frac{\hbar\omega}{e^z-1},\qquad
\frac{C_{\rm osc}}{k_B}=\frac{z^2e^{-z}}{(1-e^{-z})^2}.
$$

At $T\gg\theta_v$, the mean [energy](energy.md) approaches $k_BT$ and $C_{\rm osc}$ approaches $k_B$. At $T\ll\theta_v$, thermal excitation is exponentially suppressed and $C_{\rm osc}$ tends to zero, although the [zero-point energy](quantum-harmonic-oscillator.md#zero-point-energy) $\hbar\omega/2$ survives. Frozen thus means little thermal response, not zero motion or zero [energy](energy.md).[equations 7.140–7.155](physics-bibliography.md#thermodynamics-and-statistical-mechanics-by-richard-fitzpatrick/harmonic-oscillators)

<a id="image-model-heat-capacities-a-quantum-harmonic-oscillator-and-a-diatomic-ideal-gas"></a>
![](equipartition-quantum-heat-capacity.png)

**[Figure 2](#image-model-heat-capacities-a-quantum-harmonic-oscillator-and-a-diatomic-ideal-gas). Model heat capacities: a quantum harmonic oscillator and a diatomic ideal gas**. Original computed equilibrium curves, not measured gas data. Left: $C_{\rm osc}/k_B$ approaches its classical value 1 as $T/\theta_v$ grows. Right: $C_V/(Nk_B)=3/2+C_{\rm rot}/k_B+C_{\rm osc}/k_B$ for stipulated $\theta_v/\theta_r=100$. The rotational [partition function](#canonical-partition-function) is $\sum_{j=0}^{\infty}(2j+1)e^{-\theta_r j(j+1)/T}$ with every nonnegative integer $j$ allowed; $C_{\rm rot}/k_B$ is the [variance](variance.md) of $j(j+1)$ divided by $(T/\theta_r)^2$. No molecular nuclear-spin restrictions, [thermal dissociation](chemical-reaction.md#thermal-dissociation) or nonharmonic effects are modeled. Horizontal guides mark the three limiting values, not exact plateaus at finite [temperature](temperature.md).

A motivating measurement is [thermal calibration of an optical trap](optics.md#thermal-calibration-of-an-optical-trap). A focused [laser](laser.md) through a microscope objective confines a bead in water; imaging or a quadrant photodetector records a position [time series](time-series.md). Gieseler and colleagues describe a polystyrene bead of radius $1.03\,\mathrm{\mu m}$ at $293.15\,\mathrm K$, a $1064\,\mathrm{nm}$ trapping [laser](laser.md), and photodetector acquisition at $10^5\,\mathrm{Hz}$. Their recorded bead continues undergoing [Brownian motion](brownian-motion.md); higher trapping power produces a narrower equilibrium position distribution. Infer the centered [variance](variance.md), not a squared distance from an arbitrary camera origin:

$$
\sigma_x^2=\left\langle(x-\langle x\rangle)^2\right\rangle,\qquad
k=\frac{k_BT}{\sigma_x^2}.
$$

The [normal distribution](probability-distribution.md#normal-distribution) position histogram and agreement with dynamical calibration methods support the local [harmonic optical trap](optics.md#harmonic-optical-trap) interpretation. For a stipulated example, $T=300\,\mathrm K$ and $\sigma_x=20\,\mathrm{nm}$ imply $k\simeq1.04\times10^{-5}\,\mathrm{N/m}=0.0104\,\mathrm{pN/nm}$. This calculated scale is not an experimental reading.[§§2.1–2.2, 3.3; Tables 1–3](physics-bibliography.md#optical-tweezers-a-comprehensive-tutorial-from-calibration-to-applications-by-jan-gieseler)

Position calibration is essential: if detector output $v$ has conversion $x=s(v-v_0)$, its physical [variance](variance.md) is $s^2\operatorname{Var}(v)$. An unknown scale $s$ cannot be determined together with $k$ from that one [variance](variance.md). A complementary calibration demonstrated by Tolić-Nørrelykke and colleagues combines the [power spectrum](probability-and-statistics.md#power-spectrum) of thermal motion with the bead response to known sinusoidal motion of a translation stage. The driven response supplies an additional length scale, and their method does not require bead size, liquid [dynamic viscosity](dynamic-viscosity.md) or wall distance as inputs. It still uses a thermal dynamical model; agreement between methods is a consistency check, not a theory-free proof of [equipartition theorem](#equipartition-theorem).[abstract](physics-bibliography.md#calibration-of-optical-tweezers-with-positional-detection-in-the-back-focal-plane-by-simon-f-tolic-norrelykke-and-others)

The readout itself can hide fluctuations. Wong and Halvorsen used a $1064\,\mathrm{nm}$ [optical trap](optics.md#optical-tweezers) and adjustable-exposure CCD imaging of a bead in water. They varied exposure and trapping power, held the bead away from the nearest wall, adjusted illumination to maintain comparable images, and measured tracking noise using a stuck bead. The measured [variance](variance.md) fell as exposure increased; corrected results agreed with their time-averaging model. For a stationary overdamped [harmonic optical trap](optics.md#harmonic-optical-trap), with [optical trap relaxation time](optics.md#optical-trap-relaxation-time) $\tau$, an exposure of length $W$ measures $\bar x_W=W^{-1}\int_0^W x(t)\,dt$. Its ideal noise-free [variance](variance.md) is

$$
\operatorname{Var}(\bar x_W)=\frac{k_BT}{k}S(\alpha),\qquad
\alpha=\frac{W}{\tau},\qquad
S(\alpha)=\frac{2(\alpha-1+e^{-\alpha})}{\alpha^2}.
$$

For $\alpha>0$, $S(\alpha)<1$: using the blurred [variance](variance.md) in the uncorrected formula overestimates $k$ by $1/S(\alpha)$. At $W=\tau$, the calculated factor is $e/2\simeq1.36$. Additive tracking noise instead raises the measured [variance](variance.md) and biases the inferred $k$ downward if left uncorrected.[equations 15](physics-bibliography.md#the-effect-of-integration-time-on-fluctuation-measurements-calibrating-an-optical-trap-in-the-presence-of-motion-blur-by-wesley-p-wong-and-others)

<a id="image-equal-mean-quadratic-energies-with-unequal-fluctuations-and-exposure-biased-readout"></a>
![](equipartition-phase-space-readout.png)

**[Figure 3](#image-equal-mean-quadratic-energies-with-unequal-fluctuations-and-exposure-biased-readout). Equal mean quadratic energies with unequal fluctuations, and exposure-biased readout**. Original analytic models, not bead trajectories or measured curves. Left: equal-[energy](energy.md) contours $H/(k_BT)=1/2,2$ in scaled [phase space](hamiltonian-mechanics.md#phase-space), with $Q=x/\sqrt{k_BT/k_0}$, $P=p/\sqrt{mk_BT}$ and $H/(k_BT)=(P^2+\kappa Q^2)/2$, for $\kappa=k/k_0=1,4$. Increasing stiffness narrows position fluctuations but leaves both mean quadratic contributions equal to $k_BT/2$. Right: the exact noise-free exposure reduction $S(W/\tau)$; at $W/\tau=1$, $S=2/e$ and naive inferred stiffness is $e/2$ times true stiffness. The exposure calculation assumes stationary overdamped harmonic [Brownian motion](brownian-motion.md) and uniform averaging.

Useful controls are to record over many [optical trap relaxation times](optics.md#optical-trap-relaxation-time), compare blocks for drift, calibrate the position scale, measure fixed-bead noise, vary exposure, and check the position histogram for departures from a [normal distribution](probability-distribution.md#normal-distribution). A sparse sequence of accurate instantaneous positions can estimate an equilibrium [variance](variance.md); a long exposure averages away motion even if many frames are collected. Flow, appreciable [laser](laser.md) heating, escape from the harmonic region or nonconservative [forces](force.md) can break the assumed [thermal equilibrium](thermal-equilibrium.md). Inferring $k$ by imposing [equipartition theorem](#equipartition-theorem) is a calibration, whereas testing the relation requires an independently established stiffness and position scale. The beautiful practical connection is that microscopic randomness can set a [force](force.md) scale: once calibrated, a small constant applied [force](force.md) displaces the mean by $f/k$. The same quadratic-term counting predicts macroscopic [heat capacity](heat.md#heat-capacity) and makes microscopic fluctuations useful measurements.

### Rotational equipartition in a rough-ball gas

↑ **Parent:** [Equipartition theorem](#equipartition-theorem)

Rough elastic collisions can exchange rotational and translational [kinetic energy](energy.md#kinetic-energy). For three-dimensional rigid balls with all three rotations thermalized, these six quadratic terms contribute $3k_BT$ per particle. A uniform gravitational height distribution adds $k_BT$, giving total mechanical mean energy $4k_BT$.

#### Effective mechanical temperature of released rough balls

↑ **Parent:** [Rotational equipartition in a rough-ball gas](#rotational-equipartition-in-a-rough-ball-gas)

If each initially stationary ball is released at height $h$ and the subsequent isolated dilute assembly reaches effective classical equilibrium, energy conservation gives $4k_BT=mgh$. The height-tail probability above the release height is then $e^{-4}$. The effective [temperature](temperature.md) refers to mechanical motion, not the material's internal [temperature](temperature.md).

### Equipartition for a homogeneous potential

↑ **Parent:** [Equipartition theorem](#equipartition-theorem)

For a classical canonical coordinate with confining [potential energy](energy.md#potential-energy) $U=A|x|^s$, $A>0$ and $s>0$, [integration by parts](calculus.md#integration-by-parts) in the [Boltzmann distribution](thermodynamics.md#boltzmann-distribution) gives $\langle xU'(x)\rangle=k_BT$. Homogeneity then gives $\langle U\rangle=k_BT/s$. The usual quadratic contribution $k_BT/2$ is the special case $s=2$.

## Nonrelativistic equilibrium number density

↑ **Parent:** [Canonical ensemble](canonical-ensemble.md)

In the dilute Maxwell--Boltzmann regime, a species has number density proportional to $g(mk_BT)^{3/2}e^{(\mu-mc^2)/(k_BT)}$.

## Boltzmann factor

↑ **Parent:** [Canonical ensemble](canonical-ensemble.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Boltzmann_factor)

At inverse temperature $\beta=1/(k_BT)$, the Boltzmann factor $e^{-\beta E}$ is the relative [canonical ensemble](canonical-ensemble.md) weight of a [microstate](statistical-physics.md#microstate) with energy $E$.

## ↑ Ancestors (4)

1. [Statistical physics](statistical-physics.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (55)

- [Boltzmann distribution](thermodynamics.md#boltzmann-distribution)
- [Boltzmann factor](#boltzmann-factor)
- [Boundary-pressure correction to the virial theorem](classical-mechanics.md#boundary-pressure-correction-to-the-virial-theorem)
- [Canonical energy variance](#canonical-energy-variance)
- [Canonical ensemble](canonical-ensemble.md)
- [Crooks fluctuation theorem](stochastic-thermodynamics.md#crooks-fluctuation-theorem)
- [Edwards-Anderson order parameter](spin-model.md#edwards-anderson-order-parameter)
- [Equipartition theorem](#equipartition-theorem)
- [Heat bath](thermal-equilibrium.md#heat-bath)
- [Helmholtz free energy](thermodynamic-potential.md#helmholtz-free-energy)
- [Independent-moment magnetic response](statistical-physics.md#independent-moment-magnetic-response)
- [Independent spin Barnett response](electromagnetism.md#independent-spin-barnett-response)
- [Inverse temperature](temperature.md#inverse-temperature)
- [Ising model](spin-model.md#ising-model)
- [Microstate](statistical-physics.md#microstate)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1.md#7/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-63.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-69.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-2.md#34e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-4.md#34d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-67.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-1.md#35d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-74.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-66.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-66.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#34d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2.md#36a/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-2.md#37c/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-311.md#4/c/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-2.md#37a/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1.md#36a/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-2.md#37a/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-1.md#36b/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-3.md#35b/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-353.md#1/b/i/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2015/paper-1.md#section-c/c10/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2011/paper-1.md#section-c/c13/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2014/paper-2.md#section-c/c12/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1.md#section-b/b3/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2004.md#section-a/2/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2004.md#section-b/b8/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2015/paper-1.md#1/a/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2015/paper-1.md#1/c/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2016/paper-1.md#2/a/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2019.md#section-b/4/solution)
- [Quantum Gibbs state](#quantum-gibbs-state)
- [Reservoir constraints of equilibrium ensembles](thermodynamics.md#reservoir-constraints-of-equilibrium-ensembles)
- [Spin overlap](spin-model.md#spin-overlap)
- [Statistical ensemble](thermodynamics.md#statistical-ensemble)
- [Statistical Hamiltonian](statistical-physics.md#statistical-hamiltonian)
- [Statistical mechanics](statistical-physics.md#statistical-mechanics)
- [Thermal covariance of an elastic filament](elasticity-physics.md#thermal-covariance-of-an-elastic-filament)
- [Thermodynamic limit](statistical-physics.md#thermodynamic-limit)
- [Two-level paramagnetic cooling model](temperature.md#two-level-paramagnetic-cooling-model)
- [Zero-energy filament mode](elasticity-physics.md#zero-energy-filament-mode)
