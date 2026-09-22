<h1 id="6/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use deterministic [median of medians](../../../../../../median-of-medians.md) to select the element of rank $i$ in worst-case $\Theta(n)$ time. Partition the [array](../../../../../../array-data-structure.md) about that value, retaining the $i$ smallest elements. The input is a [set](../../../../../../set-split.md), so there are no equal-key ambiguities: take the $i-1$ smaller values and the selected value itself. Sort these $i$ elements with [merge sort](../../../../../../merge-sort.md), then output them.

For completeness, [median of medians](../../../../../../median-of-medians.md) groups values in fives, finds each small group's median, recursively selects a median of those medians as a pivot, and recurses only into the partition containing the requested rank. At least $3n/10-O(1)$ entries lie on each side of the pivot. Its worst-case recurrence is

$$
S(n)\leq S(\lceil n/5\rceil)+S(7n/10+O(1))+O(n)=O(n).
$$

Selection and partitioning cost $\Theta(n)$, and sorting the retained prefix costs $\Theta(i\log i)$ for $i\geq2$. Including output at $i=1$ gives

$$
\boxed{T_3(n,i)=\Theta(n+i\log(i+1)).}
$$

Scanning the input is necessary even to identify its minimum. Ordering the selected $i$ distinct values also has the [comparison sorting lower bound](../../../../../../comparison-sorting-lower-bound.md) $\Omega(i\log i)$, so this is asymptotically optimal for the task. A usual randomized [Quickselect](../../../../../../quickselect.md) gives linear expected selection time, but its quadratic worst case would not establish the requested worst-case guarantee.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [6](../../../6.md)
4. [Functional programming, design and analysis of algorithms](../../../../functional-programming-design-and-analysis-of-algorithms-split.md)
5. [2013](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
