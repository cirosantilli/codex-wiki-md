<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [representation invariant](../../../../../representation-invariant.md) that each input occurs at most once in `data`. It is an immutable finite [partial function](../../../../../partial-function.md), so extending or removing an input returns a new object. The source comment `get(x) returns Some(x)` contradicts both the [type signature](../../../../../type-signature.md) `Option[U]` and the input-output semantics: it must return `Some(y)` when $f(x)=y$.
```
class PartialFn[T,U](val data: List[(T,U)]) {
  require(data.map(_._1).distinct.size == data.size)

  def get(x: T): Option[U] =
    data.find(p => p._1 == x).map(_._2)

  def add(x: T, y: U): PartialFn[T,U] =
    new PartialFn[T,U]((x,y) :: data.filterNot(p => p._1 == x))

  def remove(x: T): PartialFn[T,U] =
    new PartialFn[T,U](data.filterNot(p => p._1 == x))

  def compose[V](that: PartialFn[U,V]): PartialFn[T,V] = {
    val pairs: List[(T,V)] = data.flatMap { case (x,y) =>
      that.get(y).toList.map(z => (x,z))
    }
    new PartialFn[T,V](pairs)
  }
}
```
`get` returns an [optional value](../../../../../optional-value.md) rather than inventing a result outside the [domain of a function](../../../../../domain-of-a-function.md). `add` removes any old pair for its input before inserting the replacement; `remove` retains exactly the other pairs. In `compose`, undefined intermediate outputs contribute an empty [list](../../../../../list-abstract-data-type.md); defined outputs contribute one pair. Hence uniqueness of input keys is preserved.

The printed composition order is deliberately followed:

$$
\boxed{\mathrm{this.compose(that)}=\mathrm{that}\circ\mathrm{this},\qquad x\mapsto\mathrm{that}(\mathrm{this}(x)).}
$$

This is the stated [function composition](../../../../../function-composition.md), even though some libraries use the name `compose` for the opposite order.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
