<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use null to indicate that the requested key is absent:

```
private def find(name: String, head: Entry): Entry = {
  var cursor = head
  while (cursor != null && cursor.name != name) {
    cursor = cursor.next
  }
  cursor
}
```

The [loop invariant](../../../../../loop-invariant.md) is that the skipped [string prefix](../../../../../string-prefix.md) contains no entry with the requested name and `cursor` starts the unsearched [string suffix](../../../../../string-suffix.md) of the unchanged bucket. Its remaining length is a [loop variant](../../../../../loop-variant.md). [Short-circuit evaluation](../../../../../short-circuit-evaluation.md) prevents accessing a null entry. On exit, either `cursor` is null and the whole bucket has been ruled out, or its name equals the key. **No [list](../../../../../list-abstract-data-type.md) links or stored numbers are modified.** [String](../../../../../string.md) comparison here uses value equality; node deletion elsewhere uses reference identity.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
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
