# Unmatched-vertex bound for a proper tree matching

↑ **Parent:** [Proper matching in a rooted tree](proper-matching-in-a-rooted-tree.md)

For a [proper matching in a rooted tree](proper-matching-in-a-rooted-tree.md), the number of [unmatched vertices in a matching](unmatched-vertex-in-a-matching.md) does not exceed the number of [leaves of a rooted tree](leaf-of-a-rooted-tree.md). From each unmatched [vertex](vertex-graph-theory.md), build a downward path: at an internal current node that is unmatched or matched upward, every child must be matched downward to one of its own children, or properness would fail. Follow a child and its matching partner, then repeat. The path terminates at a leaf and contains no other unmatched [vertex](vertex-graph-theory.md). Two such downward paths cannot meet, since then one unmatched starting point would lie on the other's path. Their distinct endpoints give the required [injection](injective-function.md). No maximum-size assumption is needed.

## ↑ Ancestors (7)

1. [Proper matching in a rooted tree](proper-matching-in-a-rooted-tree.md)
2. [Matching (graph theory)](matching-graph-theory-split.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2018/algorithms/2/e/solution.md)
- [Proper matching in a rooted tree](proper-matching-in-a-rooted-tree.md)
