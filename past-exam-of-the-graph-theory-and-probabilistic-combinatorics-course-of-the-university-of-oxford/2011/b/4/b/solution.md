<h1 id="b/4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $X$ count the four-vertex [sets](../../../../../set-split.md) spanning all four of their possible triples. For each such [set](../../../../../set-split.md) $S$, write $I_S$ for its [indicator](../../../../../indicator-function.md). [Independence](../../../../../independent-random-variables.md) of the four [hyperedges](../../../../../hyperedge.md) gives

$$
\mu=\mathbb E X=\binom n4p^4.
$$

If $np\to0$, then $\mu\leq (np)^4/24\to0$, and the [first moment method](../../../../../first-moment-method.md) shows that the [probability](../../../../../probability.md) of a four-clique tends to zero.

For the other direction, consider two distinct four-sets. If they meet in at most two [vertices](../../../../../vertex-graph-theory.md), they have no possible triple in common, so their indicators are [independent](../../../../../independent-random-variables.md). If they meet in three [vertices](../../../../../vertex-graph-theory.md), they share exactly one triple, so $\mathbb E(I_SI_T)=p^7$ and their [covariance](../../../../../covariance.md) is at most $p^7$. There are $O(n^5)$ ordered pairs of this latter type. The diagonal variances sum to at most $\mu$, hence

$$
\operatorname{Var}(X)\leq\mu+O(n^5p^7).
$$

For large $n$, $\mu$ is a [constant](../../../../../constant-mathematics.md) multiple of $n^4p^4$, and consequently

$$
\frac{\operatorname{Var}(X)}{\mu^2}
=O\left(\frac1{n^4p^4}+\frac1{n^3p}\right).
$$

If $np\to\infty$, the first term tends to zero, and so does the second since $n^3p=n^2(np)\to\infty$. The [second moment method](../../../../../second-moment-method.md) proves that a four-clique exists with [probability](../../../../../probability.md) tending to one. Therefore a [threshold function](../../../../../threshold-function.md) is

$$
\boxed{p^*(n)=n^{-1}.}
$$

The shared-triple overlap, rather than overlaps in one or two [vertices](../../../../../vertex-graph-theory.md), is the only off-diagonal dependence that affects this computation.

This is the [four-clique threshold in a binomial 3-uniform hypergraph](../../../../../four-clique-threshold-in-a-binomial-3-uniform-hypergraph.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
