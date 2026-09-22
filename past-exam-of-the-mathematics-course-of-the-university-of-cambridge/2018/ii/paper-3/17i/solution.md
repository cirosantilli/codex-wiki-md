<h1 id="17i/solution">Solution</h1>

↑ **Parent:** [17I](../17i.md)

A $k$-colouring assigns one of $k$ colours to every vertex so that adjacent vertices have different colours. The [chromatic number](../../../../../chromatic-number.md) $\chi(G)$ is the least such $k$. An [independent set](../../../../../independent-set-graph-theory.md) contains no adjacent pair, and the [independence number](../../../../../independence-number.md) $\alpha(G)$ is the maximum size of such a set.

For a concrete first example, start with the five-cycle $C_5$ and apply the [Mycielski construction](../../../../../mycielskian.md) $r-2$ times. Each application raises the chromatic number by one and preserves triangle-freeness. The resulting graph has chromatic number $r+1>r$ and contains no triangle, hence no [complete graph](../../../../../complete-graph.md) $K_r$ for $r\geq3$.

We next prove the stronger high-[girth](../../../../../girth.md) assertion by the [probabilistic method](../../../../../probabilistic-method.md). For a large integer $n$, take

$$
G\sim G(n,p),\qquad p=n^{-1+1/(2g)}.
$$

If $X$ counts cycles of lengths $3,\ldots,g$, then

$$
\mathbb EX
\leq\sum_{j=3}^g\frac{n^jp^j}{2j}
=O\left((np)^g\right)
=O(n^{1/2}).
$$

By the [first moment method](../../../../../first-moment-method.md), with probability tending to one $X<n/2$.

Let $m=\lfloor n/(2k)\rfloor$. The expected number of independent sets of size $m$ is at most

$$
\binom nm(1-p)^{\binom m2}
\leq
\left(\frac{en}{m}\right)^m
\exp\left(-\frac{pm(m-1)}2\right)
\longrightarrow0,
$$

because $pm^2=\Theta(n^{1+1/(2g)})$ dominates $m\log(en/m)=O(n)$. Hence with positive probability $G$ has fewer than $n/2$ short cycles and $\alpha(G)<m$.

Delete one vertex from each cycle of length at most $g$. The remaining graph $H$ has no such cycle, has at least $n/2$ vertices, and still has $\alpha(H)<n/(2k)$. Since each colour class is independent,

$$
\boxed{\chi(H)\geq\frac{|V(H)|}{\alpha(H)}\geq k.}
$$

This proves that there are [graphs of arbitrarily high girth and chromatic number](../../../../../graphs-of-arbitrarily-high-girth-and-chromatic-number.md).

For the final claim, begin instead with

$$
G\sim G(N,p),\qquad N=2n,\qquad p=N^{-0.69}.
$$

The expected number $T$ of triangles is

$$
\mathbb ET=\binom N3p^3=O(N^{0.93})=o(n),
$$

so with probability tending to one $T<n$. Put $m=\lceil n^{0.7}\rceil$. The expected number of independent $m$-sets is bounded by

$$
\binom Nm(1-p)^{\binom m2}
\leq\exp\left(
m\log\frac{eN}{m}-\frac{pm(m-1)}2
\right)\longrightarrow0,
$$

because the positive term is $O(n^{0.7}\log n)$ whereas the negative term has order $n^{0.71}$.

Thus some such $G$ has fewer than $n$ triangles and no independent set of size $m$. Delete one vertex from every triangle; more than $n$ vertices remain and the graph is triangle-free. Take any induced subgraph on exactly $n$ vertices. Vertex deletion cannot increase the [independence number](../../../../../independence-number.md), so the resulting graph satisfies

$$
\boxed{\alpha(G)<n^{0.7}.}
$$

This is the [triangle-free graph with sub-power independence number](../../../../../triangle-free-graph-with-sub-power-independence-number.md) construction.

## ↑ Ancestors (10)

1. [17I](../17i.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
