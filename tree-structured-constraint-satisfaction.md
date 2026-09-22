# Tree-structured constraint satisfaction

↑ **Parent:** [Constraint satisfaction problem](constraint-satisfaction-problem.md)

A binary [constraint satisfaction problem](constraint-satisfaction-problem.md) whose [constraint graph](constraint-graph.md) is a [tree](tree-graph-theory-split.md). Restrict [constraint domains](constraint-domain.md) by unary conditions first. Choose a [rooted tree](rooted-tree.md) orientation and process children before parents. For each child $j$ of $i$, retain in $D_i$ only values having a compatible value in the already reduced $D_j$. Thus every retained parent value has support in each child subtree.

If the root [constraint domain](constraint-domain.md) becomes empty, no solution exists. Otherwise choose any root value, then recursively choose supported child values. A child-to-parent [arc consistency](arc-consistency.md) pass need not enforce full [arc consistency](arc-consistency.md) in both directions; the chosen directional condition suffices for this construction.

The proof uses [mathematical induction](mathematical-induction.md) on subtrees. A retained leaf value satisfies its unary requirements. Each retained parent value has a supported value in every child subtree. Those subtree solutions can be combined because the [tree](tree-graph-theory-split.md) has no [edges](edge-of-a-graph.md) between different child subtrees. Therefore every retained parent value extends to a whole subtree solution, and every retained root value extends to a complete solution without [backtracking](backtracking.md).

For $N$ variables and maximum [constraint domain](constraint-domain.md) size $d$, scanning all value pairs once per [edge](edge-of-a-graph.md) costs $O(Nd^2)$ [time complexity](time-complexity.md) in [Big O notation](big-o-notation.md), when one [binary constraint](binary-constraint.md) evaluation has unit cost. If a constraint requires summing bundle values, its evaluation cost must also be counted.

## ↑ Ancestors (7)

1. [Constraint satisfaction problem](constraint-satisfaction-problem.md)
2. [Search problem](search-problem.md)
3. [Computational problem](computational-problem.md)
4. [Computational complexity theory](computational-complexity-theory.md)
5. [Theoretical computer science](theoretical-computer-science-split.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Constraint graph](constraint-graph.md)
- [Cutset conditioning](cutset-conditioning.md)
- [Cycle cutset](cycle-cutset.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2020/artificial-intelligence/2/d/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2023/artificial-intelligence/3/f/solution.md)
