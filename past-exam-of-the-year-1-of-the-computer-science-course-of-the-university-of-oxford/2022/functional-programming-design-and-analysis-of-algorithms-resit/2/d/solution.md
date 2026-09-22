<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Only the first two trees need inspection:
```
cons :: a -> List a -> List a
cons x (List ((w,t):(v,u):ts))
  | w == v = List ((2*w+1, Node x t u):ts)
cons x (List ts) = List ((1, Leaf x):ts)
```
When the first sizes agree, place `x` above those two [perfect binary trees](../../../../../perfect-binary-tree.md). Its [preorder traversal](../../../../../preorder-traversal.md) is `x` followed by the old two traversals. No further size-$w$ tree can occur, so all remaining sizes are at least $2w+1$; equality creates at most the allowed initial duplicate. When the first sizes differ, adjoining a singleton is valid, including the case that the old first tree is also a singleton. These are exactly the two possible greedy representations after increasing the length by one. Each case creates a bounded number of constructors and inspects no tree interior, giving **worst-case $O(1)$ [time complexity](../../../../../time-complexity.md)**. Existing trees are shared.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
