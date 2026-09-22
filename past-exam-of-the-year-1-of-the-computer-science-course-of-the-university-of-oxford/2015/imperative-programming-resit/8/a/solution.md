<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Store one entry per occurrence in an immutable [list](../../../../../list-abstract-data-type.md). Use [lower type bounds](../../../../../lower-type-bound.md) for arguments that might widen the element type, and remove only the first matching occurrence:
```
class CoMSet[+T](c: List[T]) {
  private val elems: List[T] = c

  def insert[U >: T](x: U): CoMSet[U] =
    new CoMSet[U](x :: elems)

  def delete[U >: T](x: U): CoMSet[T] = {
    def removeOne(xs: List[T]): List[T] = xs match {
      case Nil => Nil
      case h :: tail =>
        if (h == x) tail else h :: removeOne(tail)
    }
    new CoMSet[T](removeOne(elems))
  }

  def count[U >: T](x: U): Int =
    elems.count(y => y == x)

  def union[U >: T](that: CoMSet[U]): CoMSet[U] =
    new CoMSet[U](elems ::: that.elems)
}
```
A [covariant type parameter](../../../../../covariant-type-parameter.md) cannot appear directly as an ordinary [object method](../../../../../object-method.md) argument type. The fresh $U$ with $T<:U$ permits insertion, deletion queries and count queries without imposing such a negative occurrence of $T$. `delete` can retain result type `CoMSet[T]` because it introduces no new elements; widening its result to `CoMSet[U]` would also be valid. `union` must widen because the other [multiset](../../../../../multiset.md) may contain the broader type. The class-private immutable `elems` is accessible on another instance of the same [software class](../../../../../class-programming.md); it is not `private[this]`.[Type Parameters, Variance Annotations; variable and method parameter positions](../../../../../scala-2-11-basic-declarations-and-definitions-specification.md)

Let $c_M(y)$ be a [multiset multiplicity](../../../../../multiset-multiplicity.md). The implementations satisfy

$$
\boxed{\begin{aligned}
c_{M.\mathrm{insert}(x)}(y)&=c_M(y)+[y=x],\\
c_{M.\mathrm{delete}(x)}(y)&=\max(0,c_M(y)-[y=x]),\\
M.\mathrm{count}(x)&=c_M(x),\\
c_{M.\mathrm{union}(K)}(y)&=c_M(y)+c_K(y).
\end{aligned}}
$$

The brackets denote an [indicator function](../../../../../indicator-function.md). [Structural induction](../../../../../structural-induction.md) on the [list](../../../../../list-abstract-data-type.md) proves `removeOne` removes precisely one equal entry if present, otherwise none. `filterNot` would incorrectly remove every occurrence. [List concatenation](../../../../../list-concatenation.md) adds multiplicities, implementing the paper's additive [additive multiset union](../../../../../additive-multiset-union.md), rather than the maximum-multiplicity convention sometimes used for that name.

All methods preserve the original [immutable object](../../../../../immutable-object.md). `insert` takes constant time through [structural sharing](../../../../../structural-sharing.md); `count` and `delete` take $O(n+1)$ time, and `union` takes $O(n+1)$ time to copy the receiver's list spine. Equality is ordinary stable value equality; finite representable counts are assumed.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [8](../../8.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
