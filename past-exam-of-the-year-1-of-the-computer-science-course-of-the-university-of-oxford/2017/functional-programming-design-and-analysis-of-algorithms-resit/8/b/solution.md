<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A deterministic [comparison sort](../../../../../comparison-sort.md) on $n$ distinct keys must distinguish $n!$ possible initial orders. Its binary comparison [decision tree](../../../../../decision-tree.md) therefore has at least $n!$ leaves: a leaf fixes one output ordering and cannot be correct for two different strict orders of the original records.

A binary tree of height $h$ has at most $2^h$ leaves, hence

$$
\boxed{h\geq\lceil\log_2(n!)\rceil=\Omega(n\log n).}
$$

This is the [comparison sorting lower bound](../../../../../comparison-sorting-lower-bound.md) on the worst-case number of comparisons. Distinct keys have only two possible comparison outcomes, even if an implementation's comparator also supports equality. Algorithms exploiting numeric key values, such as counting sort, fall outside this model.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [8](../../8.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
