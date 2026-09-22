<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Store one maximizing predecessor together with every table value. For [alignment traceback](../../../../../alignment-traceback.md), start at $(m,n)$ and follow these pointers:

- $(i-1,j-1)$ emits `x[i-1]` opposite `y[j-1]`; the letters are equal because that diagonal candidate was allowed only on a match.
- $(i-1,j)$ emits `x[i-1]` opposite a gap.
- $(i,j-1)$ emits a gap opposite `y[j-1]`.

Continue to $(0,0)$, including boundary moves, then reverse the collected columns. Any deterministic choice among tied predecessors gives an optimal alignment. Each step decreases at least one index, so reconstruction costs **$O(m+n)$** additional time and output space. The full score table or predecessor table requires $O(mn)$ storage for positive lengths.

## ↑ Ancestors (12)

1. [C](../c.md)
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
