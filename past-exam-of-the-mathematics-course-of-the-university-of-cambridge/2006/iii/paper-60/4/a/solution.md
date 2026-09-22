<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The terminal term $\mathcal A$ is the objective reward. With the [Hilbert-Schmidt inner product](../../../../../../hilbert-schmidt-inner-product.md) $\langle\!\langle A|\rho\rangle\!\rangle=\operatorname{Tr}(A^\dagger\rho)$, a Hermitian target observable gives its final [expected value](../../../../../../expected-value.md). The vector $\rho_v$ is the [density operator](../../../../../../density-matrix.md) represented as a vector in operator space; it retains the same physical content as the [density matrix](../../../../../../density-matrix.md), not a wavefunction of the system.

The term $\mathcal D$ imposes the dynamical equation by a time-dependent [costate](../../../../../../costate.md) $A_v$. It is a Lagrange-multiplier operator in the same operator space, propagated backward from a terminal condition. It is not required to be a positive, trace-one [density matrix](../../../../../../density-matrix.md). Define

$$
K[f]= -\frac i\hbar\mathcal L_{\rm tot}[f].
$$

Then the enforced state equation is $\dot\rho_v=K[f]\rho_v$. The uncontrolled coherent part is $\mathcal L_0$, the dissipative contribution is $\mathcal L_D$, and each $f_m\mathcal L_m$ describes a control coupling. For [Quantum Hamiltonian](../../../../../../hamiltonian-quantum-mechanics.md) control, $\mathcal L_m\rho=[H_m,\rho]$.

The term $\mathcal C$ is a quadratic field-energy or fluence penalty. For the positive scale $p_0$ and positive weights $\lambda_m$, larger $\lambda_m$ make a given control amplitude more costly. Thus **maximizing $J$ trades terminal performance against control fluence while enforcing the dynamics**. The multiplier term vanishes on any dynamically feasible trajectory. The weights do not represent [decoherence](../../../../../../quantum-decoherence.md) rates; they specify control-resource preferences.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
