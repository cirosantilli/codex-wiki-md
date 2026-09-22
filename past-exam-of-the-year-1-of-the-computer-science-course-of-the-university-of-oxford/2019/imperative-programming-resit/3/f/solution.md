<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Let $m\geq1$ be the number of real contacts, and suppose the requested name is at position $j$, counting from one. The implementation above makes exactly $j$ name-equality comparisons, including the successful comparison; null checks are not [string](../../../../../string.md) comparisons. Thus **the minimum is one, when the first real contact is requested, and the maximum is $m$, when the last is requested**. The [precondition](../../../../../precondition.md) excludes unsuccessful recalls and recalls on an empty book. This counts calls to [string](../../../../../string.md) equality, not individual character inspections within each call.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [3](../../3.md)
3. [Imperative programming resit](../../../imperative-programming-resit-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
