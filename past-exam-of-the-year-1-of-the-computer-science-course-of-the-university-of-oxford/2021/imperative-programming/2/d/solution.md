<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Reuse the verified longest-common-prefix scan, handling equality before scanning:

```
def before(i: Int, j: Int): Boolean = {
  require(0 <= i && i < N && 0 <= j && j < N)
  if (i == j) false
  else {
    val k = longestFrom(i, j)
    if (j + k == N) false
    else if (i + k == N) true
    else a(i + k) < a(j + k)
  }
}
```

There is no additional [while loop](../../../../../while-loop.md): the helper's [loop invariant](../../../../../loop-invariant.md) is that the first `k` characters agree and both indices remain in bounds. If the second [string suffix](../../../../../string-suffix.md) ends first, the first cannot precede it; if the first ends first, it is a proper [string prefix](../../../../../string-prefix.md) and precedes the second. Otherwise the first mismatching characters decide [lexicographic order](../../../../../lexicographic-order.md). Distinct suffixes cannot both end after the same number of characters, since their lengths differ.

The `i == j` case ensures **a strict comparator**, returning false for a [string suffix](../../../../../string-suffix.md) compared with itself, in constant time. For distinct suffixes its running time is $O(K+1)$, where $K$ is the longest repeated-substring length of the full [array](../../../../../array-data-structure.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
