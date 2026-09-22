<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Select entries having the requested column. The [representation invariant](../../../../../representation-invariant.md) ensures that the selected [list](../../../../../list-abstract-data-type.md) has length at most one.
```
def get(i: Int, j: Int): Double = {
  require(0 <= i && i < N && 0 <= j && j < N)
  val entries = rows(i).filter(e => e._1 == j)
  if (entries.isEmpty) 0.0 else entries.head._2
}
```
Consequently

$$
\boxed{\mathrm{get}(i,j)=A_{ij}.}
$$

This version follows the hint and has [time complexity](../../../../../time-complexity.md) linear in the number of stored entries in row `i`. An ordered early-exit scan is also possible.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
