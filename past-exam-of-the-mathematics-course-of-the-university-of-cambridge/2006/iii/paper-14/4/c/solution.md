<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [connected graph](../../../../../../connected-graph.md) with $n>1$ has no [isolated vertices](../../../../../../isolated-vertex.md). Conversely, a disconnected [graph](../../../../../../graph-split.md) with no [isolated vertices](../../../../../../isolated-vertex.md) has a [connected component](../../../../../../connected-component.md) with size between $2$ and $n/2$. We must show that this latter event has [probability](../../../../../../probability.md) tending to zero.

The permitted component-size estimate excludes sizes between $\log\log n$ and $n/2$ [with high probability](../../../../../../with-high-probability.md). For the remaining small sizes, let $C_k$ count components with $k$ vertices. A [connected graph](../../../../../../connected-graph.md) on a fixed $k$-vertex set contains a [spanning tree](../../../../../../spanning-tree.md). By the [Cayley formula](../../../../../../cayley-s-formula.md), there are $k^{k-2}$ labelled [trees](../../../../../../tree-graph-theory.md), as follows from the [Prüfer code](../../../../../../prufer-sequence.md) [bijection](../../../../../../bijection.md) between labelled [trees](../../../../../../tree-graph-theory.md) and sequences of $k-2$ labels. A [union bound](../../../../../../boole-s-inequality.md) over the [trees](../../../../../../tree-graph-theory.md), together with the absence of every [edge](../../../../../../edge-of-a-graph.md) to the complementary [vertex set](../../../../../../vertex-set.md), gives

$$
\mathbb E C_k\leq\binom nk k^{k-2}p^{k-1}(1-p)^{k(n-k)}.
$$

Put $a=np=\log n+c$ and $L=\lceil\log\log n\rceil$. Using $\binom nk\leq(en/k)^k$ and $1-p\leq e^{-p}$, uniformly for $2\leq k\leq L$ we obtain

$$
\mathbb E C_k\leq\frac{n}{a k^2}\left(\frac{e^{1-c}a}{n}\right)^k e^{pk^2}.
$$

Here $pL^2\to0$. Therefore, with $\rho_n=e^{1-c}a/n\to0$,

$$
\sum_{k=2}^L\mathbb E C_k
\leq\frac{2n}{a}\sum_{k=2}^{\infty}\rho_n^k
=O(a/n)\longrightarrow0.
$$

The [Markov inequality](../../../../../../markov-inequality.md) excludes all these small components [with high probability](../../../../../../with-high-probability.md). Together with the permitted estimate, this proves that the difference between the [probability](../../../../../../probability.md) of connectivity and the [probability](../../../../../../probability.md) of no [isolated vertices](../../../../../../isolated-vertex.md) tends to zero. Hence

$$
\boxed{\mathbb P(G\text{ is connected})\longrightarrow e^{-e^{-c}}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 14](../../../paper-14-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
