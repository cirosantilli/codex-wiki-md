<h1 id="8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Enumerate all pairs of contiguous [substrings](../../../../../substring.md), run the global algorithm on each pair, and take the largest score, also allowing the empty alignment of score zero. There are $O(m^2)$ substrings of the first input and $O(n^2)$ of the second. Each call costs at most $O(mn)$ for positive lengths, giving the requested upper bound **$O(m^3n^3)$**. Substrings are contiguous; enumerating arbitrary subsequences would be a different search.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [8](../../8.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
