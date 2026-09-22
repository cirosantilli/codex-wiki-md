<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use [pattern matching](../../../../../pattern-matching.md) and an [optional value](../../../../../optional-value.md) to distinguish absence from a present result:
```
class PartialFn[T, U](val data: List[(T, U)]) {
  def get(x: T): Option[U] =
    data.find { case (key, _) => key == x }.map(_._2)

  def remove(x: T): PartialFn[T, U] =
    new PartialFn[T, U](data.filterNot { case (key, _) => key == x })

  def add(x: T, y: U): PartialFn[T, U] =
    new PartialFn[T, U]((x, y) ::
      data.filterNot { case (key, _) => key == x })
}
```
The representation [precondition](../../../../../precondition.md) is that equal keys always have equal associated values, with a stable equality relation on keys. This permits harmless repeated identical pairs; it excludes conflicting outputs for one input. `get` therefore returns `Some(y)` exactly when the represented [partial function](../../../../../partial-function.md) is defined at `x`. Removing filters out every occurrence of the key and leaves all other pairs unchanged. Adding first removes every old occurrence and prepends exactly the new pair, proving the [partial function](../../../../../partial-function.md) update [postcondition](../../../../../postcondition.md) even if the input contains duplicate identical pairs. The immutable [linked list](../../../../../linked-list.md) representation leaves the original mapping unchanged. Each operation has $O(m+1)$ worst-case [time complexity](../../../../../time-complexity.md) for $m$ pairs under constant-cost key equality.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [7](../../7.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
