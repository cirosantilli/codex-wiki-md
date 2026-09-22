<h1 id="8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

An indexed [binary heap](../../../../../binary-heap.md) builds the initial queue in $O(|V|)$ time; `extract_min` and `decrease_key` each cost $O(\log |V|)$, while a position table supports membership in $O(1)$. There are $|V|$ extractions and at most $2|E|$ edge inspections, with at most one successful decrease per inspection. Thus the bound is **$O((|V|+|E|)\log |V|)$**, or **$O(|E|\log |V|)$** for a connected graph with at least two vertices. The singleton case is constant time. An unindexed heap cannot provide decrease-key by vertex without an additional position structure.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [8](../../8.md)
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
