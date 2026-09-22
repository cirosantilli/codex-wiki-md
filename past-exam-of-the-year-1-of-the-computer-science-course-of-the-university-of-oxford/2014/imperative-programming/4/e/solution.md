<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Construct a fresh [sparse matrix](../../../../../sparse-matrix.md), transform each stored value, and omit products that become zero.
```
def scale(s: Double): SparseMatrix = {
  val out = new SparseMatrix(N)
  for (i <- 0 until N) {
    out.rows(i) = rows(i).map { case (j, x) => (j, s * x) }
      .filter(e => e._2 != 0.0)
  }
  out
}
```
Filtering preserves column order. It handles `s == 0.0` and any [floating point](../../../../../floating-point-representation.md) underflow producing zero. Sharing immutable [list](../../../../../list-abstract-data-type.md) structure elsewhere would be safe; this code constructs new transformed rows. Within the class, Scala's ordinary `private` permits access to `out.rows`. The result is

$$
\boxed{\mathrm{out}_{ij}=sA_{ij}.}
$$

The [time complexity](../../../../../time-complexity.md) is $O(N+M)$ for $M$ stored entries. As usual for the supplied `Double` model, arithmetic means machine arithmetic; for a finite-real interpretation assume finite operands and products, excluding infinities and NaNs.

## ↑ Ancestors (12)

1. [E](../e.md)
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
