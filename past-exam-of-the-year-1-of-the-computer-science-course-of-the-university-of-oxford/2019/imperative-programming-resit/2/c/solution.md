<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Keep a deficient interval of possible values and only the [array](../../../../../array-data-structure.md) segment containing occurrences from that interval. This is [missing-value search by deficient value intervals](../../../../../missing-value-search-by-deficient-value-intervals.md):
```
def missing(): Int = {
  val n = a.length
  var lo = 0L
  var hi = n.toLong + 1L
  var l = 0
  var r = n
  while (hi - lo > 1L) {
    val p = lo + (hi - lo) / 2L
    val k = partition(l, r, p.toInt)
    if ((k - l).toLong < p - lo) {
      hi = p
      r = k
    } else {
      lo = p
      l = k
    }
  }
  lo.toInt
}
```
The [precondition](../../../../../precondition.md) is that every original entry lies in $[0,N+1)$. The [loop invariant](../../../../../loop-invariant.md) is

$$
0\leq lo<hi\leq N+1,\qquad 0\leq l\leq r\leq N,\qquad r-l<hi-lo,
$$

together with: every active entry lies in $[lo,hi)$, and every original occurrence with a value in that interval is in the active segment. The whole [array](../../../../../array-data-structure.md) remains a [permutation](../../../../../permutation.md) of its initial contents. Initially these assertions follow from the [precondition](../../../../../precondition.md) and $N<N+1$.

After [array partitioning](../../../../../two-way-array-partition.md), the low subinterval has $k-l$ occurrences and $p-lo$ possible values. If it is deficient, retaining it preserves the [loop invariant](../../../../../loop-invariant.md). Otherwise $k-l\geq p-lo$, while the original active count is strictly less than $hi-lo$; subtraction gives

$$
r-k<(hi-lo)-(p-lo)=hi-p.
$$

Thus the high subinterval is deficient and retaining it also preserves the [loop invariant](../../../../../loop-invariant.md). Discarded occurrences lie outside the new candidate interval. The [loop variant](../../../../../loop-variant.md) is the positive [integer](../../../../../integer-split.md) $hi-lo$, which strictly decreases because the midpoint is strictly internal. At exit the interval has one possible value and fewer than one occurrence, so **`lo` is absent from the entire original [array](../../../../../array-data-structure.md)**. For $N=0$ the loop is skipped and zero is returned. The `Long` value bounds avoid overflowing $N+1$; every internal pivot is at most $N$, so its checked mathematical range fits `Int`.

For the [time complexity](../../../../../time-complexity.md), let $W_i$ be the interval width and $m_i$ its active occurrence count before iteration $i$. The [loop invariant](../../../../../loop-invariant.md) gives $m_i<W_i$, and [binary search](../../../../../binary-search.md) gives $W_{i+1}\leq\lceil W_i/2\rceil$. Each [two-way array partition](../../../../../two-way-array-partition.md) costs $O(m_i+1)$. Until the width reaches one, the widths are bounded by $(N+1)/2^i+1$, so the total scan work is bounded by a [geometric series](../../../../../geometric-series.md) plus $O(\log(N+1))$ loop overhead: **$O(N+1)$ overall, hence $O(N)$ for positive $N$**. Partitioning the full [array](../../../../../array-data-structure.md) again at every iteration would instead lose this bound. Auxiliary [space complexity](../../../../../space-complexity.md) is $O(1)$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [Imperative programming resit](../../../imperative-programming-resit-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
