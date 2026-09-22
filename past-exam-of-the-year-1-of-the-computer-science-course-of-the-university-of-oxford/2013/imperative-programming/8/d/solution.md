<h1 id="8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use an [upper type bound](../../../../../upper-type-bound.md) requiring each element type to implement the supplied comparison interface for its own type. This is [F-bounded polymorphism](../../../../../f-bounded-polymorphism.md).
```
trait Ordered[T] {
  def <(that: T): Boolean
}

class MinSet[T <: Ordered[T]](contents: List[T])
    extends Set[T](contents) {
  def min: T = {
    require(elems.nonEmpty)
    var best = elems.head
    var rest = elems.tail
    while (rest.nonEmpty) {
      if (rest.head < best) best = rest.head
      rest = rest.tail
    }
    best
  }
}
```
Use this locally defined `Ordered`, rather than silently substituting the standard library's different comparison interface. The type bound makes `rest.head < best` well typed. To interpret the result as a [minimum](../../../../../minimum-of-a-subset-of-a-total-order.md), require the comparison to be a consistent strict [total order](../../../../../total-order.md); merely providing a method named `<` cannot establish its mathematical laws.

The [loop invariant](../../../../../loop-invariant.md) is that `best` is a [minimum](../../../../../minimum-of-a-subset-of-a-total-order.md) among the entries already inspected, and `rest` is exactly the uninspected suffix. Comparing its next head with `best` preserves that property. The [loop variant](../../../../../loop-variant.md) is the length of `rest`. On termination,

$$
\boxed{min\in S,\qquad\forall x\in S,\ \neg(x<min).}
$$

The method leaves the [set](../../../../../set-split.md) unchanged, takes $O(|S|)$ [time complexity](../../../../../time-complexity.md) under constant-cost comparisons, and uses constant [auxiliary space](../../../../../auxiliary-space.md). It requires a nonempty [set](../../../../../set-split.md); inherited insertion and deletion continue to preserve the duplicate-free [representation invariant](../../../../../representation-invariant.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [8](../../8.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
