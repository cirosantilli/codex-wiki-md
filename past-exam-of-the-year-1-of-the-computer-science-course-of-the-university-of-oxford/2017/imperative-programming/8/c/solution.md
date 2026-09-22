<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use a [lower type bound](../../../../../lower-type-bound.md) to widen the element type only in the new value:

```
class ISet[+T](contents: List[T]) {
  private val data: List[T] = contents

  def add[U >: T](x: U): ISet[U] =
    new ISet[U](x :: data)

  def delete(): (T, ISet[T]) = data match {
    case x :: xs => (x, new ISet[T](xs))
    case Nil => throw new NoSuchElementException("ISet.delete")
  }
}
```

The list is immutable and neither method changes this instance. A new wider value cannot be accepted directly as the old narrow `T`; instead `add[U >: T]` returns a fresh `ISet[U]`. The original `ISet[T]` retains its element guarantee, and deletion returns both its old head and a fresh bag for the tail. This [covariant persistent multiset](../../../../../covariant-persistent-multiset.md) safely shares unchanged list tails and preserves duplicate multiplicities. The historical name `ISet` does not require silently changing the question's bag semantics into duplicate-removing set semantics.[Variance Annotations: lower-bound widening of Sequence.append](../../../../../scala-2-13-variance-annotations-specification.md)

## ↑ Ancestors (12)

1. [C](../c.md)
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
