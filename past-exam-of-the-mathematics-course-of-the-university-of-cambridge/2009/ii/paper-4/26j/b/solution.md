<h1 id="26j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The second [continuous-time Markov chain](../../../../../../continuous-time-markov-chain.md) runs in the reverse direction at rate $\rho$, as in the right diagram. Its nonzero [eigenvalues](../../../../../../eigenvalue.md) have real part $-3\rho/2$, and its [transition probabilities](../../../../../../transition-probability.md) tend to $1/3$ for each vertex. [Independence](../../../../../../independent-random-variables.md) therefore gives

$$
p(t)=\sum_{v=A,B,C}P(X_t=v)P(Y_t=v)\longrightarrow3\left(\frac13\right)^2.
$$

Thus **the limit exists for every pair of starting vertices and equals $\boxed{1/3}$**.

One can also see the limit directly without spectral multiplication. For fixed starting vertices, $X_t-Y_t$ modulo three advances with each jump of either flea. Its jump count is the sum of independent [Poisson processes](../../../../../../poisson-process.md) with rates $1$ and $\rho$, hence is Poisson with rate $1+\rho$ (multiply their generating functions). The formula from part (a), with $t$ replaced by $(1+\rho)t$ and the appropriate initial residue, gives $p(t)$ and the same limit.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [26J](../../26j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
