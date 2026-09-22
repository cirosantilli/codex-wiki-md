<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Merging two sorted [lists](../../../../../list-abstract-data-type.md) consumes one head per comparison and takes $O(n)$ time in their combined length, assuming constant-cost comparisons. Computing the length and splitting also takes $O(n)$ time. The balanced [recursion](../../../../../recursion-computer-science.md) therefore satisfies

$$
T(n)=T(\lfloor n/2\rfloor)+T(\lceil n/2\rceil)+O(n),\qquad T(0),T(1)=O(1).
$$

Each recursion level has total linear work, and there are $O(\log n)$ levels. Thus [merge sort](../../../../../merge-sort.md) takes $O(n\log n)$ worst-case time. The final `map snd` adds $O(n)$, preserving the bound. Costs of comparing variable-size keys must be included separately.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
