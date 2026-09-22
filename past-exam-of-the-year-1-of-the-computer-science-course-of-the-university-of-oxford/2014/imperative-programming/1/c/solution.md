<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use [missing-value search by deficient value intervals](../../../../../missing-value-search-by-deficient-value-intervals.md): halve the candidate value [interval](../../../../../interval-mathematics.md), and apply [array partitioning](../../../../../two-way-array-partition.md) only to the [array](../../../../../array-data-structure.md) segment whose entries lie in that [interval](../../../../../interval-mathematics.md).
```
def missing(): Int = {
  require(N < Int.MaxValue)
  var lo = 0; var hi = N + 1
  var l = 0; var r = N
  while (hi - lo > 1) {
    val p = lo + (hi - lo) / 2
    val k = partition(l, r, p)
    if (k - l < p - lo) {
      hi = p; r = k
    } else {
      lo = p; l = k
    }
  }
  lo
}
```
The [loop invariant](../../../../../loop-invariant.md) is $0\leq l\leq r\leq N$, $0\leq lo<hi\leq N+1$, and

$$
a[l..r)\subseteq[lo,hi),\qquad r-l<hi-lo.
$$

More precisely, the segment contains **all occurrences** of original values in $[lo,hi)$, and the complete [array](../../../../../array-data-structure.md) remains a [permutation](../../../../../permutation.md) of its original state. The occurrences statement is essential: absence from the final segment must imply absence from the original [array](../../../../../array-data-structure.md).

After [array partitioning](../../../../../two-way-array-partition.md), let $m=r-l$, $W=hi-lo$, $m_L=k-l$, and $W_L=p-lo$. If $m_L<W_L$, retain the left side. Otherwise the right side has

$$
m_R=m-m_L<W-W_L=W_R
$$

occurrences. Either choice preserves the strict deficiency and the all-occurrences condition. The positive [integer](../../../../../integer-split.md) width $hi-lo$ decreases, proving termination. At width one, the active segment has fewer than one entry and is empty. Therefore

$$
\boxed{\text{return }lo,\quad lo\in[0,N+1),\quad lo\text{ is absent from the original array}.}
$$

For the [time complexity](../../../../../time-complexity.md), after $t$ splits the width is at most $\lceil(N+1)/2^t\rceil$, and the scan length is smaller than that width. Summing over the $O(\log(N+1))$ levels gives a [geometric series](../../../../../geometric-series.md) plus logarithmic overhead, hence $O(N+1)$ overall, conventionally $O(N)$ for $N\geq1$. This proof bounds the retained occurrence count by the retained value width; it does not assume that each [array partitioning](../../../../../two-way-array-partition.md) splits the number of occurrences in half. The $N=0$ case returns zero immediately.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
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
