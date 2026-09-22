<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

First suppose $L\in\mathbf{RP}\cap\mathbf{co\text{-}RP}$. Run the RP algorithm for $L$ and the RP algorithm for its complement with fresh random bits. If the first accepts, output one; if the second accepts, output zero; otherwise repeat. Neither output can be wrong, and on every input the appropriate algorithm accepts in each round with probability at least $1/2$. The number of rounds is dominated by a [geometric distribution](../../../../../../geometric-distribution.md) of mean two, so this is an always-correct algorithm with polynomial [expected running time](../../../../../../expected-value.md).

Conversely, let $T$ be always correct when it halts and have expected running time at most $p(n)$. Run it for $2p(n)$ steps. [Markov inequality](../../../../../../markov-inequality.md) gives

$$
\mathbb P(T\text{ has not halted by }2p(n))\leq\frac12.
$$

Accept exactly when $T$ halts and outputs one; this is an RP algorithm for $L$. Accepting exactly when it halts and outputs zero is an RP algorithm for the complement. Therefore

$$
\boxed{\mathbf{ZPP}=\mathbf{RP}\cap\mathbf{co\text{-}RP}}
$$

is equivalent to zero-error expected polynomial time.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
