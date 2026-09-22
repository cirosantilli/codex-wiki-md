# Perfect ternary tree

↑ **Parent:** [Full ternary tree](full-ternary-tree.md)

A [full ternary tree](full-ternary-tree.md) whose leaves all have the same depth. At depth $j$ there are $3^j$ [vertices](vertex-graph-theory.md), so a tree with $h+1$ levels has $N_h=\sum_{j=0}^h3^j=(3^{h+1}-1)/2$ [vertices](vertex-graph-theory.md) and $3^h$ leaves, by the [finite geometric series](finite-geometric-series.md) formula. For a [rose tree](rose-tree.md) representation, recursively flattening children and joining their lists with ordinary [list concatenation](list-concatenation.md) copies each label once per ancestor. The work is therefore $\Theta((h+1)3^h)=\Theta(N_h\log N_h)$ when the complete output is demanded. Passing an already constructed suffix through the [recursion](recursion-computer-science.md) instead emits each label once, giving $\Theta(N_h)$ work.

## ↑ Ancestors (7)

1. [Full ternary tree](full-ternary-tree.md)
2. [Rooted tree](rooted-tree.md)
3. [Tree (graph theory)](tree-graph-theory-split.md)
4. [Combinatorics](combinatorics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/functional-programming-design-and-analysis-of-algorithms/2/d/solution.md)
