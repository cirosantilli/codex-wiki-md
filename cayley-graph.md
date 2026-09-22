# Cayley graph

↑ **Parent:** [Geometric group theory](geometric-group-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cayley_graph)

A [Cayley graph](cayley-graph.md) turns multiplication in a [group](group-split.md) into travel: the chosen [generators of a group](generator-of-a-group.md) are the allowed one-step moves, and a [word over an alphabet](string.md) becomes a route. This lets us study a [finitely generated group](finitely-generated-group.md) using [graph distances](distance-graph-theory.md), [closed balls](closed-ball.md), and [geodesics](geodesic.md), rather than only equations between products.

Let $G$ be a [group](group-split.md) with a finite [generating set of a group](generating-set-of-a-group.md) $S$ satisfying $S=S^{-1}$ and $1\notin S$. Such a [symmetric subset of a group](symmetric-subset-of-a-group.md) includes the [inverse element](inverse-element.md) of every allowed move. The [Cayley graph](cayley-graph.md) $\operatorname{Cay}_S(G)$ has [vertex set](vertex-set.md) $G$ and joins $g$ to $gs$ for each $s\in S$. We choose right multiplication for these moves. Reversing the move uses $s^{-1}$, so for [graph distance](distance-graph-theory.md) we regard $g\to gs$ and $gs\to g$ as the two orientations of one undirected [edge](edge-of-a-graph.md). An involution therefore gives one [edge](edge-of-a-graph.md), not two parallel [edges](edge-of-a-graph.md). Each [edge](edge-of-a-graph.md) has length one, regardless of its length in a drawing.[Bridson, Non-positive curvature in group theory, Definition 1.7](https://people.maths.ox.ac.uk/bridson/papers/BATH97.pdf)

A sequence $s_1,\ldots,s_n$ labels the [walk](walk-in-a-graph.md)

$$
g,\quad gs_1,\quad gs_1s_2,\quad\ldots,\quad gs_1\cdots s_n.
$$

It ends at $h$ exactly when $g^{-1}h=s_1\cdots s_n$. Thus the [Cayley graph](cayley-graph.md) is a [connected graph](connected-graph.md) precisely because $S$ generates $G$, and its [graph distance](distance-graph-theory.md) on [vertices](vertex-graph-theory.md) is the [word metric](word-metric.md). Left multiplication by $a$ sends the [edge](edge-of-a-graph.md) from $g$ to $gs$ to the [edge](edge-of-a-graph.md) from $ag$ to $(ag)s$, preserving its generator label: this is a [group action](group-action-split.md) by [graph automorphisms](graph-automorphism.md) and [isometries](isometry.md). Viewing [groups](group-split.md) as symmetries of geometric objects is the motivation of Clay and Margalit's introduction.[Clay and Margalit, Office Hours with a Geometric Group Theorist, Office Hour 1, pages 3–5](https://assets.press.princeton.edu/chapters/s11042.pdf)

The useful geometric object includes its allowed moves, not just its drawing. [Cayley graphs of the integers](cayley-graphs-of-the-integers.md) show how changing the moves adds shortcuts; [word metric balls in the integer lattice](word-metric-balls-in-the-integer-lattice.md) show how the same [group](group-split.md) can acquire visibly different [closed balls](closed-ball.md). Meier's book develops this passage from [group operations](group-operation.md) to [graphs](graph-split.md) as its central motivation.[Meier, Groups, Graphs and Trees, Preface and Chapter 1 introduction](https://api.pageplace.de/preview/DT0400.9780511421594_A23678234/preview-9780511421594_A23678234.pdf)

**Table of contents**

- [Cayley graphs of the integers](cayley-graphs-of-the-integers.md)
- [Schreier graph](schreier-graph.md)
- [Diameter of a finite group with respect to a generating set](diameter-of-a-finite-group-with-respect-to-a-generating-set.md)
  - [Trivial diameter bound for a finite group](trivial-diameter-bound-for-a-finite-group.md)
  - [Diameter bound for a non-abelian finite simple group](diameter-bound-for-a-non-abelian-finite-simple-group.md)
- [Word metric](word-metric.md)
  - [Word metric ball](word-metric-ball.md)
    - [Word metric balls in the integer lattice](word-metric-balls-in-the-integer-lattice.md)
  - [Word length](word-length.md)
  - [Stable word length](stable-word-length.md)
  - [Equivalence of finite word metrics](equivalence-of-finite-word-metrics.md)
- [Infinite line as a Cayley graph](infinite-line-as-a-cayley-graph.md)

## ↑ Ancestors (5)

1. [Geometric group theory](geometric-group-theory-split.md)
2. [Geometry and topology](geometry-and-topology-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (24)

- [Cayley graph](cayley-graph.md)
- [Cayley graphs of the integers](cayley-graphs-of-the-integers.md)
- [Combing of a group](combing-of-a-group.md)
- [Diameter of a finite group with respect to a generating set](diameter-of-a-finite-group-with-respect-to-a-generating-set.md)
- [Free product with factor generating set](free-product-with-factor-generating-set.md)
- [Growth function of a discrete metric space](growth-function-of-a-discrete-metric-space.md)
- [Infinite cyclic subgroups of hyperbolic groups are undistorted](infinite-cyclic-subgroups-of-hyperbolic-groups-are-undistorted.md)
- [Infinite line as a Cayley graph](infinite-line-as-a-cayley-graph.md)
- [Metric geodesic triangle](metric-geodesic-triangle.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-11/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-5/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-5/4/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-5/4/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-133/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-133/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-143/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-143/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-149/4/c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-111/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-133/3/b/solution.md)
- [Trivial diameter bound for a finite group](trivial-diameter-bound-for-a-finite-group.md)
- [Word length](word-length.md)
- [Word metric](word-metric.md)
- [Word metric balls in the integer lattice](word-metric-balls-in-the-integer-lattice.md)
