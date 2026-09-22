<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Reuse `split` and `swap`, but replace recursive calls with a [FIFO queue](../../../../../fifo-queue.md) of unresolved segments. Enqueue only segments of length at least two.
```
def quicksortLoop(): Unit = {
  val work = scala.collection.mutable.Queue[(Int, Int)]()
  if (a.length > 1) work.enqueue((0, a.length))
  while (!work.isEmpty) {
    val (l, r) = work.dequeue()
    val (lt, gt) = split(l, r)
    if (lt - l > 1) work.enqueue((l, lt))
    if (r - gt > 1) work.enqueue((gt, r))
  }
}
```
A useful [loop invariant](../../../../../loop-invariant.md) is that the pending segments are pairwise disjoint valid [array](../../../../../array-data-structure.md) segments of length at least two; the whole [array multiset](../../../../../array-multiset.md) equals its original value; and every inverted pair of positions lies in a single pending segment. Explicitly, if $i<j$ and $a(i)>a(j)$, some queued $[l,r)$ contains both $i$ and $j$. Thus all ordering obligations are localized to queued segments.

Initially the only possible pending segment is the whole [array](../../../../../array-data-structure.md). One [array partitioning](../../../../../two-way-array-partition.md) confines all its remaining inversions to its two child segments. Its equal middle segment is ordered, the left/middle/right boundaries have the correct ordering, and segments of length at most one cannot contain an inversion. Because [array partitioning](../../../../../two-way-array-partition.md) only permutes the selected segment's entries, it cannot create an inversion across a boundary that previously had no inversions. This proves preservation of the [loop invariant](../../../../../loop-invariant.md).

The [loop variant](../../../../../loop-variant.md) is the total pending length

$$
V=\sum_{(l,r)\text{ in work}}(r-l).
$$

Processing one segment removes $r-l$ from $V$ and adds at most $(lt-l)+(r-gt)=(r-l)-(gt-lt)$, strictly less because $gt-lt\geq1$. Thus $V$ is a nonnegative [integer](../../../../../integer-split.md) and decreases. At exit no pending segment exists, so no inversion exists:

$$
\boxed{\text{The original array is sorted in place and preserves every multiplicity}.}
$$

The [FIFO queue](../../../../../fifo-queue.md) itself can grow to $O(N)$ pairs. The [time complexity](../../../../../time-complexity.md) is that of the corresponding recursive [quicksort](../../../../../quicksort.md), including linear behavior on equal input. Removing [recursion](../../../../../recursion-computer-science.md) does not make the worst-case [time complexity](../../../../../time-complexity.md) linear or eliminate the work storage.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
