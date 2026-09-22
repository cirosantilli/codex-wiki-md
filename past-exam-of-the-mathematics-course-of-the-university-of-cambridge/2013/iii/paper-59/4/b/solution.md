<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $N=\binom n2$ be the number of independent undirected-edge bits; use unordered pairs $i<j$. The paper's [common-center graph property](../../../../../../common-center-graph-property.md) means that all present edges share a vertex. Isolated vertices are allowed, and the empty [graph](../../../../../../graph-split.md) satisfies the property. This convention matters in the count.

The empty [graph](../../../../../../graph-split.md) contributes $+1$ to the alternating sum. The $N$ one-edge [graphs](../../../../../../graph-split.md) contribute $-N$. A [graph](../../../../../../graph-split.md) with at least two edges and a common center has a unique center, since two different edges have just that common endpoint. For a fixed center, its possible edge sets are subsets of the $n-1$ incident edges. Their contribution after removing sets of size zero and one is

$$
\sum_{k=2}^{n-1}(-1)^k\binom{n-1}{k}
=(1-1)^{n-1}-1+(n-1)=n-2.
$$

These [graphs](../../../../../../graph-split.md) are counted once for each of their unique centers. Thus the [alternating count of common-center graphs](../../../../../../alternating-count-of-common-center-graphs.md) is

$$
\boxed{\sum_G(-1)^{|E(G)|}\mathrm{STAR}_n(G)
=1-\binom n2+n(n-2)=\frac{(n-1)(n-2)}2\ne0\quad(n\geq3)}.
$$

Part (a) gives $D(\mathrm{STAR}_n)\geq N$, while querying all $N$ bits always suffices. Therefore

$$
\boxed{D(\mathrm{STAR}_n)=\binom n2;\quad\mathrm{STAR}_n\text{ is evasive}}.
$$

The relevant input length is $N$, not the number $n$ of [graph](../../../../../../graph-split.md) vertices.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
