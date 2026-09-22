<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The [Schumacher compression](../../../../../schumacher-compression.md) theorem concerns a [memoryless quantum information source](../../../../../memoryless-quantum-information-source.md) with average [density matrix](../../../../../density-matrix.md) $\rho$ on a finite-dimensional [Hilbert space](../../../../../hilbert-space-split.md). For $n$ uses the average state is $\rho_n=\rho^{\otimes n}$. Compression consists of an encoding [quantum channel](../../../../../quantum-channel.md) into a space of dimension $D_n$ and a decoding channel back to the original block space, with asymptotic rate $n^{-1}\log_2D_n$ qubits per source use. **The optimal reliable rate is $S(\rho)$: every larger rate is achievable, and no smaller rate is reliable.** This holds for average pure-source fidelity; the direct construction also preserves a purification reference, and the converse for that stronger [entanglement fidelity](../../../../../entanglement-fidelity.md) criterion holds with fidelity tending to zero below the threshold. The encoding and decoding are deterministic channels; no free classical transmission of the source label is allowed.

Diagonalize $\rho=\sum_j\lambda_j|j\rangle\langle j|$ and omit zero-probability eigenvalues when sampling. Define the [quantum typical subspace](../../../../../quantum-typical-subspace.md) projector $P_{n,\delta}$ by retaining product eigenvectors with

$$
2^{-n(S+\delta)}\leq\lambda_{j_1}\cdots\lambda_{j_n}\leq2^{-n(S-\delta)}.
$$

The sampled random variable $-\log_2\lambda_j$ has expectation $S=S(\rho)$. The [weak law of large numbers](../../../../../weak-law-of-large-numbers.md) gives $w_n=\operatorname{Tr}(\rho_nP_{n,\delta})\to1$. Every retained eigenvalue is at least $2^{-n(S+\delta)}$, and the total probability is at most one, so

$$
\operatorname{rank}P_{n,\delta}\leq2^{n(S+\delta)}.
$$

This proves the two [typical subspace theorem](../../../../../typical-subspace-theorem.md) estimates used in the direct part.

Write $P=P_{n,\delta}$. Encode its range isometrically into a compressed space and reserve one orthogonal failure flag. Decode the range back isometrically and the failure flag to a fixed pure state $|\varphi\rangle$. This [typical-subspace compression with a failure flag](../../../../../typical-subspace-compression-with-a-failure-flag.md) is a physical channel whose composite action is

$$
\mathcal N_n(X)=PXP+\operatorname{Tr}[(I-P)X]|\varphi\rangle\langle\varphi|.
$$

Indeed its Kraus operators are $P$ and $|\varphi\rangle\langle e_a|$, where the $e_a$ form an orthonormal basis of $\ker P$, and their adjoint products sum to $I$. The [Kraus formula for entanglement fidelity](../../../../../kraus-formula-for-entanglement-fidelity.md) gives

$$
F_e(\rho_n,\mathcal N_n)=\sum_\alpha|\operatorname{Tr}(\rho_nK_\alpha)|^2\geq w_n^2\longrightarrow1.
$$

