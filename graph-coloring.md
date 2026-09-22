# Graph coloring

↑ **Parent:** [Graph theory](graph-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Graph_coloring)

A [graph coloring](graph-coloring.md) assigns labels called colours to elements of a [graph](graph-split.md), subject to specified constraints. Here we focus on [proper vertex colouring](proper-vertex-coloring.md) of a [simple graph](simple-graph.md) $G=(V,E)$: it is an [undirected graph](undirected-graph.md) with a [finite set](finite-set.md) of [vertices](vertex-graph-theory.md), and a colouring with at most $k$ colours is a [function](function-split.md)

$$
c:V\to\{1,\ldots,k\},\qquad \{u,v\}\in E\Longrightarrow c(u)\ne c(v).
$$

The colour labels need not be visual colours: they can represent time slots or resources. Unused labels are allowed. Properness concerns [graph adjacency](graph-adjacency.md), so moving [vertices](vertex-graph-theory.md) in a drawing does not change whether the [graph coloring](graph-coloring.md) is valid.[MIT, Graphs and Coloring, Section 2.1](https://ocw.mit.edu/courses/6-1200j-mathematics-for-computer-science-spring-2024/mit6_1200j_s24_lec11.pdf)

Each [colour class](colour-class.md) $c^{-1}(i)$ is an [independent set](independent-set-graph-theory.md): no [edge](edge-of-a-graph.md) has both endpoints in it. Conversely, a [set partition](set-partition.md) of $V$ into [independent sets](independent-set-graph-theory.md) gives a proper [graph coloring](graph-coloring.md) by assigning one colour to each part. Thus [graph coloring](graph-coloring.md) groups mutually compatible objects, and its [chromatic number](chromatic-number.md) asks for the fewest such groups.

For an illustrative scheduling model, let each [vertex](vertex-graph-theory.md) represent an activity of equal duration and each [edge](edge-of-a-graph.md) represent a pair that cannot occur in the same time slot. A proper [graph coloring](graph-coloring.md) is then a schedule respecting those pairwise conflicts. If the conflicts form a [cycle graph](cycle-graph.md) $C_4$ with [edges](edge-of-a-graph.md) $12,23,34,41$, activities $1,3$ can share one slot and $2,4$ another. This model assumes interchangeable slots and includes only the pairwise conflicts encoded by the [graph](graph-split.md).[Leighton, MIT Graph Theory and Coloring, transcript pages 8–10](https://ocw.mit.edu/courses/6-042j-mathematics-for-computer-science-fall-2010/1ccaf180bcd244fddd32e60789fa922f_h9wxtqoa1jY.pdf)

The word "colouring" also occurs in [edge coloring](edge-coloring.md), which requires different colours on [edges](edge-of-a-graph.md) sharing an endpoint. The [chromatic number](chromatic-number.md) discussed here always refers to [proper vertex colouring](proper-vertex-coloring.md).

**Table of contents**

- [Proper vertex coloring](proper-vertex-coloring.md)
- [Semi-random palette refinement for triangle-free colouring](semi-random-palette-refinement-for-triangle-free-colouring.md)
- [Colour savings from sparse neighbourhoods](colour-savings-from-sparse-neighbourhoods.md)
- [Coloring entropy weight](coloring-entropy-weight.md)
  - [Entropy weight of a graph cover](entropy-weight-of-a-graph-cover.md)
- [Greedy coloring](greedy-coloring.md)
  - [Extension of a partial colouring by neighbour-colour savings](extension-of-a-partial-colouring-by-neighbour-colour-savings.md)
    - [Neighbour-colour saving](neighbour-colour-saving.md)
- [Three-colourability problem](three-colourability-problem.md)
- [Three-colour clause gadget](three-colour-clause-gadget.md)
- [Boolean-pair colouring gadget](boolean-pair-colouring-gadget.md)
- [Greedy colouring by removing independent sets](greedy-colouring-by-removing-independent-sets.md)
- [Lovász number](lovasz-number.md)
  - [Orthonormal representation of a graph](orthonormal-representation-of-a-graph.md)
    - [Tensor-product capacity bound from an orthonormal representation](tensor-product-capacity-bound-from-an-orthonormal-representation.md)
  - [Complement theta number](complement-theta-number.md)
- [Vector coloring](vector-coloring.md)
  - [Strict vector coloring](strict-vector-coloring.md)
  - [Random hyperplane rounding](random-hyperplane-rounding.md)
- [Semicoloring](semicoloring.md)
  - [Semicoloring by independent hyperplanes](semicoloring-by-independent-hyperplanes.md)
- [Edge coloring](edge-coloring.md)
  - [Proper edge coloring](proper-edge-coloring.md)
    - [Edge coloring as scheduling](edge-coloring-as-scheduling.md)
  - [List edge coloring](list-edge-coloring.md)
    - [List-chromatic index](list-chromatic-index.md)
      - [Galvin theorem for bipartite list edge coloring](galvin-theorem-for-bipartite-list-edge-coloring.md)
  - [Chromatic index](chromatic-index.md)
    - [Chromatic index bounds](chromatic-index-bounds.md)
  - [Tait coloring](tait-coloring.md)
- [Chromatic number](chromatic-number.md)
  - [Chromatic number of Euclidean space](chromatic-number-of-euclidean-space.md)
  - [Colour-critical vertex](colour-critical-vertex.md)
  - [Mycielskian](mycielskian.md)
  - [Graphs of arbitrarily high girth and chromatic number](graphs-of-arbitrarily-high-girth-and-chromatic-number.md)
  - [Brooks' theorem](brooks-theorem.md)
- [Edge chromatic number](edge-chromatic-number.md)
  - [Vizing's theorem](vizing-s-theorem.md)
    - [Vizing fan lemma](vizing-fan-lemma.md)
- [Kempe chain](kempe-chain.md)
- [Chromatic polynomial](chromatic-polynomial.md)
  - [Chromatic polynomial determines a Turán graph](chromatic-polynomial-determines-a-turan-graph.md)
  - [Deletion-contraction recurrence for the chromatic polynomial](deletion-contraction-recurrence-for-the-chromatic-polynomial.md)
  - [Chromatic polynomial after attaching a leaf](chromatic-polynomial-after-attaching-a-leaf.md)

## ↑ Ancestors (5)

1. [Graph theory](graph-theory-split.md)
2. [Foundations of mathematics](foundations-of-mathematics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (13)

- [Chromatic number](chromatic-number.md)
- [Chromatic polynomial](chromatic-polynomial.md)
- [Extension of a partial colouring by neighbour-colour savings](extension-of-a-partial-colouring-by-neighbour-colour-savings.md)
- [Graph](graph-split.md)
- [Graph coloring](graph-coloring.md)
- [Greedy coloring](greedy-coloring.md)
- [Independent set (graph theory)](independent-set-graph-theory.md)
- [Kernel list-coloring lemma](kernel-list-coloring-lemma.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-11/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-13/3/i/solution.md)
- [Perfect elimination ordering](perfect-elimination-ordering.md)
- [Proper vertex coloring](proper-vertex-coloring.md)
- [Second-order logic](second-order-logic.md)
