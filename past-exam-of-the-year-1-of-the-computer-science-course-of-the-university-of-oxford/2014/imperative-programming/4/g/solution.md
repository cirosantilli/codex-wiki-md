<h1 id="4/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

For each source row, use a temporary dense [array](../../../../../array-data-structure.md) to accumulate contributions from nonzero pairs. For every stored $A_{ik}$, traverse stored entries in row $k$ of the other [sparse matrix](../../../../../sparse-matrix.md).
```
def mult(that: SparseMatrix): SparseMatrix = {
  require(N == that.N)
  val out = new SparseMatrix(N)
  for (i <- 0 until N) {
    val acc = Array.fill[Double](N)(0.0)
    for ((k, x) <- rows(i)) {
      for ((j, y) <- that.rows(k)) {
        acc(j) += x * y
      }
    }
    var j = N - 1
    var result: Row = Nil
    while (j >= 0) {
      if (acc(j) != 0.0) result = (j, acc(j)) :: result
      j -= 1
    }
    out.rows(i) = result
  }
  out
}
```
During accumulation, `acc(j)` is the sum of the already processed terms contributing to position $(i,j)$. Missing entries multiply to zero, so ignoring them loses no contribution under the finite arithmetic convention of part (e). At completion,

$$
\boxed{\mathrm{out}_{ij}=\sum_{k=0}^{N-1}A_{ik}\,\mathrm{that}_{kj}.}
$$

Descending `j` and prepending produce strictly increasing stored indices. Omitting zero also handles cancellation. The temporary [array](../../../../../array-data-structure.md) uses $O(N)$ [auxiliary space](../../../../../auxiliary-space.md) beyond the output. The [time complexity](../../../../../time-complexity.md) is

$$
O\left(N^2+\sum_i\sum_{(k,x)\in\mathrm{rows}(i)}|\mathrm{that.rows}(k)|\right),
$$

at worst $O(N^3)$, but potentially much smaller when the [matrices](../../../../../matrix.md) are sparse. The $N^2$ term covers clearing and scanning the row accumulators. Finite-precision rounding can affect the numerical result, as in any `Double` [matrix multiplication](../../../../../matrix-multiplication.md).

## ↑ Ancestors (12)

1. [G](../g.md)
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