For any pure-state ensemble of $\rho_n$, the average squared [quantum fidelity](../../../../../fidelity-of-quantum-states.md) is at least this number: apply convexity of $|z|^2$ separately to the amplitudes $\langle\psi_x|K_\alpha|\psi_x\rangle$ with their source probabilities. Thus average fidelity also tends to one. The compressed dimension is at most $2^{n(S+\delta)}+1$, and its rate is at most $S+\delta+o(1)$. Choose $\delta<R-S$ for any prescribed $R>S$. One may also take $\delta_n=n^{-1/4}$: the finite spectral information variance and [Chebyshev's inequality](../../../../../chebyshev-inequality.md) still give $w_n\to1$, with rate tending to $S$. A pure source, $S=0$, can simply be re-prepared exactly without sending any qubits.

For the coherent converse, we prove the [finite-dimensional quantum compression converse](../../../../../finite-dimensional-quantum-compression-converse.md). If the compressed space has dimension $D$, the state of reference plus compressed system has a pure-state decomposition with [Schmidt rank](../../../../../schmidt-rank.md) at most $D$. Applying decoder Kraus operators locally cannot increase the Schmidt rank of those vectors, so the final reference–output state has [Schmidt number](../../../../../schmidt-number.md) at most $D$. Let $|\Psi_{\rho_n}\rangle$ purify the source, with squared Schmidt coefficients equal to the decreasing eigenvalues $\mu_1\geq\mu_2\geq\cdots$ of $\rho_n$. For any normalized vector $|v\rangle$ of Schmidt rank at most $D$, its reference support lies in a rank-at-most-$D$ projector $Q$. Hence

$$
|\langle\Psi_{\rho_n}|v\rangle|^2
\leq\|(Q\otimes I)|\Psi_{\rho_n}\rangle\|^2
=\operatorname{Tr}(Q\rho_{n,R})\leq\sum_{j=1}^D\mu_j.
$$

The last bound follows by maximizing $\sum_j\mu_j\langle j|Q|j\rangle$ subject to $0\leq\langle j|Q|j\rangle\leq1$ and their sum at most $D$. Average over a Schmidt-rank-bounded decomposition of the final state to obtain $F_e\leq\sum_{j=1}^D\mu_j$.

At rate $R<S$, choose $0<\delta<S-R$. The total source probability outside the [quantum typical subspace](../../../../../quantum-typical-subspace.md) tends to zero, while every eigenvalue inside it is at most $2^{-n(S-\delta)}$. Therefore for $D_n\leq2^{nR}$,

$$
F_e\leq\sum_{j=1}^{D_n}\mu_j\leq(1-w_n)+2^{nR}2^{-n(S-\delta)}\longrightarrow0.
$$

This argument allows arbitrary encoding and decoding channels, not only subspace projection.

For completeness, average pure-source reliability also forces the same rate, even though it is a weaker criterion than entanglement fidelity. Here is a separate converse for that formulation. Let the emitted block pure states be $\psi_x$, with probabilities $p_x$, and let $\sigma_x$ be the decoded states. If their mean squared fidelity tends to one, then their mean [trace distance](../../../../../trace-distance.md) $\bar\delta_n$ tends to zero, since $\tfrac12\|\sigma_x-\psi_x\|_1\leq\sqrt{1-\langle\psi_x|\sigma_x|\psi_x\rangle}$. This inequality follows by choosing a purification with that overlap and using contraction of trace distance under a partial trace.

We need only an elementary [entropy continuity from Jordan decomposition](../../../../../entropy-continuity-from-jordan-decomposition.md) bound, derivable from Question 4. If $\delta=\tfrac12\|\sigma-\tau\|_1$, write the positive and negative parts of $\sigma-\tau$ as $\delta\omega_+,\delta\omega_-$. The common density matrix

$$
\frac{\sigma+\delta\omega_-}{1+\delta}=\frac{\tau+\delta\omega_+}{1+\delta}
$$

and the two mixture bounds give

$$
|S(\sigma)-S(\tau)|\leq\delta\log_2d+g(\delta),\qquad
g(\delta)=(1+\delta)h_2\left(\frac\delta{1+\delta}\right).
$$

Here $g$ is increasing and concave, $g(0)=0$. Apply this in block dimension $d^n$, both to the average states and to individual outputs, using convexity of trace distance and concavity of $g$. Since the original ensemble is pure, its [Holevo quantity](../../../../../holevo-quantity.md) is $S(\rho_n)=nS$. The decoded ensemble has

$$
\chi_{\mathrm{out}}=S\left(\sum_xp_x\sigma_x\right)-\sum_xp_xS(\sigma_x)
\geq nS-2\bar\delta_n n\log_2d-2g(\bar\delta_n)=nS-o(n).
$$

The [Holevo quantity under a quantum channel](../../../../../holevo-quantity-under-a-quantum-channel.md) cannot increase. To specify the entropy ingredient, [Strong subadditivity of Von Neumann entropy](../../../../../strong-subadditivity-of-quantum-entropy.md) states $S(XB)+S(BE)\geq S(B)+S(XBE)$. Attach the classical source label $X$, dilate the decoder isometrically to $BE$, and trace out $E$. The displayed inequality says $I(X:B)\leq I(X:BE)$; the isometry preserves the input mutual information. Since $I(X:B)$ of a labelled ensemble is its Holevo quantity, this proves the needed decoder monotonicity. Before decoding, the system has dimension $D_n$, so its Holevo quantity is at most $\log_2D_n$. Thus $\log_2D_n\geq nS-o(n)$ and the rate cannot be below $S$. **Both operational fidelity formulations therefore have the claimed noiseless coding threshold.**

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
