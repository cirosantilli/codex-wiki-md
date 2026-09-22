<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [operator norm](../../../../../../operator-norm.md) induced by the usual vector norm, and assume the input [quantum state](../../../../../../quantum-state.md) is normalized. Since $J(\alpha)=HP(\alpha)$ and the [Hadamard gate](../../../../../../hadamard-gate.md) is unitary, the [J-gate phase-error operator norm](../../../../../../j-gate-phase-error-operator-norm.md) is

$$
\|J(\alpha')-J(\alpha)\|
=\|P(\alpha')-P(\alpha)\|
=|e^{i\alpha'}-e^{i\alpha}|
=2\left|\sin\frac{\alpha'-\alpha}{2}\right|
\leq|\alpha'-\alpha|<\eta.
$$

Write the exact and implemented [quantum circuits](../../../../../../quantum-circuit-split.md) as ordered products $C=U_m\cdots U_1$ and $C'=U'_m\cdots U'_1$. The [quantum circuit gate-error telescoping bound](../../../../../../quantum-circuit-gate-error-telescoping-bound.md) follows from

$$
C'-C=\sum_{j=1}^mU'_m\cdots U'_{j+1}(U'_j-U_j)U_{j-1}\cdots U_1.
$$

Every surrounding factor is unitary, including gates tensored with identities on other [qubits](../../../../../../qubit.md), so the [triangle inequality](../../../../../../triangle-inequality.md) and the [submultiplicativity of the operator norm](../../../../../../submultiplicativity-of-the-operator-norm.md) give

$$
\|C'-C\|\leq\sum_j\|U'_j-U_j\|<k\eta.
$$

The exact [Controlled-Z gates](../../../../../../controlled-z-gate.md) contribute zero to that sum. Thus

$$
\||\psi'_{\rm out}\rangle-|\psi_{\rm out}\rangle\|
\leq\|C'-C\|<k\eta,
\qquad
\boxed{0<\eta\leq\frac{\epsilon}{k}\quad(k\geq1)}.
$$

The endpoint $\eta=\epsilon/k$ is sufficient because each implemented angle error is strictly smaller than $\eta$. If $k=0$, the circuits are identical and any positive $\eta$ works. The bound controls the stated vector distance with actual gate phases retained, so no adjustment of the global phase of one output is needed.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
