<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $q=1-p$. A disconnected [graph](../../../../../../graph-split.md) has a [connected component of a graph](../../../../../../component-graph-theory.md) of size $1\leq s\leq\lfloor n/2\rfloor$. For a fixed $s$-element [vertex set](../../../../../../vertex-set.md) $S$, all $s(n-s)$ [edges](../../../../../../edge-of-a-graph.md) between $S$ and its complement must be absent. Their independent absence has probability $q^{s(n-s)}$. The [union bound](../../../../../../boole-s-inequality.md) gives

$$
\mathbb P(G(n,p)\text{ disconnected})
\leq\sum_{s=1}^{\lfloor n/2\rfloor}\binom ns q^{s(n-s)}
\leq\boxed{\sum_{s=1}^{\lfloor n/2\rfloor}
\left(nq^{n/2}\right)^s}.
$$

Set $r_n=nq^{n/2}$. Since $p$ is fixed in $(0,1)$, $r_n\to0$. For large $n$, the final sum is at most the [geometric series](../../../../../../geometric-series.md) $r_n/(1-r_n)$, which tends to zero. Hence the [binomial random graph](../../../../../../binomial-random-graph.md) is [connected](../../../../../../connected-space.md) with probability tending to one, as in [connectivity of a fixed-density binomial random graph](../../../../../../connectivity-of-a-fixed-density-binomial-random-graph.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
