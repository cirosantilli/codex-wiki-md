<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The ordering operations used to decide the partitions require an **`Ord a` constraint**. A [function](../../../../../function-split.md) with [parametric polymorphism](../../../../../parametric-polymorphism.md) and type `[a] -> [a]` cannot inspect arbitrary element values to decide which one is smaller; for example, [functions](../../../../../function-split.md) themselves need not admit the comparison operations required by this [sorting algorithm](../../../../../sorting-algorithm.md). A [Haskell Ord class](../../../../../haskell-ord-class.md) instance supplies the comparison method, with its ordering laws a separate semantic assumption.[Chapter 9, the Ord class and compare method](../../../../../haskell-2010-language-report.md)

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
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
