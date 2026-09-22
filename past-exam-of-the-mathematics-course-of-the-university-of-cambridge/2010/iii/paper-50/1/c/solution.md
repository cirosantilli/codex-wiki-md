<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Lyapunov quantum control](../../../../../../lyapunov-quantum-control.md) law requires an exact instantaneous expectation value. Cyclicity writes it as

$$
f(t)=\operatorname{Tr}\bigl(\rho(t)A(t)\bigr),\qquad A(t)=i[H_1,\rho_d(t)],
$$

where $A(t)$ is a known Hermitian [observable](../../../../../../observable.md). A measurement on one system produces a random outcome, not its exact ensemble expectation, and changes the system state. Repeated measurements for state estimation or continuous weak measurements introduce noise and backaction absent from the assumed closed-system equation. Thus **the law cannot be implemented unchanged as exact measurement-based quantum feedback while retaining the dynamics and guarantee in part (a)**. A conditional-state feedback scheme must include the measurement evolution and rederive its stability properties.

If the initial [density operator](../../../../../../density-matrix.md) and Hamiltonian model are known, we can instead solve the deterministic equations in a computer, calculate $f(t)$ along the simulated trajectory, and apply that precomputed waveform in the laboratory as [open-loop control](../../../../../../open-loop-control.md). Ensemble measurements can help calibrate such a waveform, but they do not supply nondisturbing instantaneous feedback from an individual evolving system.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
