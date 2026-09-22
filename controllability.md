# Controllability

↑ **Parent:** [Control theory](control-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Controllability)

[Controllability](controllability.md) asks whether the available [control inputs](control-input.md) can move a [dynamical system](dynamical-system.md) between every pair of states in its declared [state space](state-space.md). Fixing a duration $T>0$ gives the precise condition $\mathcal R_T(x_0)=X$ for every $x_0\in X$, where $X$ is the [state space](state-space.md) and $\mathcal R_T(x_0)$ its [reachable set](reachable-set.md). With freely chosen duration, every pair must instead be connectable in some permitted finite time, which may depend on the pair. Always specify admissible [control inputs](control-input.md), deadlines and any constraints along the path. [Åström and Murray, Feedback Systems: State Feedback, reachability definitions](https://fbswiki.org/wiki/index.php/State_Feedback)

The surprising part is that one [control input](control-input.md) can control several state variables by acting at different times. For the [double integrator](double-integrator.md), [acceleration](acceleration.md) changes [velocity](velocity.md) directly, while the accumulated [velocity](velocity.md) changes [position](position.md). Starting from rest, accelerate during the first half of the journey and brake during the second: the final [velocity](velocity.md) can vanish although the final [position](position.md) has changed. The figure is an analytic mathematical example in [dimensionless quantities](dimensionless-quantity.md), with no experimental measurements.

<a id="image-timing-one-control-input-controls-both-position-and-velocity"></a>
![](controllability-pulse-span.png)

**[Figure 2](#image-timing-one-control-input-controls-both-position-and-velocity). Timing one control input controls both position and velocity**. The [double integrator](double-integrator.md) starts at $(p,v)=(0,0)$ and runs to $T=2$. Left: $u=1$ for one time unit, then $u=-1$ for one time unit. Middle: the analytic state path ends at $(1,0)$, after reaching $(1/2,1)$ when braking begins. Right: unit inputs on the first and second halves separately contribute $(3/2,1)$ and $(1/2,1)$ to the endpoint. Their [linear combinations](linear-combination.md) fill the plane when input amplitudes are unrestricted [real numbers](real-number.md); subtracting the second contribution from the first gives $(1,0)$.

[Controllability](controllability.md) is useful before trying to design a [controller](controller-control-theory.md): a requested endpoint outside the [reachable set](reachable-set.md) cannot be attained by clever choice of [feedback control](closed-loop-control.md). The [Kalman rank criterion](kalman-rank-criterion.md) makes this an exact [linear algebra](linear-algebra-split.md) calculation for the stated [linear time-invariant system](linear-time-invariant-system.md) model. It concerns whole states, so attaining one [plant output](output-control-theory.md) is not enough to establish [controllability](controllability.md). In [quantum control](quantum-control.md), the declared [state space](state-space.md) may be an orbit constrained by conservation laws; see [quantum controllability](quantum-controllability.md) and [unitary orbit of a density operator](unitary-orbit-of-a-density-operator.md).

**Table of contents**

- [Controllability matrix](controllability-matrix.md)
- [Kalman rank criterion](kalman-rank-criterion.md)
- [Controllability Gramian](controllability-gramian.md)
- [Quantum controllability](quantum-controllability.md)
  - [Bilinear Hamiltonian control system](bilinear-hamiltonian-control-system.md)
  - [Dynamical Lie algebra](dynamical-lie-algebra.md)
    - [Connected nondegenerate transition chain generates special unitary control](connected-nondegenerate-transition-chain-generates-special-unitary-control.md)
    - [Strongly regular quantum Hamiltonian](strongly-regular-quantum-hamiltonian.md)
    - [Codimension-one quantum dynamical algebra is special unitary](codimension-one-quantum-dynamical-algebra-is-special-unitary.md)
    - [Symplectic dynamical symmetry in quantum control](symplectic-dynamical-symmetry-in-quantum-control.md)
      - [Symplectic invariant of a density operator](symplectic-invariant-of-a-density-operator.md)
    - [Two adjacent transitions generate the qutrit unitary Lie algebra](two-adjacent-transitions-generate-the-qutrit-unitary-lie-algebra.md)
    - [Orthogonal dynamical symmetry in quantum control](orthogonal-dynamical-symmetry-in-quantum-control.md)
    - [Identity augmentation in quantum controllability](identity-augmentation-in-quantum-controllability.md)
  - [Pure-state controllability](pure-state-controllability.md)
  - [Density operator controllability](density-operator-controllability.md)
  - [Unitary operator controllability](unitary-operator-controllability.md)

## ↑ Ancestors (4)

1. [Control theory](control-theory-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (11)

- [Controllability](controllability.md)
- [Controllability Gramian](controllability-gramian.md)
- [Double integrator](double-integrator.md)
- [Kalman rank criterion](kalman-rank-criterion.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-60/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-61/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-61/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-61/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-52/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-50/3/a/solution.md)
- [Reachability in control theory](reachability-in-control-theory.md)
