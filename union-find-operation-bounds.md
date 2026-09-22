# Union-find operation bounds

↑ **Parent:** [Disjoint-set data structure](disjoint-set-data-structure.md)

Assume identifiers, pointers and ranks fit into constant-size [machine words](machine-word.md), with constant-cost indexed [array](array-data-structure.md) access, comparison and assignment. Initializing $n\geq1$ members costs $O(n)$ time and [machine words](machine-word.md). With [union by rank](union-by-rank.md) and full [path compression](path-compression.md), any [sequence](sequence.md) of $m$ [disjoint-set find operations](disjoint-set-find-operation.md) and [disjoint-set union operations](disjoint-set-union-operation.md) then has total [time complexity](time-complexity.md), in [Big O notation](big-o-notation.md),

$$
O\bigl(n+m\alpha(n)\bigr).
$$

Here $\alpha(n)\geq1$ is a conventionally normalized [inverse Ackermann function](inverse-ackermann-function.md). The documented path-halving implementation has the same [amortized analysis](amortized-analysis.md) bound.[Algorithms, 4th edition by Robert Sedgewick and others; UF.java, class documentation: linear constructor, logarithmic worst-case operations and inverse-Ackermann sequence bound for rank with halving](algorithms-4th-edition-by-robert-sedgewick-and-others/uf-java.md)

A [disjoint-set union operation](disjoint-set-union-operation.md) includes two [disjoint-set find operations](disjoint-set-find-operation.md) and a constant amount of additional linking work. Including $n$ in the bound accounts for initialization even if no queries follow.

This is a bound on an entire [sequence](sequence.md). It is not a worst-case constant bound for each call: a [disjoint-set find operation](disjoint-set-find-operation.md) can still encounter a previously uncompressed route of logarithmic length. The [inverse Ackermann function](inverse-ackermann-function.md) grows extraordinarily slowly but is unbounded, so it cannot be replaced by a mathematical constant in this asymptotic statement. The general distinction between a per-operation maximum and a whole-[sequence](sequence.md) guarantee is explained in [amortized analysis](amortized-analysis.md).

[Robert Tarjan](robert-tarjan.md)'s 1975 paper established an [inverse Ackermann function](inverse-ackermann-function.md) bound for set union. Its abstract states the sharper two-parameter form for $m\geq n$ representative queries and $n-1$ intermixed merges: the worst total cost is bounded above and below by positive constant multiples of $m\alpha(m,n)$. Those variables count different operations from the convenient $n+m\alpha(n)$ formulation above; the abstract's matching lower bound is about its analyzed method, rather than a claim that every conceivable representation obeys the same lower bound.[Efficiency of a Good But Not Linear Set Union Algorithm, Journal of the ACM 22(2), April 1975, pp. 215–225, DOI 10.1145/321879.321884; abstract reproduced in Princeton's publication record](efficiency-of-a-good-but-not-linear-set-union-algorithm-by-robert-endre-tarjan.md)

The intuition is that [union by rank](union-by-rank.md) limits how parent routes grow, while [path compression](path-compression.md) makes an expensive traversal improve later queries. The rank argument alone proves only a logarithmic bound. Establishing the [inverse Ackermann function](inverse-ackermann-function.md) bound requires a finer accounting of traversals across rank ranges; it does not follow merely from drawing a flatter [rooted tree](rooted-tree.md). The useful result is that repeated merging and membership queries can share the work of maintaining a changing [partition of a set](partition-of-a-set.md).

## ↑ Ancestors (4)

1. [Disjoint-set data structure](disjoint-set-data-structure.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)
