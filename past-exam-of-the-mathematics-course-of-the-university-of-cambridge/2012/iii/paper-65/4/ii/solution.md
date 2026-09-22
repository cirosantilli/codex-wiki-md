<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Diagonalize the source average $\pi=\sum_j\lambda_j|j\rangle\langle j|$, using its positive eigenvalues. For fixed $\delta>0$, let $\Pi_{n,\delta}$ project onto product eigenvectors whose eigenvalues obey

$$
2^{-n(S(\pi)+\delta)}\leq\lambda_{j_1}\cdots\lambda_{j_n}
\leq2^{-n(S(\pi)-\delta)}.
$$

The [typical subspace theorem](../../../../../../typical-subspace-theorem.md) states that, for every $\epsilon>0$ and all sufficiently large $n$,

$$
\operatorname{Tr}(\pi^{\otimes n}\Pi_{n,\delta})\geq1-\epsilon,
$$



$$
2^{-n(S(\pi)+\delta)}\Pi_{n,\delta}
\leq\Pi_{n,\delta}\pi^{\otimes n}\Pi_{n,\delta}
\leq2^{-n(S(\pi)-\delta)}\Pi_{n,\delta},
$$



$$
(1-\epsilon)2^{n(S(\pi)-\delta)}
\leq\dim\mathcal T_{n,\delta}\leq2^{n(S(\pi)+\delta)}.
$$

The probability statement is the [weak law of large numbers](../../../../../../weak-law-of-large-numbers.md) applied to $-\log_2\lambda_j$; the dimension bounds follow by summing the typical eigenvalue bounds. This explains why the [quantum typical subspace](../../../../../../quantum-typical-subspace.md) retains almost all probability using about $nS(\pi)$ qubits.

For $R>S(\pi)$ choose $0<\delta<R-S(\pi)$. Measure $\{\Pi_{n,\delta},I-\Pi_{n,\delta}\}$. On success, encode the projected state isometrically into a space of dimension $\dim\mathcal T_{n,\delta}$; on failure, output a separate fixed flag. Decode the successful sector by the inverse [isometry](../../../../../../isometry.md), and map the flag to a fixed state $|\varphi_0\rangle$. The compressed dimension is at most $2^{n(S(\pi)+\delta)}+1$, hence fits within rate $R$ for all sufficiently large $n$. Both maps are trace-preserving [quantum channels](../../../../../../quantum-channel.md), not merely successful postselected operations.

Writing $\Pi=\Pi_{n,\delta}$, the composite channel is

$$
\mathcal N_n(\tau)=\Pi\tau\Pi+
\operatorname{Tr}[(I-\Pi)\tau]|\varphi_0\rangle\langle\varphi_0|.
$$

For a pure source signal $|\Psi_k\rangle$, set $a_k=\langle\Psi_k|\Pi|\Psi_k\rangle$. Its squared [quantum fidelity](../../../../../../fidelity-of-quantum-states.md) after the composite channel is at least $a_k^2$. Since the source is memoryless, its average state on $n$ uses is $\pi^{\otimes n}$. Convexity of the square gives

$$
\sum_kp_k^{(n)}\langle\Psi_k|\mathcal N_n(|\Psi_k\rangle\langle\Psi_k|)|\Psi_k\rangle
\geq\sum_kp_k^{(n)}a_k^2
\geq\left[\operatorname{Tr}(\pi^{\otimes n}\Pi)\right]^2
\geq(1-\epsilon)^2.
$$

The [Kraus formula for entanglement fidelity](../../../../../../kraus-formula-for-entanglement-fidelity.md) gives the same lower bound for $F_e(\pi^{\otimes n},\mathcal N_n)$, because one [Kraus operator](../../../../../../kraus-operator.md) is $\Pi$ and the other terms are nonnegative. Taking $\epsilon\to0$ proves **reliable compression at every $R>S(\pi)$**, in both average pure-signal fidelity and the stronger entanglement-fidelity sense. This is [typical-subspace compression with a failure flag](../../../../../../typical-subspace-compression-with-a-failure-flag.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
