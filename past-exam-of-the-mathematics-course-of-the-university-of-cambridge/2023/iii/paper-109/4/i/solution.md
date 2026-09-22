<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Choose a [Uniformly random maximal chain in a Boolean lattice](../../../../../../uniformly-random-maximal-chain-in-a-boolean-lattice.md). A fixed $h$-element set lies on the chain with probability $\binom nh^{-1}$. Since an [antichain](../../../../../../antichain.md) meets any chain at most once, the expected number of its members on the chain is at most one:

$$
\sum_{h=0}^n|\mathcal A_h|\binom nh^{-1}\leq1.
$$

This is the [Lubell-Yamamoto-Meshalkin inequality](../../../../../../lubell-yamamoto-meshalkin-inequality.md).

For the equality case, every maximal chain must meet $\mathcal A$. Suppose $S\in\mathcal A$ has size $h$ and $T$ is obtained from $S$ by exchanging one element. There is a maximal chain whose rank-$h$ member is $T$, whose rank-$(h-1)$ member is $S\cap T$, and whose rank-$(h+1)$ member is $S\cup T$. Every lower member is contained in $S$ and every higher member contains $S$, so antichainness excludes all of them. Equality forces $T\in\mathcal A$. The graph of $h$-subsets joined by one-element exchanges is connected, hence $\mathcal A=[n]^{(h)}$. Conversely, a full level clearly gives equality.

Since $\binom nh\leq\binom n{\lfloor n/2\rfloor}$,

$$
\frac{|\mathcal A|}{\binom n{\lfloor n/2\rfloor}}
\leq\sum_h|\mathcal A_h|\binom nh^{-1}\leq1.
$$

The equality characterization above leaves exactly either middle level. This proves [Sperner theorem](../../../../../../sperner-s-theorem.md) with its equality cases.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
