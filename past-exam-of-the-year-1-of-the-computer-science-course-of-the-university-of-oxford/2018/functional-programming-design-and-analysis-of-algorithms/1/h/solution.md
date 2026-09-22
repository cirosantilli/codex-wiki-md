<h1 id="1/h/solution">Solution</h1>

↑ **Parent:** [H](../h.md)

Suppose that a direct [tree fold](../../../../../tree-fold.md) with result type `[Tree a]` implements `proper`, so `proper = fold one two`. Every leaf has result `[]`, hence `one x = []` for every label `x`. Consequently `proper (Two (One x) (One y))` would always equal `two [] []`, independently of either label. Taking labels from `Bool`, the inputs `Two (One False) (One False)` and `Two (One True) (One False)` would therefore have equal results. Their correct results are `[One False, One False]` and `[One True, One False]`, which differ. This is a contradiction.

**There is no direct fold with only the proper-subtree list as its recursive summary.** This is the [direct tree-fold information obstruction](../../../../../direct-tree-fold-information-obstruction.md): replacing both children by equal summaries prevents the parent operation from recovering their different labels. The claim must not be extended to every expression containing a [tree fold](../../../../../tree-fold.md). A fold retaining the original tree alongside its proper-subtree list, followed by projection, does work; alternatively `tail . subs` uses the richer fold from part (f).

## ↑ Ancestors (12)

1. [H](../h.md)
2. [1](../../1.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
