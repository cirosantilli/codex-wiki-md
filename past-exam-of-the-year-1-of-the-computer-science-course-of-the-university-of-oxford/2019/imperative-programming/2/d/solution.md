<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Replace the tail call by updates to local bounds and a local rank:
```
def selectIterative(k: Int, l: Int, r: Int): Int = {
  require(0 <= l && l < r && r <= a.length)
  require(0 <= k && k < r - l)
  var low = l
  var high = r
  var rank = k
  while (high - low > 1) {
    val p = partition(low, high)
    val pivotRank = p - low
    if (rank == pivotRank) return a(p)
    if (rank < pivotRank) high = p
    else {
      rank -= pivotRank + 1
      low = p + 1
    }
  }
  a(low)
}
```
The [loop invariant](../../../../../loop-invariant.md) says that $l\leq low<high\leq r$, $0\leq rank<high-low$, and selecting rank `rank` in the active segment yields the originally requested [order statistic](../../../../../order-statistic.md). The original segment's [multiset](../../../../../multiset.md) is preserved, and outside it no entries change. The updates are exactly the recursive reductions proved in part (c). The [loop variant](../../../../../loop-variant.md) is $high-low$; a non-returning iteration strictly decreases it. A one-entry segment has only rank zero, establishing the final return. **Auxiliary space is $O(1)$**, rather than a potentially deep [call stack](../../../../../call-stack.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
