<h1 id="section-c/c10/solution">Solution</h1>

↑ **Parent:** [C10](../c10.md)

A [density operator](../../../../../density-matrix-split.md) describes both a [quantum state](../../../../../quantum-state.md) prepared in one [pure state](../../../../../pure-state.md) and a statistical preparation whose members occupy different [pure states](../../../../../pure-state.md). If normalized vectors $|\psi_i\rangle$ occur with [probabilities](../../../../../probability.md) $p_i$, define

$$
\rho=\sum_i p_i|\psi_i\rangle\langle\psi_i|,\qquad
p_i\geq0,\quad\sum_i p_i=1.
$$

The resulting operator is [Hermitian](../../../../../hermitian-operator.md), [positive semidefinite](../../../../../positive-semidefinite-matrix.md) and has [trace](../../../../../matrix-trace.md) one. Positivity follows because $\langle v|\rho|v\rangle=\sum_i p_i|\langle\psi_i|v\rangle|^2\geq0$. Conversely, the [spectral theorem](../../../../../spectral-theorem.md) gives such a representation of any finite-dimensional operator with these properties, using its [eigenvectors](../../../../../eigenvector.md) and [eigenvalues](../../../../../eigenvalue.md). The [matrix](../../../../../matrix.md) representing $\rho$ depends on the chosen [basis](../../../../../basis.md); the operator and its predictions do not.

**One operator gives every measurement [probability](../../../../../probability.md).** For a [projective measurement](../../../../../projective-measurement.md) with [orthogonal projections](../../../../../orthogonal-projection.md) $\Pi_a$ and outcomes $a$,

$$
P(a)=\operatorname{Tr}(\rho\Pi_a),\qquad
\langle A\rangle=\operatorname{Tr}(\rho A),\qquad
(\Delta A)^2=\operatorname{Tr}(\rho A^2)-\langle A\rangle^2.
$$

For example, the first formula follows by averaging $\langle\psi_i|\Pi_a|\psi_i\rangle$ over the preparation. The [trace](../../../../../matrix-trace.md) expression is [basis](../../../../../basis.md) independent. A general measurement replaces $\Pi_a$ by positive measurement effects that sum to the identity, without changing the [probability](../../../../../probability.md) formula. Thus $\rho$ specifies the statistics accessible to measurements on that system.

The distinction between pure and [mixed states](../../../../../mixed-state.md) is especially transparent in the [eigenvalues](../../../../../eigenvalue.md). A [pure state](../../../../../pure-state.md) has $\rho=|\psi\rangle\langle\psi|$, $\rho^2=\rho$, and $\operatorname{Tr}\rho^2=1$. A [mixed state](../../../../../mixed-state.md) has at least two positive [eigenvalues](../../../../../eigenvalue.md) and $\operatorname{Tr}\rho^2<1$. For a [qubit](../../../../../qubit.md),

$$
\rho=\tfrac12(I+\mathbf r\cdot\boldsymbol\sigma),\qquad
|\mathbf r|\leq1,\qquad
\operatorname{Tr}\rho^2=\tfrac12(1+|\mathbf r|^2).
$$

[pure states](../../../../../pure-state.md) lie on the [Bloch sphere](../../../../../bloch-sphere.md); [mixed states](../../../../../mixed-state.md) lie inside the [Bloch ball](../../../../../bloch-ball.md). The maximally mixed [qubit](../../../../../qubit.md) $\rho=I/2$ can be prepared by choosing equally between the two $z$ spin [eigenstates](../../../../../eigenstate.md), or equally between the two $x$ spin [eigenstates](../../../../../eigenstate.md). These ensembles are different preparation procedures but give the same [density operator](../../../../../density-matrix-split.md). No measurement on the resulting [qubit](../../../../../qubit.md) alone can identify which ensemble was used.

[quantum coherence](../../../../../quantum-coherence-in-a-specified-basis.md) must be distinguished from merely having two populated levels. In the $z$ [basis](../../../../../basis.md), the state $|+x\rangle$ has

