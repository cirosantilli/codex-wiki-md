<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the [quantum circuit](../../../../../../quantum-circuit-split.md) as $U=U_T\cdots U_1$, and let $V_0=I$, $V_t=U_t\cdots U_1$. Use a [nonlocal quantum clock](../../../../../../nonlocal-quantum-clock.md) with orthonormal states $|0\rangle,\ldots,|T\rangle$. Let the work space include the [quantum witness](../../../../../../quantum-witness.md) and the [ancilla qubits](../../../../../../ancilla-qubit.md). The [input penalty of a history Hamiltonian](../../../../../../input-penalty-of-a-history-hamiltonian.md) is built from

$$
Q=\sum_{a\in A_0}|1\rangle\langle1|_a+\sum_{a\in A_+}|-\rangle\langle-|_a.
$$

It annihilates precisely the correctly initialized [ancilla qubits](../../../../../../ancilla-qubit.md), leaving the [quantum witness](../../../../../../quantum-witness.md) unrestricted. The [Feynman-Kitaev Hamiltonian](../../../../../../feynman-kitaev-hamiltonian.md) without output penalty is

$$
\boxed{H=H_{\rm in}+H_{\rm prop},\qquad H_{\rm in}=Q\otimes|0\rangle\langle0|,}
$$



$$
H_{\rm prop}=\frac12\sum_{t=1}^T\left[I\otimes\bigl(|t\rangle\langle t|+|t-1\rangle\langle t-1|\bigr)-U_t\otimes|t\rangle\langle t-1|-U_t^\dagger\otimes|t-1\rangle\langle t|\right].
$$

Each propagation summand is positive: on vectors with adjacent clock components $\eta_{t-1},\eta_t$, its [quadratic form](../../../../../../quadratic-form.md) is $\tfrac12\|\eta_t-U_t\eta_{t-1}\|^2$. The [input penalty of a history Hamiltonian](../../../../../../input-penalty-of-a-history-hamiltonian.md) is also a [positive semidefinite operator](../../../../../../positive-operator.md), so $H\geq0$.

To verify that this is a [stoquastic Hamiltonian](../../../../../../stoquastic-hamiltonian.md), use the work [computational basis](../../../../../../computational-basis.md) and the clock basis. Every $U_t$ is a [permutation matrix](../../../../../../permutation-matrix.md), so the propagation off-diagonal entries are nonpositive. The zero-ancilla projectors are diagonal, while $|-\rangle\langle-|=\tfrac12\begin{pmatrix}1&-1\\-1&1\end{pmatrix}$ also has nonpositive off-diagonal entries. No positive off-diagonal entry is introduced by summing these terms. **Thus $H$ is positive semidefinite and stoquastic, with no output penalty.**

The construction uses the abstract $T+1$ dimensional clock space. A binary implementation needs diagonal penalties for unused clock labels. The clock transitions are nonlocal; the construction alone does not establish fixed qubit locality of an ordinary [local Hamiltonian problem](../../../../../../local-hamiltonian-problem.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 63](../../../paper-63-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
