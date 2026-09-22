# Sequential qubit measurement correlation

↑ **Parent:** [Quantum measurement](quantum-measurement-split.md)

Prepare $I/2$, measure a Pauli observable $N=\mathbf n\cdot\boldsymbol\sigma$, apply a fixed [unitary operator](unitary-operator.md) $U$, then measure $N$ again. If the first and second [eigenvalue](eigenvalue.md) labels are $j,k\in\{+1,-1\}$, their joint [probability](probability.md) is $\frac12|\langle n_k|U|n_j\rangle|^2$. Consequently

$$
E_{\mathbf n}(U)=\mathbb E[jk]=\frac12\operatorname{Tr}(NUNU^\dagger).
$$

The first outcome has [probability](probability.md) $1/2$ and its conditional state is $|n_j\rangle$ by the [Lüders rule](luders-rule.md). Summing $jk$ times the joint [probabilities](probability.md) and using $N=\sum_jj|n_j\rangle\langle n_j|$ proves the [trace](matrix-trace.md) formula. This temporal correlation differs from the spatial correlation $\langle\psi|N\otimes N|\psi\rangle$ of two simultaneously measured [qubits](qubit.md).

## ↑ Ancestors (5)

1. [Quantum measurement](quantum-measurement-split.md)
2. [Quantum theory](quantum-theory-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)
