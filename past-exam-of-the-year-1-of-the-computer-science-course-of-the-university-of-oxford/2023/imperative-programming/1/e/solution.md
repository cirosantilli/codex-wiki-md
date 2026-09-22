<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Search only the suffix strictly after each candidate first index. This enforces distinct indices even when the target is twice an existing value. Compute the complement in `Long` to prevent [integer overflow](../../../../../integer-overflow.md): subtracting two `Int` values can require 33 signed bits.

```
def twoSum(a: Array[Int], target: Int): (Int, Int) = {
  def lowerBound(from: Int, wanted: Long): Int = {
    var lo = from
    var hi = a.length
    while (lo < hi) {
      val mid = lo + (hi - lo) / 2
      if (a(mid).toLong < wanted) lo = mid + 1
      else hi = mid
    }
    lo
  }
  var i = 0
  while (i < a.length - 1) {
    val wanted = target.toLong - a(i).toLong
    val j = lowerBound(i + 1, wanted)
    if (j < a.length && a(j).toLong == wanted) return (i, j)
    i += 1
  }
  (0, 0)
}
```

The outer [loop invariant](../../../../../loop-invariant.md) says that no solution has a smaller first index than `i`, when a pair is written in increasing index order. A failed suffix [binary search](../../../../../binary-search.md) proves there is no partner for the current `i`, extending the excluded prefix by one. A successful return has $j>i$ and $a(j)=t-a(i)$ in exact [integer arithmetic](../../../../../integer-arithmetic.md). At exhaustion, every possible ordered pair has been excluded, so **the sentinel `(0,0)` means no solution**. The inner [loop invariant](../../../../../loop-invariant.md) is the standard lower-bound partition, restricted to the suffix starting at `i + 1`.

There are at most $N-1$ suffix searches, each taking $O(\log(N+1))$ [running time](../../../../../running-time.md), so the total is $O(N\log(N+1))$, customarily written $O(N\log N)$ for $N\geq2$. [Auxiliary space](../../../../../auxiliary-space.md) is $O(1)$. Empty and singleton [arrays](../../../../../array-data-structure.md) immediately return the sentinel. This is [distinct-index two-sum by suffix lower bounds](../../../../../distinct-index-two-sum-by-suffix-lower-bounds.md); a faster [two-pointer technique](../../../../../two-pointer-technique.md) is also possible on a [sorted array](../../../../../sorted-array.md), but the code here directly meets the requested search-based bound.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
