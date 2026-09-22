<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use a [lower-bound search](../../../../../lower-bound-search.md) separately in each nondecreasing row:

```
def searchRows(f: Array[Array[Int]], x: Int): Option[(Int, Int)] = {
  val n = f.length
  val m = if (n == 0) 0 else f(0).length
  if (m == 0) return None
  var i = 0
  while (i < n) {
    var lo = 0
    var hi = m
    while (lo < hi) {
      val mid = lo + (hi - lo) / 2
      if (f(i)(mid) < x) lo = mid + 1
      else hi = mid
    }
    if (lo < m && f(i)(lo) == x) return Some((i, lo))
    i += 1
  }
  None
}
```

The outer [loop invariant](../../../../../loop-invariant.md) says there is no match in earlier rows. The inner invariant is $0\leq lo\leq hi\leq m$, with every value before `lo` smaller than $x$ and every value from `hi` onward at least $x$. [Sortedness](../../../../../sortedness.md) justifies each exclusion, and `hi - lo` strictly decreases. At exit, a match in this row exists exactly when the lower-bound index is inside the row and holds $x$. Failure extends the outer exclusion.

The cost is **$O(n(1+\log m))$**, conventionally written $O(n\log m)$ for $m\geq2$; the extra one matters when a row has a single entry. Storage is constant. The source's column ranges must use indices strictly below $m$, since `f(i)(m)` is outside the [array](../../../../../array-data-structure.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
