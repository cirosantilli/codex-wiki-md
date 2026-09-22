<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Return the key's active [array index](../../../../../array-index.md), or **`-1` if absent**:

```
private def isInMap(x: Int): Int = {
  var i = 0
  while (i < used && elements(i) != x) i += 1
  if (i < used) i else -1
}
```

The [loop invariant](../../../../../loop-invariant.md) states that every index below `i` has a key different from `x`. The scan ignores all inactive cells, and [short-circuit evaluation](../../../../../short-circuit-evaluation.md) protects the array access at the end of the active prefix. Key uniqueness makes a successful index unambiguous. Its [running time](../../../../../running-time.md) is $O(used)$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [5](../../5.md)
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
