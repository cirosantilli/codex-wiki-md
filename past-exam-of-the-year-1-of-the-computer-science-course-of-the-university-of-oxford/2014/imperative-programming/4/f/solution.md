<h1 id="4/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Entry $(j,x)$ in source row `i` becomes entry $(i,x)$ in destination row `j`. Visit source rows in descending order and prepend, producing increasing destination column order without a sorting pass.
```
def transpose: SparseMatrix = {
  val out = new SparseMatrix(N)
  var i = N - 1
  while (i >= 0) {
    for ((j, x) <- rows(i)) {
      out.rows(j) = (i, x) :: out.rows(j)
    }
    i -= 1
  }
  out
}
```
Before processing source row `i`, each destination row contains exactly the contributions from source rows with index greater than `i`, in increasing index order. Prepending index `i` preserves that order, and each source position is unique. Hence the [representation invariant](../../../../../representation-invariant.md) holds and

$$
\boxed{\mathrm{out}_{ji}=A_{ij},\qquad O(N+M)\text{ time}.}
$$

The source [sparse matrix](../../../../../sparse-matrix.md) is unchanged.

## ↑ Ancestors (12)

1. [F](../f.md)
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
