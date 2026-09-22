<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Merge sort](../../../../../merge-sort.md) splits the [array](../../../../../array-data-structure.md) into two halves, recursively sorts both and merges their sorted outputs. During the [merge algorithm](../../../../../merge-algorithm.md), compare the first unconsumed entry of each half, emit the smaller and advance that half; append the remainder when one half ends. The emitted prefix is always sorted and contains exactly the already consumed entries, proving the merge step correct. [Induction](../../../../../mathematical-induction.md) on input length proves the full [sorting algorithm](../../../../../sorting-algorithm.md) correct.

The [recurrence relation](../../../../../recurrence-relation.md) is $T(n)=2T(n/2)+\Theta(n)$ for powers of two, with constant base cost. In the [Master theorem](../../../../../master-theorem.md), $a=b=2$ and $n^{\log_b a}=n$, matching the merge term. Hence **$T(n)=\Theta(n\log n)$**. Floor/ceiling splits give the same bound for arbitrary $n$; conventional merging uses $O(n)$ auxiliary space.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
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
