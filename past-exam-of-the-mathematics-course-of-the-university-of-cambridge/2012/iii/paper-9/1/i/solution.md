<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $d=np=\gamma\log n$ and $\mu=n^{1-\gamma}$. The hypothesis implies $\mu\geq e^{\omega(n)}\to\infty$. For the number $I$ of [isolated vertices](../../../../../../isolated-vertex.md), the [isolated vertices in the Erdős-Rényi model](../../../../../../isolated-vertices-in-the-erdos-renyi-model.md) formulas give

$$
\mathbb EI=n(1-p)^{n-1}=(1+o(1))\mu,\qquad
\frac{\operatorname{var}I}{(\mathbb EI)^2}\leq\frac1{\mathbb EI}+\frac p{1-p}=o(1).
$$

Thus the [Chebyshev inequality](../../../../../../chebyshev-inequality.md) gives $I=(1+o(1))\mu$ [with high probability](../../../../../../with-high-probability.md), uniformly over the specified $\gamma$ range.

The [Cayley formula](../../../../../../cayley-s-formula.md) supplies a [spanning tree](../../../../../../spanning-tree.md) on any connected vertex set. Consequently the [expected value](../../../../../../expected-value.md) $C_j$ of the number of [graph components](../../../../../../component-graph-theory.md) of order $j\geq2$ is bounded by

$$
\mathbb EC_j\leq\binom nj j^{j-2}p^{j-1}(1-p)^{j(n-j)}.
$$

Choose a fixed $\eta\in(0,1/2)$ with $\gamma_0(1-\eta)(k+1)>1$. For $k+1\leq j\leq\eta n$, with $j\geq2$, the [binomial coefficient](../../../../../../binomial-coefficient.md) bound $\binom nj\leq(en/j)^j$ gives

$$
\mathbb EC_j\leq\frac n{d j^2}\left(ed\,e^{-d(1-\eta)}\right)^j.
$$

Here $ed\,e^{-d(1-\eta)}\leq e\log n\,n^{-\gamma_0(1-\eta)}\to0$. The [geometric series](../../../../../../geometric-series.md) and a [union bound](../../../../../../boole-s-inequality.md) therefore exclude this entire size range, since $n[ e\log n\,n^{-\gamma_0(1-\eta)}]^{k+1}=o(1)$. For $\eta n\leq j\leq n/2$, an empty [graph cut](../../../../../../graph-cut.md) would be necessary. Its total [probability](../../../../../../probability.md) is at most

$$
2^n e^{-p\eta n^2/2}=o(1).
$$

There are consequently no [graph components](../../../../../../component-graph-theory.md) of orders between $k+1$ and $n/2$, [with high probability](../../../../../../with-high-probability.md).

For each fixed $2\leq j\leq k$, a [graph component](../../../../../../component-graph-theory.md) containing a [graph cycle](../../../../../../cycle-in-a-graph.md) has a [spanning tree](../../../../../../spanning-tree.md) and at least one extra [edge](../../../../../../edge-of-a-graph.md). Counting that extra [edge](../../../../../../edge-of-a-graph.md) gives an [expected value](../../../../../../expected-value.md) $O_k(d^j e^{-dj})=o(1)$; hence every small [graph component](../../../../../../component-graph-theory.md) is a [tree component](../../../../../../tree-component.md). The total number $R_2$ of [vertices](../../../../../../vertex-graph-theory.md) in [tree components](../../../../../../tree-component.md) of orders $2,\ldots,k$ satisfies

$$
\mathbb ER_2=O_k\left(n d e^{-2d}\right)=O_k(\mu d e^{-d})=o(\mu).
$$

The [Markov inequality](../../../../../../markov-inequality.md) gives $R_2=o(\mu)$ [with high probability](../../../../../../with-high-probability.md). When $k=1$, this sum is empty and $R_2=0$. Since $\mu=o(n)$, the remaining [vertices](../../../../../../vertex-graph-theory.md) must lie in one [graph component](../../../../../../component-graph-theory.md) larger than $n/2$. It is unique, and its order is **$n-(1+o(1))n^{1-\gamma}$**. Every other [graph component](../../../../../../component-graph-theory.md) is a [tree](../../../../../../tree-graph-theory.md) with at most $k$ [vertices](../../../../../../vertex-graph-theory.md). This is the [logarithmic-regime giant component](../../../../../../logarithmic-regime-giant-component.md) mechanism: almost all missing [vertices](../../../../../../vertex-graph-theory.md) are isolated.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
