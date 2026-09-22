<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The necessary definedness condition is local: **every [predicate](../../../../../predicate.md) application actually reached before the first false result must produce a Boolean value**. No condition is needed on [predicate](../../../../../predicate.md) applications after that first false result, because the [list suffix](../../../../../suffix-of-a-list.md) is then returned without further testing. If a reached test is bottom at a known cons cell, the reconstructed [list](../../../../../list-abstract-data-type.md) is bottom at that position, while the original [list](../../../../../list-abstract-data-type.md) still exposes a cons there; equality fails.

To prove sufficiency on finite [lists](../../../../../list-abstract-data-type.md), induct on the spine. The empty case gives `[] ++ [] = []`. At a true test the left [list prefix](../../../../../prefix-of-a-list.md) contributes the head, and the [induction](../../../../../mathematical-induction.md) hypothesis reconstructs the tail. At a false test the [list prefix](../../../../../prefix-of-a-list.md) is empty and the [list suffix](../../../../../suffix-of-a-list.md) is the whole current [list](../../../../../list-abstract-data-type.md). For an infinite true-tested [list prefix](../../../../../prefix-of-a-list.md), every finite output [list prefix](../../../../../prefix-of-a-list.md) is copied correctly; the infinite [list prefix](../../../../../prefix-of-a-list.md) hides the possibly divergent [list suffix](../../../../../suffix-of-a-list.md) computation. A partial spine ending in bottom is reconstructed up to exactly the same bottom. Thus finiteness is sufficient for an elementary [induction](../../../../../mathematical-induction.md) proof but is not itself necessary for the identity.

For the uniform [list fold](../../../../../list-fold.md) calculation in part (f), use the convenient stronger assumption that **the input is a finite total [list](../../../../../list-abstract-data-type.md) and the [predicate](../../../../../predicate.md) terminates on every element of that [list](../../../../../list-abstract-data-type.md)**. This makes the reconstruction identity available on every [list suffix](../../../../../suffix-of-a-list.md), not only on the [list suffixes](../../../../../suffix-of-a-list.md) visited by the original [list prefix](../../../../../prefix-of-a-list.md) scan. A total [predicate](../../../../../predicate.md) on the element type ensures this uniformly over all finite total inputs.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
