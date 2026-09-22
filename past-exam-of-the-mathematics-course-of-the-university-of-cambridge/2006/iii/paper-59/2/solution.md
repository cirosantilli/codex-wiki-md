<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The target states here are [qubit](../../../../../qubit.md) states, as appropriate to sharing [singlet states](../../../../../singlet-state.md) of two [qubits](../../../../../qubit.md). Write $|\psi\rangle=\alpha|0\rangle+\beta|1\rangle$ and choose $|\psi^\perp\rangle=-\beta^*|0\rangle+\alpha^*|1\rangle$. These form an [orthonormal basis](../../../../../orthonormal-basis.md), and the shared [Bell state](../../../../../bell-state-split.md) can be expressed as

$$
|\Psi^-\rangle_{AB}
=\frac{|0\rangle_A|1\rangle_B-|1\rangle_A|0\rangle_B}{\sqrt2}
=\frac{|\psi\rangle_A|\psi^\perp\rangle_B
-|\psi^\perp\rangle_A|\psi\rangle_B}{\sqrt2}.
$$

Alice knows the classical description of $|\psi\rangle$, so she can perform the [projective measurement](../../../../../projective-measurement.md) in this basis. The outcome $|\psi^\perp\rangle$ has [probability](../../../../../probability.md) $1/2$ and leaves Bob in $|\psi\rangle$, up to an irrelevant overall phase. Alice sends a success [bit](../../../../../bit.md): one for this outcome and zero for the other. Bob keeps his [qubit](../../../../../qubit.md) only on success. This proves [heralded remote preparation of an arbitrary qubit](../../../../../heralded-remote-preparation-of-an-arbitrary-qubit.md):

$$
\boxed{p_{\mathrm{success}}=\frac12,\qquad
\text{one singlet and one classical success flag}.}
$$

The other outcome leaves $|\psi^\perp\rangle$ at Bob's side; the protocol makes no claim of success in that branch.

For a block of $n$ targets, share $n$ independent [singlet states](../../../../../singlet-state.md). Alice measures her $j$th [qubit](../../../../../qubit.md) in the basis $|\psi_j\rangle,|\psi_j^\perp\rangle$. She sends one [bit](../../../../../bit.md) indicating whether all $n$ outcomes were of the successful kind. Because the pairs are independent, all-success has [probability](../../../../../probability.md) $2^{-n}$; conditioned on it, Bob's joint state is precisely $\bigotimes_{j=1}^n|\psi_j\rangle$. Thus [one-bit heralding of a remote state preparation block](../../../../../one-bit-heralding-of-a-remote-state-preparation-block.md) gives

$$
\boxed{p_{\mathrm{success}}=2^{-n},\qquad
n\text{ singlets and one block-success flag}.}
$$

On failure Bob discards the block, so he does not need a list of which component states failed.

For [asymptotic remote state preparation by block indexing](../../../../../asymptotic-remote-state-preparation-by-block-indexing.md), prelabel a supply of independent candidate blocks, each containing $n$ [singlet states](../../../../../singlet-state.md). Alice measures blocks until she finds the first all-success block, of index $J$. She does not send a flag after each trial. Since $q=2^{-n}$ is the success [probability](../../../../../probability.md) of each block,

$$
\mathbb P(J=j)=q(1-q)^{j-1},\qquad j\geq1.
$$

This [geometric distribution](../../../../../geometric-distribution.md) is independent of the target states. The [probability](../../../../../probability.md) of never succeeding is $\lim_{k\to\infty}(1-q)^k=0$. Alice needs to communicate only $J$; Bob retrieves the labelled [qubits](../../../../../qubit.md) in that block, and thereby knows that every requested state was prepared exactly.

Here is an explicit [prefix code for a rare geometric success](../../../../../prefix-code-for-a-rare-geometric-success.md). Set $M=2^n$ and divide $J-1=MQ+R$, where $0\leq R<M$. Encode $Q$ as $Q$ ones followed by zero, then encode $R$ in exactly $n$ [bits](../../../../../bit.md). Bob can decode this without knowing any target-state description. The message length is $L=n+Q+1$. With $r=(1-q)^M$,

$$
\mathbb P(Q\geq k)=r^k,\qquad
\mathbb E Q=\sum_{k=1}^\infty r^k=\frac{r}{1-r}.
$$

Since $(1-1/M)^M\leq e^{-1}$,

$$
\boxed{\mathbb E L=n+\frac1{1-r}\leq n+\frac e{e-1},\qquad
\frac{\mathbb E L}{n}\longrightarrow1.}
$$

This version succeeds exactly with [probability](../../../../../probability.md) one and has the stated expected [classical communication](../../../../../classical-communication.md) cost. It consumes $n\,\mathbb EJ=n2^n$ [singlet states](../../../../../singlet-state.md) on average, compatible with the unlimited entanglement assumption.

There is also a fixed-message-length version. Try at most $K=n2^n$ candidate blocks and send the first successful index, or a zero codeword reporting that none succeeded. Encoding the $K+1$ possibilities uses $\lceil\log_2(K+1)\rceil=n+\log_2n+O(1)$ [bits](../../../../../bit.md). Its failure [probability](../../../../../probability.md) is

$$
(1-2^{-n})^{n2^n}\leq e^{-n}.
$$

Thus **fixed-length communication approaches one [bit](../../../../../bit.md) per state with success [probability](../../../../../probability.md) tending to one; variable-length communication achieves exact eventual success with expected cost approaching one [bit](../../../../../bit.md) per state.** Before the index arrives, Bob's unconditional state remains independent of the target descriptions, in agreement with the [no-signalling theorem](../../../../../quantum-no-signalling.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 59](../../paper-59-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
