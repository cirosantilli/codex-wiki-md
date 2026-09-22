<h1 id="11k/solution">Solution</h1>

↑ **Parent:** [11K](../11k.md)

Take every logarithm in base two. The [information entropy](../../../../../information-entropy.md) of $X$ is

$$
\boxed{H(X)=-\sum_{i=1}^Np_i\log_2p_i},
$$

with $0\log_20=0$. If the codeword $c(\mu_i)$ has length $s_i$, then its [expected codeword length](../../../../../expected-codeword-length.md) is

$$
\boxed{\mathbb E(S)=\sum_{i=1}^Np_is_i}.
$$

For any [decipherable code](../../../../../decipherable-code.md), the [Kraft inequality](../../../../../kraft-mcmillan-inequality.md) gives

$$
K=\sum_{i=1}^N2^{-s_i}\leq1.
$$

Define the [probability distribution](../../../../../probability-distribution.md) $q_i=2^{-s_i}/K$. By [Gibbs inequality](../../../../../gibbs-inequality.md),

$$
0\leq\sum_i p_i\log_2\frac{p_i}{q_i}
=-H(X)+\mathbb E(S)+\log_2K.
$$

Since $\log_2K\leq0$,

$$
\mathbb E(S)\geq H(X)-\log_2K\geq H(X).
$$

Conversely, choose the integer lengths

$$
s_i=\lceil-\log_2p_i\rceil.
$$

Then $2^{-s_i}\leq p_i$, so their Kraft sum is at most one and the converse part of Kraft's inequality supplies a binary [prefix code](../../../../../prefix-code.md). Moreover,

$$
\mathbb E(S)
=\sum_i p_i\lceil-\log_2p_i\rceil
<\sum_i p_i(-\log_2p_i+1)
=H(X)+1.
$$

Thus the minimum expected length $S^*$ satisfies the [Shannon noiseless coding theorem](../../../../../shannon-s-source-coding-theorem.md)

$$
\boxed{H(X)\leq S^*<H(X)+1}.
$$

For a decipherable code with arbitrary lengths $s_1,\ldots,s_N$, apply the lower bound to the uniform source $p_i=1/N$. Its entropy is $\log_2N$ and its expected length is $(s_1+\cdots+s_N)/N$. Hence

$$
\boxed{N\log_2N\leq s_1+\cdots+s_N},
$$

the [total length lower bound for a decipherable binary code](../../../../../total-length-lower-bound-for-a-decipherable-binary-code.md).

Now consider the cumulative construction. Since

$$
b_j-b_i=\sum_{k=i}^{j-1}p_k\geq p_i\geq2^{-s_i}
\qquad(j>i),
$$

$b_i$ and $b_j$ cannot have the same first $s_i$ binary digits: numbers sharing those digits lie in one half-open dyadic interval of length $2^{-s_i}$. Also, $p_i\geq p_j$ implies $s_i\leq s_j$. Therefore no earlier codeword $b_i^*$ is a prefix of a later one, and no later, weakly longer codeword can be a prefix of an earlier one. The [cumulative Shannon code](../../../../../cumulative-shannon-code.md) is thus a [prefix code](../../../../../prefix-code.md), hence decipherable.

An optimal code minimizes [expected codeword length](../../../../../expected-codeword-length.md) over all decipherable codes for the specified source probabilities. The cumulative construction need not be optimal. For example, if

$$
(p_1,p_2)=(0.6,0.4),
$$

then $(s_1,s_2)=(1,2)$ and the construction gives codewords $0$ and $10$, with expected length $1.4$. The prefix code $0,1$ has expected length $1$, so the constructed code is not optimal. In general, [Huffman coding](../../../../../huffman-coding.md) produces an optimal prefix code.

## ↑ Ancestors (10)

1. [11K](../11k.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
