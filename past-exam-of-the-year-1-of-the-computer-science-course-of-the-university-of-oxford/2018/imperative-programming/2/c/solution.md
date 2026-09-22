<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A second [binary search](../../../../../binary-search.md) locates the first entry strictly greater than `x`:
```
def upperBound(a: Array[Int], x: Int): Int = {
  require(a != null) // a is nondecreasing
  var lo = 0
  var hi = a.length
  while (lo < hi) {
    val mid = lo + (hi - lo) / 2
    if (a(mid) <= x) lo = mid + 1
    else hi = mid
  }
  lo
}

def equalRange(a: Array[Int], x: Int): (Int, Int) =
  (lowerBound(a, x), upperBound(a, x))
```
For [upper-bound search](../../../../../upper-bound-search.md), the [loop invariant](../../../../../loop-invariant.md) is $0\leq lo\leq hi\leq n$, $a[0..lo)\leq x$, and $x<a[hi..n)$; its [loop variant](../../../../../loop-variant.md) is again $hi-lo$. The same midpoint and sortedness arguments prove preservation, termination and $O(\log(n+1))$ [time complexity](../../../../../time-complexity.md). The first [binary search](../../../../../binary-search.md) in part (b) already has its own [loop invariant](../../../../../loop-invariant.md) and [loop variant](../../../../../loop-variant.md).

Let the two boundaries be $i,j$. There cannot be a value greater than $x$ before the first value at least $x$, so $i\leq j$. Every entry between them is simultaneously at least and at most $x$, hence equals $x$. Entries before $i$ are smaller and entries at or after $j$ are larger, so the interval cannot be extended at either end. This proves the [equal-range search](../../../../../equal-range-search.md) result is maximal. **If `x` is absent, `i == j`, both equal to its insertion position**; this can be zero, $n$, or an interior gap. Two logarithmic searches still have logarithmic total [time complexity](../../../../../time-complexity.md). Computing an upper boundary as `lowerBound(a, x+1)` would introduce an unnecessary [integer overflow](../../../../../integer-overflow.md) bug at the largest [integer](../../../../../integer-split.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
