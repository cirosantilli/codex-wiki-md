<h1 id="8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use an [F-bounded polymorphism](../../../../../f-bounded-polymorphism.md) constraint to make comparisons with another `T` available:

```
trait Ordered[T] {
  def <(that: T): Boolean
}

class MinMSet[T <: Ordered[T]](contents: List[T])
    extends MSet[T](contents) {

  def min: T = {
    if (data.isEmpty) throw new NoSuchElementException("MinMSet.min")
    var best = data.head
    var rest = data.tail
    while (rest.nonEmpty) {
      if (rest.head < best) best = rest.head
      rest = rest.tail
    }
    best
  }
}
```

The [upper type bound](../../../../../upper-type-bound.md) `T <: Ordered[T]` guarantees the method signature needed for `rest.head < best`. Assuming that comparison implements the intended total ordering, the [loop invariant](../../../../../loop-invariant.md) says `best` is a minimum of the inspected prefix; the remaining suffix length decreases. The method returns a minimum in $O(N)$ comparisons and $O(1)$ auxiliary space, without deleting it. The bound supplies a comparison operation, not a proof of its order laws.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [8](../../8.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
