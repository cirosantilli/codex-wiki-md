<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Return immediately on equality and omit the final [array](../../../../../array-data-structure.md) inspection:
```
def searchEarly(u: Array[Int], z: Int): Boolean = {
  var a = 0
  var b = u.length
  while (a < b) {
    val middle = a + (b - a) / 2
    val value = u(middle)
    if (value == z) return true
    if (value > z) a = middle + 1
    else b = middle
  }
  false
}
```
An equality returns a genuine matching entry. After a nonequal comparison, descending order excludes the inspected middle entry and one whole side. In the half-open range, setting `b = middle` already excludes the middle index; subtracting one would incorrectly exclude another possible entry. The candidate interval decreases as before, so absence is reported exactly when no possible entry remains.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
