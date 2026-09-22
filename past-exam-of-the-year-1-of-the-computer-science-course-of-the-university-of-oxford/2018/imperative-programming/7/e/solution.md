<h1 id="7/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Declare `+U`, keep its stored [linked list](../../../../../linked-list.md) immutable, and generalize operations that need to accept output values by a fresh [lower type bound](../../../../../lower-type-bound.md):
```
class PartialFn[T, +U](val data: List[(T, U)]) {
  def get(x: T): Option[U] =
    data.find { case (key, _) => key == x }.map(_._2)

  def remove(x: T): PartialFn[T, U] =
    new PartialFn[T, U](data.filterNot { case (key, _) => key == x })

  def add[V >: U](x: T, y: V): PartialFn[T, V] =
    new PartialFn[T, V]((x, y) ::
      data.filterNot { case (key, _) => key == x })

  def compose[V >: U, W](that: PartialFn[V, W]): PartialFn[T, W] = {
    val pairs: List[(T, W)] = data.flatMap {
      case (x, y) => that.get(y).map(z => (x, z)).toList
    }
    new PartialFn[T, W](pairs)
  }
}
```
`get`, `remove`, and the immutable `val data` expose `U` in covariant result positions: [Scala](../../../../../scala.md)'s immutable `List`, `Tuple2` and `Option` preserve that position. The old `add(x:T,y:U)` consumed `U` directly, violating the [variance-position rule](../../../../../variance-position-rule.md). The new `add` accepts a value of a chosen supertype `V` and returns a new mapping with that widened output type; it never inserts the wider value into the old narrower mapping.

The original `compose` also mentions `U` as the first, invariant parameter of `PartialFn[U,V]`. Changing only `add` is therefore insufficient. Its new first [type parameter](../../../../../type-parameter.md) `V >: U` is independent of the class's covariant parameter except for the allowed lower bound. Any stored `y:U` is acceptable to `that.get` as a `V`, while the result has output type `W`. This [lower type bound](../../../../../lower-type-bound.md) solution avoids unchecked variance annotations or casts. The official variance rules illustrate the same lower-bound widening technique for an immutable collection's consuming method; the later 2.13 text corroborates the rule, without identifying an installed 2018 compiler version.[Variance Annotations: method-parameter positions, invariant type arguments, and the lower-bound widening example for Sequence.append](../../../../../scala-2-13-variance-annotations-specification.md)

## ↑ Ancestors (12)

1. [E](../e.md)
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
