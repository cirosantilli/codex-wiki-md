<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Describe routes by [array](../../../../../array-data-structure.md) indices, so repeated entry values cannot confuse positions. Two valid routes are

$$
\boxed{0\to2\to4\to9\to10,\qquad0\to2\to3\to4\to8\to10.}
$$

The first uses jump lengths $2,2,5,1$, bounded respectively by $A[0]=2$, $A[2]=3$, $A[4]=5$, $A[9]=7$. The second uses lengths $2,1,1,4,2$, bounded by $2,3,3,5,2$ at its departing positions. Both reach the final index without landing at the zero entry at index six.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
