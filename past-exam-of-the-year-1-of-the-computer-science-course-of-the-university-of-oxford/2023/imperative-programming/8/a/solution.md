<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The maximally variant safe declarations are:

```
trait Rel1[+X, +Y] { val pairs: List[(X, Y)] }
trait Rel2[-X, +Y] { def relatives(x: X): List[Y] }
trait Rel3[-X, -Y] { def related(x: X, y: Y): Boolean }
```

Leaving one or both parameters invariant is also legal but admits fewer [subtyping](../../../../../subtyping.md) conversions. These are [type variance](../../../../../type-variance.md) annotations.

For `Rel1`, both parameters occur only as outputs. Scala's immutable `List` and `Tuple2` are covariant, so a list of pairs of narrower types can safely be read as pairs of broader types. Thus both may be [covariant type parameters](../../../../../covariant-type-parameter.md). A contravariant declaration would permit, for example, treating a `Rel1[Any, Int]` containing `(7, 0)` as a `Rel1[String, Int]`, then reading its first component as a `String`. That would be unsound; the [compiler](../../../../../compiler.md) rejects the negative annotation at this output position.

For `Rel2`, `X` occurs as a method argument and therefore may be a [contravariant type parameter](../../../../../contravariant-type-parameter.md); `Y` is returned in an immutable list and may be a [covariant type parameter](../../../../../covariant-type-parameter.md). A function that accepts every `Any` is safe to use where only `String` queries are issued. The opposite direction would be unsafe: if `X` were covariant, the following hypothetical conversion could call a string-only implementation with an [integer](../../../../../integer-split.md):

```
val strings: Rel2[String, Int] = new Rel2[String, Int] {
  def relatives(x: String): List[Int] = List(x.length)
}
// Unsafe if Rel2 were incorrectly covariant in X:
// val arbitrary: Rel2[Any, Int] = strings
// arbitrary.relatives(7)
```

Making `Y` contravariant would instead allow an integer-valued `Rel2[String, Any]` to be read as a string-valued `Rel2[String, String]`, recreating the output error.

For `Rel3`, both generic values are consumed and only a [Boolean function](../../../../../boolean-function.md) result is produced, so both may be [contravariant type parameters](../../../../../contravariant-type-parameter.md). A predicate accepting all values of broad types can answer queries restricted to narrower types. Covariance in either parameter would allow passing an unsupported value to a specialized implementation. For example, treating a string-only first-argument predicate as accepting `Any` would permit `related(7, y)` even though its body might call `x.length`. These are applications of the [variance-position rule](../../../../../variance-position-rule.md): method inputs reverse variance, whereas immutable outputs preserve it.[Variance annotations and the change of position in method parameter types](../../../../../scala-2-13-variance-annotations-specification.md)

## ↑ Ancestors (12)

1. [A](../a.md)
2. [8](../../8.md)
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
