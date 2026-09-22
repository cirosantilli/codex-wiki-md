<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use base-two logarithms throughout, so classical rates are measured in bits and quantum compression rates in qubits. A [memoryless classical information source](../../../../../memoryless-classical-information-source.md) is a sequence $U_1,U_2,\ldots$ of [independent and identically distributed random variables](../../../../../independent-and-identically-distributed-random-variables.md) on a finite alphabet $\mathcal U$, with fixed [probability mass function](../../../../../probability-mass-function.md) $p$. A length-$n$ word has probability $p(u^n)=\prod_{j=1}^np(u_j)$, and the one-symbol [Shannon entropy](../../../../../information-entropy.md) is $H(U)=-\sum_up(u)\log_2p(u)$, with $0\log_20=0$.

For $\varepsilon>0$, the [typical set](../../../../../typical-set.md) is

$$
T_\varepsilon^{(n)}=\left\{u^n:p(u^n)>0,\quad
\left|-\frac1n\log_2p(u^n)-H(U)\right|\leq\varepsilon\right\}.
$$

This is weak typicality: it constrains the normalized self-information, not each empirical symbol count separately.

The [typical sequence theorem](../../../../../typical-sequence-theorem.md) gives the following three facts for fixed $\varepsilon>0$. The [probability](../../../../../probability.md) $P(U^n\in T_\varepsilon^{(n)})$ tends to one; each word in the set has probability between $2^{-n(H(U)+\varepsilon)}$ and $2^{-n(H(U)-\varepsilon)}$; and, once the set has probability at least $1-\delta$,

$$
(1-\delta)2^{n(H(U)-\varepsilon)}\leq |T_\varepsilon^{(n)}|
\leq2^{n(H(U)+\varepsilon)}.
$$

The concentration assertion follows from the [weak law of large numbers](../../../../../weak-law-of-large-numbers.md) applied to the iid information variables $-\log_2p(U_j)$, whose finite-alphabet mean is $H(U)$. The probability bounds are the definition of typicality exponentiated. Summing the lower bound over the typical words and using total probability at most one proves the cardinality upper bound; summing the upper bound and using total typical probability at least $1-\delta$ proves the lower bound.

Fix $R>H(U)$ and choose $0<\varepsilon<R-H(U)$. Enumerate all words in $T_\varepsilon^{(n)}$ and assign a distinct fixed-length binary index to each. Reserve one more index as a failure symbol for every atypical input. For all sufficiently large $n$,

$$
|T_\varepsilon^{(n)}|+1\leq2^{\lceil nR\rceil},
$$

so these indices can be transmitted using $\lceil nR\rceil$ bits. The decoder inverts the typical-word enumeration; on the failure index it returns any fixed word. This describes both the compressor and decompressor, and its block error probability obeys

$$
\boxed{P(\widehat U^n\ne U^n)\leq P(U^n\notin T_\varepsilon^{(n)})\longrightarrow0.}
$$

Its rate tends to $R$ bits per symbol. Thus every $R>H(U)$ permits reliable fixed-rate compression, with no claim that atypical words are reconstructed correctly.

For the [memoryless quantum information source](../../../../../memoryless-quantum-information-source.md), the average one-use [density matrix](../../../../../density-matrix.md) is

$$
\rho=\frac12|0\rangle\langle0|+\frac12|+\rangle\langle+|
=\begin{pmatrix}3/4&1/4\\1/4&1/4\end{pmatrix}.
$$

Its trace is one and determinant $1/8$, so its two [eigenvalues](../../../../../eigenvalue.md) are

$$
\lambda_\pm=\frac12\left(1\pm\frac1{\sqrt2}\right).
$$

The source-coding limit in [Schumacher compression](../../../../../schumacher-compression.md) is the [Von Neumann entropy](../../../../../von-neumann-entropy-split.md) of this average state: every larger qubit rate allows asymptotically faithful recovery of the emitted states, and a smaller rate cannot do so. Applying that limit gives

$$
\boxed{R_{\mathrm{opt}}=S(\rho)
=h_2\!\left(\frac{1+1/\sqrt2}{2}\right)\approx0.600876\ \text{qubits per signal},}
$$

where $h_2(t)=-t\log_2t-(1-t)\log_2(1-t)$ is the [binary entropy](../../../../../binary-entropy.md). The [quantum typical subspace](../../../../../quantum-typical-subspace.md) of $\rho^{\otimes n}$ has dimension about $2^{nS(\rho)}$ and carries asymptotically all source weight, which explains the compression rate. The entropy of the classical emission label is one bit; it is not the quantum rate because the two emitted [pure states](../../../../../pure-state.md) are nonorthogonal.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 60](../../paper-60-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
