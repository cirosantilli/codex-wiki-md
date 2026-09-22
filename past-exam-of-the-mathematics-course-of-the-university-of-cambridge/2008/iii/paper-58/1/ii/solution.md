<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Here is a [tripartite Schmidt projection entanglement concentration](../../../../../../tripartite-schmidt-projection-entanglement-concentration.md) protocol. For $0<p<1$, set $q=1-p$. Regrouping the $n$ local [qubits](../../../../../../qubit.md) of each party gives

$$
|\Psi_1\rangle^{\otimes n}=\sum_{x\in\{0,1\}^n}p^{(n-|x|)/2}q^{|x|/2}|x\rangle_A|x\rangle_B|x\rangle_C,
$$

where $|x|$ counts ones. Alice performs a [projective measurement](../../../../../../projective-measurement.md) of that count, without learning the individual string. The [orthogonal projector](../../../../../../orthogonal-projection.md) for outcome $k$ is $\Pi_k=\sum_{|x|=k}|x\rangle\langle x|$. By the [Born rule](../../../../../../born-rule.md), its [probability](../../../../../../probability.md) and conditional [pure state](../../../../../../pure-state.md) are

$$
P_k=\binom nk p^{n-k}q^k,\qquad
|T_k\rangle=\frac1{\sqrt{d_k}}\sum_{|x|=k}|x\rangle_A|x\rangle_B|x\rangle_C,\qquad d_k=\binom nk.
$$

Alice sends $k$ by [classical communication](../../../../../../classical-communication.md); all three parties use [local unitary operations](../../../../../../local-unitary-operation.md) to relabel the same ordered type class as $0,\ldots,d_k-1$. There are now $d_k$ equal common-label amplitudes. Measuring the individual [qubits](../../../../../../qubit.md) instead would have destroyed precisely this coherence.

To obtain an integer number $f$ of target [GHZ states](../../../../../../greenberger-horne-zeilinger-state.md), choose $m=2^f\leq d_k$. The following exact [LOCC](../../../../../../local-operations-and-classical-communication.md) step handles type classes whose sizes are not powers of two. For every $m$-element subset $S\subseteq\{0,\ldots,d_k-1\}$, Alice uses the [Kraus operator](../../../../../../kraus-operator.md)

$$
K_S=\frac{\Pi_S}{\sqrt{\binom{d_k-1}{m-1}}},\qquad \Pi_S=\sum_{r\in S}|r\rangle\langle r|.
$$

Every label occurs in $\binom{d_k-1}{m-1}$ such subsets, proving $\sum_SK_S^\dagger K_S=I$ on the occupied subspace. Thus this is a complete [measurement in quantum mechanics](../../../../../../quantum-measurement-split.md). Each outcome has [probability](../../../../../../probability.md) $m/[d_k\binom{d_k-1}{m-1}]=1/\binom{d_k}{m}$, and leaves the normalized [pure state](../../../../../../pure-state.md) $m^{-1/2}\sum_{r\in S}|r,r,r\rangle$. After Alice communicates $S$, all parties relabel its elements in the same order. Binary expansion of the labels then factors the state into **exactly $f$ independent copies of the target GHZ state**. Local extensions of these operations handle unused basis vectors and do not affect the protocol.

For example, taking $f(k)=\lfloor\log_2d_k\rfloor$ gives an outcome-dependent yield without any failure branch. Since $K$ has a [binomial distribution](../../../../../../binomial-distribution.md) with parameters $(n,q)$, the [weak law of large numbers](../../../../../../weak-law-of-large-numbers.md) gives $K/n\to q$ in probability. [Stirling's formula](../../../../../../stirling-formula.md), uniformly when $k/n$ stays away from zero and one, gives

$$
\log_2\binom nk=nh_2(k/n)-\frac12\log_2\bigl(2\pi n(k/n)(1-k/n)\bigr)+O(n^{-1}).
$$

By continuity of the [binary entropy](../../../../../../binary-entropy.md), $f(K)/n\to h_2(q)=h_2(p)$ in probability. The integer rounding and logarithmic correction have no first-order effect.

A fixed yield with success probability tending to one is also explicit. For sufficiently large $n$, take

$$
f_n=\left\lfloor nh_2(p)-n^{3/4}\right\rfloor.
$$

On $|K-nq|\leq n^{2/3}$, the bounded derivative of the [binary entropy](../../../../../../binary-entropy.md) in a neighborhood of the fixed $q\in(0,1)$ and [Stirling's formula](../../../../../../stirling-formula.md) give $\log_2d_K\geq nh_2(q)-C_qn^{2/3}-O(\log n)\geq f_n$. [Chebyshev's inequality](../../../../../../chebyshev-inequality.md) bounds the complementary [probability](../../../../../../probability.md) by $q(1-q)n^{-1/3}$. Abort there if necessary, and otherwise use the subset [measurement in quantum mechanics](../../../../../../quantum-measurement-split.md) with $m=2^{f_n}$. Thus

$$
\boxed{P(\text{success})\longrightarrow1,\qquad f_n/n\longrightarrow h_2(p).}
$$

This matches the first-order rate in part (i), with exact outputs on every successful forward branch. If $p=1/2$, simply retain the original $n$ target copies; if $p$ is an endpoint, output zero target copies.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
