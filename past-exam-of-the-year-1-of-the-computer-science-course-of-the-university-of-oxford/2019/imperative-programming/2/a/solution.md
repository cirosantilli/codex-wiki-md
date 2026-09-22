<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Compare values directly, avoiding subtraction that could overflow:
```
def bestIndex(l: Int, r: Int): Int = {
  require(0 <= l && l < r && r <= a.length)
  val first = l
  val middle = l + (r - l) / 2
  val last = r - 1
  if (a(first) <= a(middle)) {
    if (a(middle) <= a(last)) middle
    else if (a(first) <= a(last)) last
    else first
  } else {
    if (a(first) <= a(last)) first
    else if (a(middle) <= a(last)) last
    else middle
  }
}
```
Each branch returns an index whose value lies between the other two sampled values. Non-strict comparisons make ties harmless. **The [precondition](../../../../../precondition.md) is a nonempty valid segment**, not a segment of at least three elements: for lengths one or two some sample indices coincide, but the code still returns a valid median of the sampled triple. This matters because selection can reach a two-element segment. With three distinct sample values, the pivot is not the minimum or maximum of the whole segment, but it need not be near the segment's true median. [Median-of-three pivot selection](../../../../../median-of-three-pivot-selection.md) is a heuristic, not a balance guarantee.

## ↑ Ancestors (12)

1. [A](../a.md)
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
