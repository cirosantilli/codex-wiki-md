<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume `NumLevels >= 1`. Both [sentinel nodes](../../../../../sentinel-node.md) occur on every level; the tail ends every [linked list](../../../../../linked-list.md).
```
val head = new Node(Int.MinValue)
val tail = new Node(Int.MaxValue)
for (level <- 0 until NumLevels) {
  head.nexts(level) = tail
  tail.nexts(level) = null
}
```
The empty [skip list](../../../../../skip-list.md) therefore has

$$
\boxed{\mathrm{head}\longrightarrow\mathrm{tail}\longrightarrow\mathrm{null}\quad\text{at every level}.}
$$

The forbidden data values distinguish the [sentinel nodes](../../../../../sentinel-node.md) from genuine entries.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
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
