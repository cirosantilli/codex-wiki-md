<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Maintain a remaining rectangle with its top-right corner at `(i,j)`:

```
def searchMonotone(f: Array[Array[Int]], x: Int): Option[(Int, Int)] = {
  val n = f.length
  val m = if (n == 0) 0 else f(0).length
  var i = 0
  var j = m - 1
  while (i < n && j >= 0) {
    val v = f(i)(j)
    if (v == x) return Some((i, j))
    else if (v < x) i += 1
    else j -= 1
  }
  None
}
```

The [loop invariant](../../../../../loop-invariant.md) is that any match must lie in rows $i,\ldots,n-1$ and columns $0,\ldots,j$. Smaller corner values exclude the current row, larger ones exclude the current column, as shown in part (d). The [loop variant](../../../../../loop-variant.md) $(n-i)+(j+1)$ is nonnegative while the rectangle is nonempty and decreases by one on every unsuccessful inspection. When the loop exits, the rectangle is empty, so absence is established.

**At most $n+m-1$ entries are inspected when both dimensions are positive**, giving $O(n+m)$ [running time](../../../../../running-time.md) and $O(1)$ [auxiliary space](../../../../../auxiliary-space.md). An empty dimension causes no entry access. Duplicates do not affect the argument, since every exclusion uses a [strict inequality](../../../../../strict-inequality.md) relative to the target.

## ↑ Ancestors (12)

1. [E](../e.md)
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
