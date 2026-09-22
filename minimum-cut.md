# Minimum cut

↑ **Parent:** [Cut of a flow network](cut-of-a-flow-network.md)

A [minimum cut](minimum-cut.md) is a [cut of a flow network](cut-of-a-flow-network.md) of least [cut capacity](cut-capacity.md) for the prescribed source $s$ and sink $t$. The [max-flow min-cut theorem](max-flow-min-cut-theorem.md) equates that least [cut capacity](cut-capacity.md) with the greatest [flow value](strength-of-a-flow.md).[Graph Theory by Reinhard Diestel; Diestel, Flows, §6.2, Theorem 6.2.2, printed p. 159](graph-theory-by-reinhard-diestel/flows-author-hosted-chapter-preview.md)

To certify a particular [minimum cut](minimum-cut.md), exhibit a [feasible flow](feasible-flow.md) whose [flow value](strength-of-a-flow.md) equals its [cut capacity](cut-capacity.md). Every [feasible flow](feasible-flow.md) is bounded above by every [cut capacity](cut-capacity.md), so this single equality proves both optimalities.[Algorithms, 4th edition by Robert Sedgewick and others; Sedgewick and Wayne, FordFulkerson.java, check method, lines 180–209: feasibility, source/sink membership and equality of values](algorithms-4th-edition-by-robert-sedgewick-and-others/fordfulkerson-java.md)

In the running example, the four possible source sides $\{s\}$, $\{s,a\}$, $\{s,b\}$ and $\{s,a,b\}$ have [cut capacities](cut-capacity.md) $5,5,6,5$, respectively. The [feasible flow](feasible-flow.md) of [flow value](strength-of-a-flow.md) $5$ therefore certifies three different [minimum cuts](minimum-cut.md). A [minimum cut](minimum-cut.md) need not be unique; the optimum [cut capacity](cut-capacity.md) is the same for all of them. Merely saturating many [edges](edge-of-a-graph.md) does not give this certificate: [flow conservation](flow-conservation.md) and the particular [cut of a flow network](cut-of-a-flow-network.md) must also be checked.

**Table of contents**

- [Diagonal cut in a nearest-neighbour lattice flow](diagonal-cut-in-a-nearest-neighbour-lattice-flow.md)

## ↑ Ancestors (7)

1. [Cut of a flow network](cut-of-a-flow-network.md)
2. [Flow network](flow-network-split.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Cut capacity](cut-capacity.md)
- [Max-flow min-cut theorem](max-flow-min-cut-theorem.md)
- [Minimum cut](minimum-cut.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-35/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ib/paper-2/9h/solution.md)
