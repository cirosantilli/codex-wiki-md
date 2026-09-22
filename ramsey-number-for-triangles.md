# Ramsey number for triangles

↑ **Parent:** [Ramsey number](ramsey-number.md)

Every red-blue [edge coloring](edge-coloring.md) of the [complete graph](complete-graph.md) $K_6$ contains a [monochromatic](monochromatic-set.md) [triangle in a graph](triangle-in-a-graph.md), and some coloring of $K_5$ contains none. Together the [five-cycle Ramsey coloring](five-cycle-ramsey-coloring.md) and [six-vertex monochromatic triangle argument](six-vertex-monochromatic-triangle-argument.md) give

$$
5<R(3,3)\leq6,\qquad R(3,3)=6.
$$

The threshold is exact: one carefully chosen coloring establishes the lower bound, while the upper bound must handle every coloring.

A familiar interpretation uses six people and colors each pair red if they know one another and blue if they do not. Assuming the relation is symmetric and every pair falls into exactly one case, there are either three mutual acquaintances or three mutual strangers. The conclusion concerns all three pairs within the group, not merely two relationships through a common person. There is no prediction about which color wins or which three people form the group.

The small size makes exhaustive verification practical. The [complete graph](complete-graph.md) $K_5$ has $\binom52=10$ [edges](edge-of-a-graph.md), giving $2^{10}=1024$ red-blue colorings of labeled [vertices](vertex-graph-theory.md); exactly 12 have no [monochromatic](monochromatic-set.md) [triangle in a graph](triangle-in-a-graph.md). They are the choices of a red [cycle graph](cycle-graph.md) of length five, whose blue [complement graph](complement-graph.md) is another five-cycle. The [complete graph](complete-graph.md) $K_6$ has $\binom62=15$ [edges](edge-of-a-graph.md), giving $2^{15}=32768$ colorings. Checking all $\binom63=20$ triples in every coloring finds none without a [monochromatic](monochromatic-set.md) [triangle in a graph](triangle-in-a-graph.md); in fact the minimum number is two. These counts can be reproduced by assigning one [bit](bit.md) to each [unordered pair](unordered-pair.md) and testing whether the three [bits](bit.md) of each triple agree. The [monochromatic-triangle counting formula](monochromatic-triangle-counting-formula.md) gives a separate explanation of the stronger minimum-two conclusion.

**Table of contents**

- [Five-cycle Ramsey coloring](five-cycle-ramsey-coloring.md)
- [Six-vertex monochromatic triangle argument](six-vertex-monochromatic-triangle-argument.md)

## ↑ Ancestors (8)

1. [Ramsey number](ramsey-number.md)
2. [Finite Ramsey theorem](finite-ramsey-theorem.md)
3. [Ramsey's theorem](ramsey-s-theorem.md)
4. [Ramsey theory](ramsey-theory-split.md)
5. [Combinatorics](combinatorics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Finite Ramsey theorem](finite-ramsey-theorem.md)
- [Five-cycle Ramsey coloring](five-cycle-ramsey-coloring.md)
- [Ramsey number](ramsey-number.md)
- [Ramsey theory](ramsey-theory-split.md)
- [Six-vertex monochromatic triangle argument](six-vertex-monochromatic-triangle-argument.md)
