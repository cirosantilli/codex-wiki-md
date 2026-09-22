<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

An [immutable object](../../../../../immutable-object.md) can widen its element type when adding a value by returning a new object. Introduce a [lower type bound](../../../../../lower-type-bound.md) $U>:T$ on the method's fresh [type parameter](../../../../../type-parameter.md).
```
class ISet[+T](contents: List[T]) {
  private val elems: List[T] = contents.distinct

  def add[U >: T](x: U): ISet[U] = {
    val widened: List[U] = elems
    if (widened.contains(x)) new ISet[U](widened)
    else new ISet[U](x :: widened)
  }

  def delete(): (T, ISet[T]) = {
    require(elems.nonEmpty)
    (elems.head, new ISet[T](elems.tail))
  }
}
```
As before, the [representation invariant](../../../../../representation-invariant.md) excludes duplicates, and the [abstraction function](../../../../../abstraction-function.md) returns the unordered [set](../../../../../set-split.md) of entries. The constructor normalization makes the [representation invariant](../../../../../representation-invariant.md) hold even for repeated initial entries. Both operations construct a fresh [set](../../../../../set-split.md) object and leave the original object unchanged, including when addition finds an existing member.

For a receiver representing $S$, the new object returned by `add` represents $S\cup\{x\}$. Deletion returns a pair $(x,R)$ with $x\in S$ and $R$ representing $S\setminus\{x\}$. Crucially,

$$
\boxed{add[U>:T](x:U):ISet[U],\qquad delete():(T,ISet[T]).}
$$

The widened [list](../../../../../list-abstract-data-type.md) is valid because immutable `List` itself has a [covariant type parameter](../../../../../covariant-type-parameter.md). A client can view an `ISet[Int]` as `ISet[Any]`, but adding a [string](../../../../../string.md) creates a separate widened result; it cannot put a [string](../../../../../string.md) into the old [integer](../../../../../integer-split.md) [set](../../../../../set-split.md). This explains how using [immutable objects](../../../../../immutable-object.md) makes the desired [type variance](../../../../../type-variance.md) sound. A direct `add(x: T)` on a covariant [software class](../../../../../class-programming.md) would still violate the [variance-position rule](../../../../../variance-position-rule.md); immutability alone does not repair an incorrectly typed method signature.

## ↑ Ancestors (12)

1. [C](../c.md)
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
