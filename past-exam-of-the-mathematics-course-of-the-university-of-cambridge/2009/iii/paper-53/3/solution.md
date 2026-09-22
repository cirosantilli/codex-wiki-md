<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Write $a=|\alpha|^2$, $b=|\beta|^2=1-a$, so $1/2<a<1$ and $0<b<1/2$. Regrouping the four copies by party gives

$$
|\Psi\rangle=\sum_{x\in\{0,1\}^4}\alpha^{z(x)}\beta^{4-z(x)}|x\rangle_A|x\rangle_B,
$$

where $z(x)$ counts zeroes. Alice must measure only this count, preserving coherence inside each degenerate [eigenspace](../../../../../eigenspace.md), rather than measuring her four bits separately. Her [projective measurement](../../../../../projective-measurement.md) has projectors $\Pi_k=\sum_{z(x)=k}|x\rangle\langle x|$, and the [Born rule](../../../../../born-rule.md) gives

$$
\boxed{p_k=\binom4k a^k b^{4-k},\qquad k=0,1,2,3,4.}
$$

Alice sends $k$ to Bob. Up to the common phase of $\alpha^k\beta^{4-k}$, their conditional [pure state](../../../../../pure-state.md) is

$$
|T_k\rangle=\frac1{\sqrt{d_k}}\sum_{z(x)=k}|x\rangle_A|x\rangle_B,\qquad d_k=\binom4k.
$$

This is [Schmidt projection entanglement concentration](../../../../../schmidt-projection-entanglement-concentration.md): its equal [Schmidt coefficients](../../../../../schmidt-coefficient.md) give a [maximally entangled state](../../../../../maximally-entangled-state.md) of [Schmidt rank](../../../../../schmidt-rank.md) $d_k$.

For $k=0$ or $4$, $d_k=1$, and the branch is a [product state](../../../../../product-state.md). No [Bell pair](../../../../../bell-pair.md) can be extracted using [local operations and classical communication](../../../../../local-operations-and-classical-communication.md). The respective [probabilities](../../../../../probability.md) are $b^4$ and $a^4$.

For $k=1$ or $3$, $d_k=4$. List the four surviving strings in lexicographic order as $x_0,x_1,x_2,x_3$. For $k=1$ this list is $0111,1011,1101,1110$; for $k=3$ it is $0001,0010,0100,1000$. Each party applies a [local unitary operation](../../../../../local-unitary-operation.md) extending the basis relabelling

$$
|x_j\rangle\longmapsto |j_1j_0\rangle\otimes|00\rangle,\qquad j=2j_1+j_0.
$$

Such a unitary exists because these are four distinct [orthonormal](../../../../../orthonormal-set.md) basis vectors mapped to four distinct basis vectors; extend the mapping to a permutation of all sixteen. Discarding the two fixed local ancillary bits leaves

$$
\frac12\sum_{j_1,j_0=0}^1|j_1j_0\rangle_A|j_1j_0\rangle_B
=|\Phi^+\rangle_{A_1B_1}\otimes|\Phi^+\rangle_{A_0B_0}.
$$

Thus these branches give exactly two [Bell pairs](../../../../../bell-pair.md), with [probabilities](../../../../../probability.md) $4ab^3$ and $4a^3b$, and no further [measurement in quantum mechanics](../../../../../quantum-measurement-split.md) is needed.

For $k=2$, the six strings in lexicographic order are $x_0=0011$, $x_1=0101$, $x_2=0110$, $x_3=1001$, $x_4=1010$, $x_5=1100$. A suitable local [POVM](../../../../../positive-operator-valued-measure.md) gives two [Bell pairs](../../../../../bell-pair.md) with certainty, rather than losing some of these branches to a simple subspace projection. Partition these labels into the three pairs $T_0=\{0,1\}$, $T_1=\{2,3\}$, $T_2=\{4,5\}$. Alice uses the [Kraus operators](../../../../../kraus-operator.md)

$$
K_r=\frac1{\sqrt2}\sum_{j\notin T_r}|x_j\rangle\langle x_j|,\qquad r=0,1,2.
$$

On the six-dimensional support, each label is retained by two operators, so $\sum_{r=0}^2K_r^\dagger K_r=\Pi_2$. Add $K_\perp=I-\Pi_2$ to define a complete [measurement in quantum mechanics](../../../../../quantum-measurement-split.md) on Alice's four qubits; that extra outcome has [probability](../../../../../probability.md) zero on this branch. Each nonzero outcome has conditional [probability](../../../../../probability.md) $(1/2)(4/6)=1/3$, and gives the normalized state

$$
\frac12\sum_{j\notin T_r}|x_j\rangle_A|x_j\rangle_B.
$$

Alice sends $r$ to Bob. Both parties relabel the four surviving strings in increasing order to $|00\rangle,|01\rangle,|10\rangle,|11\rangle$ on two output qubits, with two fixed ancillary bits, just as above. Every $r$ therefore gives two [Bell pairs](../../../../../bell-pair.md). The joint [probability](../../../../../probability.md) of $(k,r)=(2,r)$ is $p_2/3=2a^2b^2$ for each $r$.

For an explicit local implementation of this [POVM](../../../../../positive-operator-valued-measure.md), Alice can append an ancilla in a fixed state and apply an isometry on the six-dimensional support,

$$
|x_j\rangle\longmapsto |x_j\rangle\otimes\frac1{\sqrt2}\sum_{r:\,j\notin T_r}|r\rangle.
$$

It preserves inner products, extends to a unitary on system and ancilla, and measuring the ancilla realizes precisely the operators $K_r$. No nonlocal operation has been used. This is a [deterministic reduction of maximally entangled Schmidt rank](../../../../../deterministic-reduction-of-maximally-entangled-schmidt-rank.md) from six to four.

The complete output distribution for this strategy is consequently

$$
\boxed{\Pr(2\text{ Bell pairs})=1-a^4-b^4,\qquad \Pr(0\text{ Bell pairs})=a^4+b^4.}
$$

The mean yield is $2(1-a^4-b^4)$ pairs per four-copy block. These are the maximum possible pair counts after the stipulated count measurement: any nonzero branch has [Schmidt rank](../../../../../schmidt-rank.md) at most six, whereas three independent [Bell pairs](../../../../../bell-pair.md) require [Schmidt rank](../../../../../schmidt-rank.md) eight. In any refined [LOCC](../../../../../local-operations-and-classical-communication.md) branch the coefficient matrix is multiplied by local matrices on the left and right, which cannot increase its [rank](../../../../../rank-one-quadratic-form.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 53](../../paper-53-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
