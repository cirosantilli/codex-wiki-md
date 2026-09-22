<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Keep the entries before column `j`, discard any old entry at `j`, and retain those after it. Insert the replacement only when it is nonzero.
```
def set(i: Int, j: Int, x: Double): Unit = {
  require(0 <= i && i < N && 0 <= j && j < N)
  val before = rows(i).takeWhile(e => e._1 < j)
  val after = rows(i).dropWhile(e => e._1 <= j)
  val middle: Row = if (x == 0.0) Nil else List((j, x))
  rows(i) = before ::: middle ::: after
}
```
All indices in `before` are below `j` and all in `after` are above it, so the [representation invariant](../../../../../representation-invariant.md) is preserved. Other rows and all other column values remain unchanged:

$$
\boxed{A'_{ij}=x,\qquad A'_{kl}=A_{kl}\text{ when }(k,l)\ne(i,j).}
$$

Assigning zero removes storage for that entry. The [time complexity](../../../../../time-complexity.md) is linear in the stored row length.

## ↑ Ancestors (12)

1. [D](../d.md)
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