$$
\rho_{+x}=\frac12\begin{pmatrix}1&1\\1&1\end{pmatrix},
\qquad
\rho_{\rm mix}=\frac12\begin{pmatrix}1&0\\0&1\end{pmatrix}.
$$

Both give equal [probabilities](../../../../../probability.md) for the two $z$ outcomes. A measurement along $x$ gives the positive result with [probability](../../../../../probability.md) one for the first state and one half for the second. The off-diagonal entries encode the relative phase information responsible for this difference. Whether a [matrix](../../../../../matrix.md) entry is off diagonal is [basis](../../../../../basis.md) dependent; [purity](../../../../../purity-of-a-density-operator.md) is not.

For an isolated system, each component evolves with the same unitary time-evolution operator. Therefore $\rho(t)=U(t)\rho(0)U^\dagger(t)$ and

$$
\boxed{i\hbar\dot\rho=[H,\rho]}.
$$

Unitary evolution preserves the [eigenvalues](../../../../../eigenvalue.md) and [purity](../../../../../purity-of-a-density-operator.md) of $\rho$. A [density operator](../../../../../density-matrix-split.md) commuting with a time-independent [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md) is stationary. A [thermal equilibrium](../../../../../thermal-equilibrium-split.md) example is the [canonical ensemble](../../../../../canonical-ensemble-split.md) $\rho_\beta=e^{-\beta H}/Z$, where $Z=\operatorname{Tr}(e^{-\beta H})$ and $\beta=1/(k_{\rm B}T)$. [expectation values](../../../../../expectation-value.md) then reproduce quantum [statistical mechanics](../../../../../statistical-mechanics.md) without assigning the system a definite [energy eigenstate](../../../../../energy-eigenstate.md) on every run.

A [mixed state](../../../../../mixed-state.md) can also arise without classical randomness in the joint preparation. For a [bipartite quantum system](../../../../../bipartite-quantum-system.md), the [reduced density operator](../../../../../reduced-density-matrix.md) $\rho_A=\operatorname{Tr}_B\rho_{AB}$ gives every measurement [probability](../../../../../probability.md) accessible to subsystem $A$. For the [Bell state](../../../../../bell-state-split.md) $(|00\rangle+|11\rangle)/\sqrt2$, the joint state is pure, whereas $\rho_A=I/2$. Its local mixedness reflects [entanglement](../../../../../entangled-state.md) with the inaccessible system; the [partial trace](../../../../../partial-trace.md) discards [correlations](../../../../../pearson-correlation-coefficient.md) that matter for joint measurements. More generally, interaction with an environment can suppress off-diagonal entries in a selected [basis](../../../../../basis.md), producing [decoherence](../../../../../quantum-decoherence.md) while the combined system still evolves unitarily.

Finally, state evolution conditional on a measurement outcome differs from isolated evolution. An ideal [projective measurement](../../../../../projective-measurement.md) yielding $a$ updates the state by the [Lüders rule](../../../../../luders-rule.md) $\rho\mapsto\Pi_a\rho\Pi_a/P(a)$. Discarding the outcome gives $\sum_a\Pi_a\rho\Pi_a$, which generally removes coherence between different [eigenspaces](../../../../../eigenspace.md). The [Von Neumann entropy](../../../../../von-neumann-entropy-split.md) $-\operatorname{Tr}(\rho\ln\rho)$ quantifies mixedness: it vanishes for [pure states](../../../../../pure-state.md) and reaches $\ln d$ for $I/d$. Multiplying by $k_{\rm B}$ gives thermodynamic [entropy](../../../../../entropy-split.md) units. These uses make the [density operator](../../../../../density-matrix-split.md) a common language for preparation uncertainty, measurement, thermal states and entangled subsystems, while retaining their distinct physical origins.

## ↑ Ancestors (14)

1. [C10](../c10.md)
2. [Section C](../../section-c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
