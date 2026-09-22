<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Starting at `last.next`, visit each node once and stop when the traversal would return to its start. This helper is private so that callers do not receive writable nodes from the representation.

```
private def find(name: String): Node = {
  if (last == null) return null
  val first = last.next
  var p = first
  do {
    if (p.name == name) return p
    p = p.next
  } while (p ne first)
  null
}
```

**Null means no entry has that name.** The test `p ne first` compares [object identity](../../../../../object-identity.md), not the equality of name or number fields. At each iteration all previously visited nodes failed the name test. The finite simple cycle guarantees that either a match is found or the traversal returns to `first` after exactly one turn. A singleton cycle is inspected exactly once. Stopping at null instead would fail to terminate on this representation.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [4](../../4.md)
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
