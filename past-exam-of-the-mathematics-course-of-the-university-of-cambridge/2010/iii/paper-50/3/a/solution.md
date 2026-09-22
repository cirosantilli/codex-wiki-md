<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For [reachability in control theory](../../../../../../reachability-in-control-theory.md), a state $x_1$ is reachable from $x_0$ if an admissible input and a permitted duration drive the dynamical system from $x_0$ to $x_1$. [Controllability](../../../../../../controllability.md) requires this for every initial-target pair in the specified state space. Restrictions on duration or field amplitudes change the reachable set, so the admissible controls are part of the definition.

For a closed quantum system, $\dot U=-iH[f(t)]U$, $U(0)=I$, and states evolve as $\psi(t)=U(t)\psi(0)$ or $\rho(t)=U(t)\rho(0)U(t)^\dagger$. This gives three notions of [quantum controllability](../../../../../../quantum-controllability.md). [Unitary operator controllability](../../../../../../unitary-operator-controllability.md) requires every desired $U_d\in U(N)$ to be reachable from the identity; when a [global phase](../../../../../../global-phase.md) is immaterial, one instead asks for every special unitary operation. [Density operator controllability](../../../../../../density-operator-controllability.md) requires every pair of [density operators](../../../../../../density-matrix.md) with the same spectrum to be connected. The spectral qualification is necessary because [unitary time evolution](../../../../../../unitary-time-evolution.md) cannot change eigenvalues; the natural state space is a [unitary orbit of a density operator](../../../../../../unitary-orbit-of-a-density-operator.md). [Pure-state controllability](../../../../../../pure-state-controllability.md) requires any normalized initial state to be transferred to any target ray, $U(T)\psi_0=e^{i\chi}\psi_d$.

Thus $\boxed{\text{operator controllability}\Rightarrow\text{density operator controllability}\Rightarrow\text{pure-state controllability}}$, with the operator implication also valid if [global phase](../../../../../../global-phase.md) is discarded. The converse implications need not hold. A pure-state task concerns one vector, whereas an operator task must act correctly on every input vector at once.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
