<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [covariant type parameter](../../../../../covariant-type-parameter.md) may be produced but not consumed directly. Widen the output type of `add` through a [lower type bound](../../../../../lower-type-bound.md). In `compose`, the first parameter of `CoPartialFn` is invariant, so replace its occurrence of `U` by a fresh [type parameter](../../../../../type-parameter.md) `W` with [lower type bound](../../../../../lower-type-bound.md) `U`.
```
class CoPartialFn[T,+U](val data: List[(T,U)]) {
  require(data.map(_._1).distinct.size == data.size)

  def get(x: T): Option[U] =
    data.find(p => p._1 == x).map(_._2)

  def add[V >: U](x: T, y: V): CoPartialFn[T,V] = {
    val old: List[(T,V)] = data.filterNot(p => p._1 == x)
    new CoPartialFn[T,V]((x,y) :: old)
  }

  def remove(x: T): CoPartialFn[T,U] =
    new CoPartialFn[T,U](data.filterNot(p => p._1 == x))

  def compose[V, W >: U](that: CoPartialFn[W,V]): CoPartialFn[T,V] = {
    val pairs: List[(T,V)] = data.flatMap { case (x,y) =>
      that.get(y).toList.map(z => (x,z))
    }
    new CoPartialFn[T,V](pairs)
  }
}
```
`List`, `Tuple2`, and `Option` are covariant in their element/output parameters, so `data`, `get`, and `remove` are valid producers. The [variance-position rule](../../../../../variance-position-rule.md) permits `U` in the [lower type bounds](../../../../../lower-type-bound.md); every value of `U` can be passed to `that.get`, since $U<:W$. No cast or mutation through a widened reference is needed.[Variance Annotations: variance positions and lower-bound widening](../../../../../scala-2-11-basic-declarations-and-definitions-specification.md)

$$
\boxed{\texttt{add[V >: U]},\qquad\texttt{compose[V, W >: U](that: CoPartialFn[W,V])}.}
$$

The input-key [representation invariant](../../../../../representation-invariant.md) and the [partial function](../../../../../partial-function.md) semantics are unchanged.

## ↑ Ancestors (12)

1. [B](../b.md)
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
