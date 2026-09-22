<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Because `Set` is invariant in the specified [Scala](../../../../../scala.md) library, even returning `Set[U]` would place the class's [covariant type parameter](../../../../../covariant-type-parameter.md) in an invariant position. Introduce a fresh widened type for each lifting.
```
class CoPartialFnExt[T,+U](data: List[(T,U)])
    extends CoPartialFn[T,U](data) {

  def forwardLift[V >: U](s: Set[T]): Set[V] = {
    val ys: List[V] = this.data.collect {
      case (x,y) if s.contains(x) => y
    }
    ys.toSet
  }

  def backwardLift[V >: U](s: Set[V]): Set[T] =
    this.data.collect {
      case (x,y) if s.contains(y) => x
    }.toSet
}
```
The [lower type bound](../../../../../lower-type-bound.md) gives $U<:V$, so stored output values can be widened into `List[V]` or passed to `s.contains`. Both exposed `Set` types use invariant method [type parameters](../../../../../type-parameter.md), not the class's `U`. Calling `forwardLift[U]` or `backwardLift[U]` when the concrete output type is known recovers the exact output universe; a broader admissible universe is also safe.

For a [partial function](../../../../../partial-function.md), the forward formula is understood only for inputs in its [domain of a function](../../../../../domain-of-a-function.md). The implementations therefore compute

$$
\boxed{F(S)=\{y\mid(x,y)\in\mathrm{data},\ x\in S\},\qquad B(R)=\{x\mid(x,y)\in\mathrm{data},\ y\in R\}.}
$$

The conversion to a [set](../../../../../set-split.md) removes repeated images. Inputs not in the [domain of a function](../../../../../domain-of-a-function.md) contribute nothing to either lifting.

## ↑ Ancestors (12)

1. [C](../c.md)
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
