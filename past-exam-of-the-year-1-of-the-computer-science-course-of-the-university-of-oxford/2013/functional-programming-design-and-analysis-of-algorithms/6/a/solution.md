<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Divide-and-conquer algorithms](../../../../../divide-and-conquer-algorithm.md) split a problem into smaller instances of the same kind, solve them recursively, and combine the solutions. A base case handles instances too small to split. For [merge sort](../../../../../merge-sort.md), divide the input into two halves, recursively sort both halves, and merge them by repeatedly taking the smaller current head. Empty and singleton inputs are already sorted.

The [merge algorithm](../../../../../merge-algorithm.md) step preserves sortedness because its chosen head is no larger than either remaining head; it also preserves every input occurrence. These facts and [mathematical induction](../../../../../mathematical-induction.md) on input length prove correctness. Splitting and merging take $\Theta(n)$ time, so

$$
\boxed{T(n)=T(\lfloor n/2\rfloor)+T(\lceil n/2\rceil)+\Theta(n)=\Theta(n\log n).}
$$

At each level the subproblem sizes sum to $n$, and there are $\Theta(\log n)$ levels. Part 3(c) supplies an explicit [Haskell](../../../../../haskell.md) implementation of this construction with a more specialized comparison rule. Standard [array](../../../../../array-data-structure.md) implementations use $O(n)$ auxiliary storage.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
