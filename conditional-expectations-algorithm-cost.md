# Conditional expectations algorithm cost

↑ **Parent:** [Conditional expectations for maximum cut](conditional-expectations-for-maximum-cut.md)

Directly scanning all $m$ [edges](edge-of-a-graph.md) to evaluate each child of each of $n$ choices takes $O(nm+n)$ elementary operations, in [Big O notation](big-o-notation.md). There is a faster implementation. When assigning [vertex](vertex-graph-theory.md) $v$, let $d_0$ and $d_1$ count its already assigned [graph neighbours](neighbour-of-a-vertex.md) labelled zero and one. Contributions from [edges](edge-of-a-graph.md) not incident to $v$ are unchanged, and contributions from [edges](edge-of-a-graph.md) to unassigned [graph neighbours](neighbour-of-a-vertex.md) stay $1/2$ for either choice. Therefore

$$
q(P,v=0)-q(P,v=1)=d_1-d_0.
$$

Choose zero if $d_1\geq d_0$, otherwise one: put $v$ on the side with fewer already assigned [graph neighbours](neighbour-of-a-vertex.md). With [adjacency lists](adjacency-list.md), scanning each [vertex](vertex-graph-theory.md)'s list once costs $O(n+m)$ operations overall and uses $O(n+m)$ storage including the [graph](graph-split.md). These bounds count operations on labels and counters that fit in machine words of $O(\log(n+m+2))$ [bits](bit.md). Multiplying the [conditional expectation cut formula](conditional-expectation-cut-formula.md) by two also permits exact integer comparisons without rounding.

If $\operatorname{OPT}$ is the size of a [maximum cut](maximum-cut.md), then $\operatorname{OPT}\leq m$. The constructed [cut of a graph](cut-graph-theory.md) thus has size at least $m/2\geq\operatorname{OPT}/2$, an [approximation ratio](approximation-ratio.md) of $1/2$ in the maximization convention. The five-versus-six example illustrates the gap between this guarantee and exact optimization.

For a general [randomized algorithm](randomized-algorithm.md), the averaging proof alone does not establish efficient [derandomization](derandomization.md). One needs a polynomial number of commitments, an efficient way to find a suitable child at each step, and manageable representations and evaluation costs for the relevant [conditional expectations](conditional-expectation.md). Those evaluations can themselves be hard. Enumerating all completions verifies this small example, but would take exponentially many assignments as $n$ grows. The [polynomial-time algorithm](polynomial-time-algorithm.md) here comes from the local [conditional expectation cut formula](conditional-expectation-cut-formula.md), not from that enumeration.

## ↑ Ancestors (7)

1. [Conditional expectations for maximum cut](conditional-expectations-for-maximum-cut.md)
2. [Method of conditional probabilities](method-of-conditional-probabilities.md)
3. [Derandomization](derandomization.md)
4. [Randomized algorithm](randomized-algorithm.md)
5. [Algorithm](algorithm-split.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)
