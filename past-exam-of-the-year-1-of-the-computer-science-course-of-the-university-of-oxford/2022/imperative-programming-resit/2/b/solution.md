<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Without order information, inspect entries one row at a time:

```
def searchUnordered(f: Array[Array[Int]], x: Int): Option[(Int, Int)] = {
  val n = f.length
  val m = if (n == 0) 0 else f(0).length
  var i = 0
  while (i < n) {
    var j = 0
    while (j < m) {
      if (f(i)(j) == x) return Some((i, j))
      j += 1
    }
    i += 1
  }
  None
}
```

The outer [loop invariant](../../../../../loop-invariant.md) excludes every entry in earlier rows; the inner one also excludes columns before `j` in the current row. Failed [equality tests](../../../../../equality-test.md) preserve these exclusions. The inner and outer [loop variants](../../../../../loop-variant.md) are $m-j$ and $n-i$, respectively. A successful return identifies an actual match, while exhaustion excludes the entire [array](../../../../../array-data-structure.md). At most $nm$ entries are inspected.

The source's “at least $O(nm)$” should be read as a worst-case **$\Omega(nm)$ lower bound**, using the correct asymptotic direction. If any entry were left unread on an all-nonmatching input, changing only that entry to $x$ would leave the observations identical while changing the answer. Thus every always-correct procedure needs $nm$ inspections in the worst case, and this algorithm achieves $\Theta(nm)$ entry inspections. Empty dimensions return absence; the asymptotic claim concerns nonempty arrays.

## ↑ Ancestors (12)

1. [B](../b.md)
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
