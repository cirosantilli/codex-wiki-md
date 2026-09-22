<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Return the [lower-bound search](../../../../../lower-bound-search.md) boundary, permitting both zero and the [array](../../../../../array-data-structure.md) length:
```
def lowerBound(a: Array[Int], x: Int): Int = {
  require(a != null) // a is nondecreasing
  var lo = 0
  var hi = a.length
  while (lo < hi) {
    val mid = lo + (hi - lo) / 2
    if (a(mid) < x) lo = mid + 1
    else hi = mid
  }
  lo
}
```
The [precondition](../../../../../precondition.md) includes nondecreasing order. The [loop invariant](../../../../../loop-invariant.md) is

$$
0\leq lo\leq hi\leq n,\qquad a[0..lo)<x,\qquad x\leq a[hi..n).
$$

Initially both excluded ranges are empty. If $a(mid)<x$, sortedness justifies excluding every position through `mid`; otherwise it justifies excluding every position from `mid` onwards. The [loop variant](../../../../../loop-variant.md) $hi-lo$ is a nonnegative [integer](../../../../../integer-split.md) that strictly decreases. When the old width is positive, `mid` is a valid [array index](../../../../../array-index.md). The midpoint expression avoids adding two potentially large indices. At exit $lo=hi$, so **`lo` satisfies the required partition**, including when $n=0$. Each new width is at most half the old width, rounded down; this gives $O(\log(n+1))$ [time complexity](../../../../../time-complexity.md) and [constant space](../../../../../constant-space.md), conventionally $O(\log n)$ for nontrivial sizes.

## ↑ Ancestors (12)

1. [B](../b.md)
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
