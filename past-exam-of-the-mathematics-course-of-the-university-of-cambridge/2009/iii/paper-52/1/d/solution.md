<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

[Hamiltonian engineering](../../../../../../hamiltonian-engineering.md) chooses accessible interactions so that their actual or effective [Quantum Hamiltonian](../../../../../../hamiltonian-quantum-mechanics.md) produces the desired evolution. A typical model is $H_f(t)=H_0+\sum_kf_k(t)H_k$; the controls may change frequencies, amplitudes, phases or coupling strengths. Three standard model-based [open-loop control](../../../../../../open-loop-control.md) approaches illustrate different mechanisms.

In [resonant quantum control](../../../../../../resonant-quantum-control.md), select a transition with a near-resonant field. In a rotating frame, after neglecting rapidly oscillating terms in a justified regime, an effective two-level drive can be $H_{\mathrm{eff}}(t)=\Omega(t)\sigma_x/2$. When its axis is fixed,

$$
U(T)=\exp\left[-\frac{i\sigma_x}{2}\int_0^T\Omega(t)\,dt\right].
$$

The pulse area sets the rotation angle and the drive phase selects the transverse axis. A resonant pulse of area $\pi$ swaps the two level populations. This requires knowledge of transition frequencies, couplings and the validity of the selective-drive approximation.

In [adiabatic quantum control](../../../../../../adiabatic-quantum-control.md), design a slowly varying [Quantum Hamiltonian](../../../../../../hamiltonian-quantum-mechanics.md) whose desired instantaneous eigenstate connects the initial and final states. For a nondegenerate eigenstate separated by a gap, the [quantum adiabatic theorem](../../../../../../adiabatic-theorem.md) explains why sufficiently slow evolution follows that state up to a phase. The relative size of matrix elements of $\dot H$ and squared spectral gaps controls the approximation; degeneracies or rapid changes invalidate simple following. This engineers a state path rather than a prescribed resonant rotation.

In [average Hamiltonian engineering](../../../../../../average-hamiltonian-engineering.md), apply a predetermined sequence of fast pulses $P_j$ and let the system evolve for intervals $\tau_j$ in the corresponding frames. For cycle length $T_c=\sum_j\tau_j$, the leading effective generator is

$$
\overline H^{(0)}=\frac1{T_c}\sum_j\tau_j P_j^\dagger H_0P_j.
$$

Choose the sequence to cancel unwanted terms or retain desired couplings. For instance, equal intervals under $H_0=\omega\sigma_z/2$ and its $\sigma_x$ conjugate cancel the leading generator because $\sigma_x\sigma_z\sigma_x=-\sigma_z$. Noncommuting terms produce higher-order [commutator](../../../../../../commutator.md) corrections, so fast cycling, finite pulse errors and the accuracy of the model matter. All three methods determine a waveform or sequence before its execution; none automatically corrects an unknown mismatch during that run.

## ↑ Ancestors (11)

1. [D](../d.md)
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
