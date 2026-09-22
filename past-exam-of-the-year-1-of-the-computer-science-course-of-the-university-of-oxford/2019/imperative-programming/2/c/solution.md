<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Ranks are relative to the current segment. The pivot's rank is `p-l`, not its absolute index:
```
def select(k: Int, l: Int, r: Int): Int = {
  require(0 <= l && l < r && r <= a.length)
  require(0 <= k && k < r - l)
  if (r - l == 1) a(l)
  else {
    val p = partition(l, r)
    val rank = p - l
    if (k == rank) a(p)
    else if (k < rank) select(k, l, p)
    else select(k - rank - 1, p + 1, r)
  }
}
```
The [array partitioning](../../../../../two-way-array-partition.md) places exactly `rank` strictly smaller entries before the pivot, with all later entries at least the pivot. Thus the pivot is the element of sorted rank `rank`, even when equal values occur later. A requested earlier rank is unchanged in the left segment; a later rank loses the low entries and the pivot, accounting for the subtraction `rank+1`. The recursive segment is nonempty in either branch that takes it, and its length strictly decreases. [Induction](../../../../../mathematical-induction.md) on segment length therefore proves **the returned value is the requested [order statistic](../../../../../order-statistic.md)**, with at most one recursive call. Only the selected segment is permuted; all outside entries remain unchanged. This is [Quickselect](../../../../../quickselect.md).

## ↑ Ancestors (12)

1. [C](../c.md)
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
