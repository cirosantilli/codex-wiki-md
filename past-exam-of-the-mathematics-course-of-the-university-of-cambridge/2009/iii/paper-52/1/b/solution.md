<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Three standard objectives are state preparation, [observable](../../../../../../observable.md) optimization and process implementation. All optimizations are over admissible [control inputs](../../../../../../control-input.md) and a specified final time $T$.

For state preparation, steer an initial [density operator](../../../../../../density-matrix.md) to a target $\rho_d$. An exact goal is $\rho_f(T)=\rho_d$, or one may minimize the squared [Hilbert-Schmidt distance](../../../../../../hilbert-schmidt-distance.md)

$$
\boxed{J_{\mathrm{state}}(f)=\tfrac12\operatorname{Tr}[(\rho_f(T)-\rho_d)^2].}
$$

For a pure target $\rho_d=|\psi_d\rangle\langle\psi_d|$, maximizing $\langle\psi_d|\rho_f(T)|\psi_d\rangle$ is a useful alternative. The target must be physically attainable: [Hamiltonian engineering](../../../../../../hamiltonian-engineering.md) alone preserves the initial [spectrum](../../../../../../spectrum-functional-analysis.md) of the [density operator](../../../../../../density-matrix.md).

For an [observable](../../../../../../observable.md) objective, choose a [Hermitian operator](../../../../../../hermitian-operator.md) $O$ and maximize its expected final value:

$$
\boxed{J_O(f)=\operatorname{Tr}[O\rho_f(T)]\quad\text{to be maximized}.}
$$

Population transfer is a special case with $O$ the projector onto the desired level or subspace; suppressing an unwanted population reverses the sign or minimizes this quantity.

For coherent process engineering, implement a target [unitary operator](../../../../../../unitary-operator.md) $V$ on every input, rather than merely arranging one state transfer. If the propagator is $U_f(T)$, a phase-insensitive error is

$$
\boxed{J_{\mathrm{gate}}(f)=1-\frac{|\operatorname{Tr}[V^\dagger U_f(T)]|^2}{N^2}.}
$$

The error vanishes precisely when $U_f(T)=e^{i\phi}V$: equality in the [Hilbert-Schmidt inner product](../../../../../../hilbert-schmidt-inner-product.md) [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) bound makes the two operators proportional. For an open-system process, the analogous objective compares the implemented [quantum channel](../../../../../../quantum-channel.md) with the target channel. These objectives can be supplemented by pulse-energy, amplitude, bandwidth and duration constraints in [quantum optimal control](../../../../../../quantum-optimal-control.md).

## ↑ Ancestors (11)

1. [B](../b.md)
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
