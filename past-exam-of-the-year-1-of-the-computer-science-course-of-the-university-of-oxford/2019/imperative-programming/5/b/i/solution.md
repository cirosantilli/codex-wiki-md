<h1 id="5/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**Yes, provided balancing guarantees logarithmic height.** In a suitably maintained [balanced binary tree](../../../../../../balanced-binary-tree.md) of height $O(\log(n+1))$, insertion searches one root-to-leaf path and deletion of the minimum follows the leftmost path. Reconnecting the tree and performing the required rebalancing also costs at most a constant amount per level for the standard logarithmic-time schemes. Thus both operations take $O(\log(n+1))$ time, conventionally written $O(\log n)$ for nontrivial sizes. Merely calling a tree approximately balanced would not prove that height bound; it is the balancing guarantee that matters. Without it, a [binary search tree](../../../../../../binary-search-tree.md) can have linear height.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Imperative programming](../../../../imperative-programming-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
