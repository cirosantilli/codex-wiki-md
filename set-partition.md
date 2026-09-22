# Set partition

↑ **Parent:** [Combinatorics](combinatorics-split.md)

A [set partition](set-partition.md) of a [finite set](finite-set.md) $X$ is a [set](set-split.md) $\pi=\{B_1,\ldots,B_k\}$ of nonempty [subsets](subset.md), called [blocks of a set partition](block-of-a-set-partition.md), with

$$
B_i\ne\varnothing,\qquad B_i\cap B_j=\varnothing\quad(i\ne j),\qquad \bigcup_{i=1}^k B_i=X.
$$

Thus every [set element](element-of-a-set.md) of $X$ belongs to exactly one [block of a set partition](block-of-a-set-partition.md). This is the finite counting version of a [partition of a set](partition-of-a-set.md). The [blocks of a set partition](block-of-a-set-partition.md) are **unlabelled**: their subscripts help describe them, but give them no roles or order. Stanley uses this definition in his classification of counting problems.[section 1.9: set partitions and their blocks](enumerative-combinatorics-volume-1-second-edition-draft-by-richard-stanley.md)

**All possibilities for three elements.** The [set](set-split.md) $\{1,2,3\}$ has exactly five [set partitions](set-partition.md):

$$
\begin{gathered}
\{\{1,2,3\}\},\\
\{\{1,2\},\{3\}\},\quad \{\{1,3\},\{2\}\},\quad \{\{1\},\{2,3\}\},\\
\{\{1\},\{2\},\{3\}\}.
\end{gathered}
$$

For two [blocks of a set partition](block-of-a-set-partition.md), one must have size two and the other size one; the three choices of the lone element give the middle row. One [block of a set partition](block-of-a-set-partition.md) forces the whole [set](set-split.md), and three [blocks of a set partition](block-of-a-set-partition.md) force three [singleton sets](singleton-mathematics.md). This proves the enumeration complete, with counts $1,3,1$ by number of [blocks of a set partition](block-of-a-set-partition.md). Their [sum](sum.md) is the [Bell number](bell-number.md) $B_3=5$.

<a id="image-exact-enumeration-of-the-five-set-partitions-of-1-2-3-outlines-show-blocks-of-a-set-partition-whose-positions-and-colours-carry-no-labels"></a>
![](set-partitions-stirling-three-elements.png)

**[Figure 11](#image-exact-enumeration-of-the-five-set-partitions-of-1-2-3-outlines-show-blocks-of-a-set-partition-whose-positions-and-colours-carry-no-labels). Exact enumeration of the five set partitions of $\{1,2,3\}$: outlines show blocks of a set partition, whose positions and colours carry no labels**.

**What information is kept?** Exchanging the two [blocks of a set partition](block-of-a-set-partition.md) in $\{\{1,2\},\{3\}\}$ leaves the same [set partition](set-partition.md); writing the [tuple](finite-tuple.md) $(\{1,2\},\{3\})$ instead makes an ordered list, different from $(\{3\},\{1,2\})$. Exchanging elements within a [block of a set partition](block-of-a-set-partition.md) also changes nothing. In contrast, $\{\{1,3\},\{2\}\}$ is a different [set partition](set-partition.md), because the actual memberships differ. Both have the same [integer partition](integer-partition.md) $2+1$ of sizes. An [integer partition](integer-partition.md), or its [Ferrers diagram](ferrers-diagram.md), forgets which distinct objects were grouped together.

For four named people, $\{\{1,2\},\{3,4\}\}$ and $\{\{1,3\},\{2,4\}\}$ therefore describe different ways of making two unnamed teams, although both have sizes $2+2$. If every team must have exactly two people, only three [set partitions](set-partition.md) qualify; if any nonempty team sizes are permitted, the [Stirling number of the second kind](stirling-numbers-of-the-second-kind.md) $S(4,2)=7$ counts them. Naming the teams changes the counting problem again.

A [set partition](set-partition.md) is useful whenever membership matters but category names do not. Define $x\sim y$ when $x$ and $y$ belong to the same [block of a set partition](block-of-a-set-partition.md). This is an [equivalence relation](equivalence-relation.md), and its [equivalence classes](equivalence-class.md) recover the [set partition](set-partition.md). Conversely, an [equivalence relation](equivalence-relation.md) supplies its [set partition](set-partition.md) of [equivalence classes](equivalence-class.md). The beautiful simplification is that one grouping can be described by whole [subsets](subset.md) or by a rule comparing two elements. Additional distinctions are organized by [refinement of a set partition](refinement-of-a-set-partition.md).

The [empty set](empty-set.md) has one [set partition](set-partition.md), the empty collection $\pi=\varnothing$, with zero [blocks of a set partition](block-of-a-set-partition.md). This differs from $\{\varnothing\}$, which is forbidden because its proposed [block of a set partition](block-of-a-set-partition.md) is empty.

**Table of contents**

- [Ordered set partition](ordered-set-partition.md)
- [Noncrossing partition](noncrossing-partition.md)
- [Exact cover](exact-cover.md)
- [Block of a set partition](block-of-a-set-partition.md)
- [Refinement of a set partition](refinement-of-a-set-partition.md)
- [Integer partition](integer-partition.md)
  - [Binary partition](binary-partition.md)
  - [Bulgarian solitaire](bulgarian-solitaire.md)
  - [Partition in a rectangle](partition-in-a-rectangle.md)
  - [Ferrers diagram](ferrers-diagram.md)
- [Stirling numbers of the second kind](stirling-numbers-of-the-second-kind.md)
  - [Bell number](bell-number.md)
  - [Graphical Stirling number](graphical-stirling-number.md)

## ↑ Ancestors (4)

1. [Combinatorics](combinatorics-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (40)

- [Allocation to labelled bins](allocation-to-labelled-bins.md)
- [Bell number](bell-number.md)
- [Block of a set partition](block-of-a-set-partition.md)
- [Chromatic index](chromatic-index.md)
- [Colour class](colour-class.md)
- [Combinatorics](combinatorics-split.md)
- [Equitable regularity energy](equitable-regularity-energy.md)
- [Forced merging of large components](forced-merging-of-large-components.md)
- [Graph coloring](graph-coloring-split.md)
- [Integer partition](integer-partition.md)
- [Partition of an integer](partition-of-an-integer.md)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2024/paper-2/d12/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-11/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-13/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-14/1/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-88/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-4/2d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-11/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-11/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-4/2e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-4/2d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-24/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-9/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-9/5/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-4/5e/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-129/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-110/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-130/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-147/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-210/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-2/14/b/i/solution.md)
- [Proper edge coloring](proper-edge-coloring.md)
- [Refinement of a set partition](refinement-of-a-set-partition.md)
- [Refinement variance identity for regularity energy](refinement-variance-identity-for-regularity-energy.md)
- [Regular pair of bipartite partitions](regular-pair-of-bipartite-partitions.md)
- [Set partition](set-partition.md)
- [Stirling numbers of the second kind](stirling-numbers-of-the-second-kind.md)
- [Tripartite graph](tripartite-graph.md)
- [Ultrafilter selection from a partition-rich family](ultrafilter-selection-from-a-partition-rich-family.md)
- [Weighted Szemerédi regularity lemma](weighted-szemeredi-regularity-lemma.md)
