<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Different move orders can lead to the same position, and the two occupancy [lists](../../../../../list-abstract-data-type.md) also retain irrelevant insertion order. Thus this [search tree](../../../../../search-tree.md) repeatedly solves the same remaining game. For example, swapping the order of two `O` moves while leaving the intervening `X` moves legal can reach the same occupied [sets](../../../../../set-split.md).

Canonicalize each state by sorted occupancy [sets](../../../../../set-split.md), or by two [bitboards](../../../../../bitboard.md), and apply [memoization](../../../../../memoization.md) or a visited-state [set](../../../../../set-split.md). Expand each canonical position once, stopping at terminal states, and collect terminal positions in a [set](../../../../../set-split.md). There are at most $3^9$ cell assignments, many of which are illegal; this is much smaller than a [tree](../../../../../tree-graph-theory-split.md) of move permutations. **Store positions, not histories, when the requested output is distinct final positions.** Board rotations and reflections can reduce work further if handled as an additional equivalence: if the output must retain every oriented board, reconstruct those distinct orientations rather than silently returning one representative per symmetry class.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [3](../../3.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
