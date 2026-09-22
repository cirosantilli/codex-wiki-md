<h1 id="6/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Assume the subtrees rooted at the [children in a rooted tree](../../../../../../child-in-a-rooted-tree.md) of $i$ already obey the [max-heap](../../../../../../max-heap.md) condition. Compare $A[i]$ with each present child and choose an index of the largest of these at most three keys. If that index is $i$, stop. Otherwise exchange the two keys, continue at the chosen child, and repeat. This is [sift down](../../../../../../sift-down.md), with the inequality reversed from a minimum-oriented [binary heap](../../../../../../binary-heap.md).

The exchange repairs the old root position because its new key dominates both child roots; only the subtree receiving the displaced key can still be defective. This [recursion invariant](../../../../../../recursion-invariant.md) proves correctness. Each exchange descends one level and costs constant work, so **the worst-case [running time](../../../../../../running-time.md) is $O(h)$ for subtree height $h$, hence $O(\log n)$**. A small key at the root of a suitably ordered heap must descend to a leaf, so the logarithmic worst-case bound is attained.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [6](../../../6.md)
4. [Functional programming, design and analysis of algorithms](../../../../functional-programming-design-and-analysis-of-algorithms-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
