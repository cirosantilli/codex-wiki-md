<h1 id="5/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For [Chomp](../../../../../../chomp.md), one representation is a Boolean [array](../../../../../../array-data-structure.md) `occupied(y)(x)` with one entry per cell. The initial board has every entry true. For the noninitial board in the figure, the sets of occupied column indices in successive rows $y=0,1,\ldots,5$ are $\{0,1,2,3,4,5\}$, $\{0,1,2,3\}$, $\{0,1,2,3\}$, $\{0,1\}$, $\varnothing$, $\varnothing$; all other entries are false.

A more compact representation is the [monotone boundary representation of a grid order ideal](../../../../../../monotone-boundary-representation-of-a-grid-order-ideal.md): an [array](../../../../../../array-data-structure.md) `row(y)` giving the number of occupied cells in row $y$. Occupied cells in a row always form a left prefix. The initial representation is $[6,6,6,6,6,6]$, and **the illustrated noninitial representation is $[6,4,4,2,0,0]$**, indexed upwards from row zero. Its total is $16$. These descriptions use the same coordinate orientation as the original figure; no source image is needed in the solution.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Imperative programming resit](../../../../imperative-programming-resit-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
