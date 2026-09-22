<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $|0\rangle=|\uparrow_z\rangle$ and $|1\rangle=|\downarrow_z\rangle$. The [total-spin sector](../../../../../../total-spin-sector.md) with spin zero consists of the [spin singlet state](../../../../../../spin-singlet-state.md) $|\Psi^-\rangle=(|01\rangle-|10\rangle)/\sqrt2$, not the whole subspace with zero $z$ component. These must be distinguished: the [Bell state](../../../../../../bell-state-split.md) $|\Psi^+\rangle$ has zero $z$ component but total spin one.

There are two meanings of verification to separate here. A one-pair [entanglement-assisted statistical singlet verification](../../../../../../entanglement-assisted-statistical-singlet-verification.md) is possible: choose a shared random axis from $x,y,z$, measure that axis's two-spin parity by the meter circuit below, and accept anticorrelation. An $x$ or $y$ test uses local basis changes before and after the computational-axis circuit. The singlet always passes and is unchanged. Averaging the three acceptance projectors gives

$$
\Omega=\frac13\sum_{j=x,y,z}\frac{I-\sigma_j\otimes\sigma_j}{2}
=P_s+\frac13(I-P_s).
$$

Every triplet state passes with probability $1/3$, so a failure excludes the singlet, while repeated tests on independently prepared copies can give statistical confidence. A single pass does not certify the singlet with certainty.

**Exact single-shot verification cannot be implemented with just one shared Bell pair.** Here exact verification means a yes outcome with probability one on the [spin singlet state](../../../../../../spin-singlet-state.md), zero on its orthogonal complement, and preservation of the singlet on yes. If that stronger meaning is intended, the question needs an extra resource. The [Bell-pair cost of exact nondemolition singlet verification](../../../../../../bell-pair-cost-of-exact-nondemolition-singlet-verification.md) gives a short proof. For a fully resolved tuple $\mu,\nu$ of local measurement records, contraction of the shared $|\Phi^+\rangle$ gives a system [Kraus operator](../../../../../../kraus-operator.md)

$$
K_{\mu\nu}=\frac1{\sqrt2}\left(A_{\mu0}\otimes B_{\nu0}+A_{\mu1}\otimes B_{\nu1}\right).
$$

Local ancillas and locally adaptive operations are included in these operators. Refining any unobserved local environment gives the same form, so the [operator Schmidt rank](../../../../../../operator-schmidt-rank.md) is at most two. On each nonzero yes branch, zero false positives forces $K_{\mu\nu}$ to vanish on the entire triplet subspace, and singlet preservation forces

$$
K_{\mu\nu}=c_{\mu\nu}P_s,\qquad
P_s=\frac14(I\otimes I-X\otimes X-Y\otimes Y-Z\otimes Z).
$$

The four [Pauli matrices](../../../../../../pauli-matrices.md), including the identity, are an orthogonal operator basis. Thus $P_s$ has [operator Schmidt rank](../../../../../../operator-schmidt-rank.md) four, contradicting the rank-two bound. At least one yes branch is nonzero because the singlet must pass with certainty. Shared classical randomness cannot evade this branchwise argument.

With **two shared Bell pairs**, an explicit corrected protocol is available. On the first meter pair, apply local system-to-meter [CNOT gates](../../../../../../controlled-not-gate.md) and measure both meters in the computational basis. If their records are $u,v$, the [Kraus operator](../../../../../../kraus-operator.md) is $P_z/\sqrt2$, where $z=(-1)^{u\oplus v}$ and $P_z=(I+zZ_AZ_B)/2$. On the second pair, measure $X_AX_B$ by the same circuit conjugated with local [Hadamard gates](../../../../../../hadamard-gate.md) on the system. The two parities commute, and their joint projectors are the four [Bell-state nondemolition measurement](../../../../../../bell-state-nondemolition-measurement.md) projectors. The singlet is exactly the outcome $(z,x)=(-1,-1)$ and remains unchanged. Local interactions and readouts fit within the stated interval; the combined verdict becomes available only after the records are compared by [classical communication](../../../../../../classical-communication.md).

This corrected exact protocol resolves the triplet into three [Bell states](../../../../../../bell-state-split.md). It preserves the singlet and every [Bell state](../../../../../../bell-state-split.md), but generally destroys triplet superpositions. A binary [Lüders rule](../../../../../../luders-rule.md) measurement preserving all triplet coherence is a different operation: it violates the [singlet-triplet measurement causality obstruction](../../../../../../singlet-triplet-measurement-causality-obstruction.md). The one-pair protocol used below measures a single parity and supplies the statistical test above; it does not give exact single-shot singlet verification.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
