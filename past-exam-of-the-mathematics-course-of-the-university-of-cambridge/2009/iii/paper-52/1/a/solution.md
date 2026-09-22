<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The target specifies the desired output; the controller selects a [control input](../../../../../../control-input.md); an actuator realizes it on the system; and the sensor returns a measured output. The environment supplies additional interactions and disturbances. A simple loop is:

<a id="1/a/image-quantum-control-loop-showing-the-measurement-record-and-measurement-backaction"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-52-control-loop.png)

**[Figure 1](#1/a/image-quantum-control-loop-showing-the-measurement-record-and-measurement-backaction). Quantum control loop, showing the measurement record and measurement backaction**.

For a quantum sensor, a [measurement in quantum mechanics](../../../../../../quantum-measurement-split.md) has statistical outcomes and generally changes the state through [measurement backaction](../../../../../../measurement-backaction.md). For example, outcome $m$ of an instrument with operator $K_m$ has [probability](../../../../../../probability.md) and conditional state

$$
p_m=\operatorname{Tr}(K_m\rho K_m^\dagger),\qquad
\rho_m=\frac{K_m\rho K_m^\dagger}{p_m}.
$$

A single unknown [quantum state](../../../../../../quantum-state.md) cannot generally supply its complete instantaneous state vector to a controller. Noncommuting [observables](../../../../../../observable.md) cannot be read simultaneously with arbitrary precision, and reliable [quantum state tomography](../../../../../../quantum-state-tomography.md) normally needs many reproducible preparations. A conditional state estimate can instead be updated from a continuous record, with its disturbance included in the model.

Quantum actuators change a [Quantum Hamiltonian](../../../../../../hamiltonian-quantum-mechanics.md) through applied electromagnetic fields, tunable interactions or couplings to auxiliary systems. A closed-system actuator implements [unitary operators](../../../../../../unitary-operator.md), so it preserves the [spectrum](../../../../../../spectrum-functional-analysis.md) and [purity of a density operator](../../../../../../purity-of-a-density-operator.md); it cannot arbitrarily overwrite a state as a classical assignment operation could. Dissipative actuators or [measurement in quantum measurements](../../../../../../quantum-measurement-split.md) can change these invariants, but their dynamics must be accounted for.

The environment can entangle with the system, causing [decoherence](../../../../../../quantum-decoherence.md) and dissipation when unobserved degrees of freedom are traced out. It is consequently part of the dynamical model, rather than just an additive classical disturbance. Conversely, [Markovian reservoir engineering](../../../../../../markovian-reservoir-engineering.md) uses such coupling constructively to prepare and stabilize states.

In [open-loop control](../../../../../../open-loop-control.md) the applied waveform is prescribed without using measurements from the current evolution. In [closed-loop control](../../../../../../closed-loop-control.md) it depends on the available measurement record or inferred state. [Measurement-based quantum feedback](../../../../../../measurement-based-quantum-feedback.md) is one realization of the latter; experimental adaptation across repeated preparations is another. The measurement record is classical information, but its production has quantum backaction.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 52](../../../paper-52-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
