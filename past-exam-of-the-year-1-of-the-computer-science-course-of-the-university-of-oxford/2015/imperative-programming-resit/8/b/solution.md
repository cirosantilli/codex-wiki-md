<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Represent a [multiset](../../../../../multiset.md) by a pure [multiplicity function](../../../../../multiplicity-function.md). Every operation returns a new [function](../../../../../function-split.md) describing updated counts:
```
class ContraMSet[-T](f: T => Int) {
  def count(x: T): Int = f(x)

  def insert(x: T): ContraMSet[T] =
    new ContraMSet[T]((y: T) => f(y) + (if (y == x) 1 else 0))

  def delete(x: T): ContraMSet[T] =
    new ContraMSet[T]((y: T) => {
      val old = f(y)
      if (y == x && old > 0) old - 1 else old
    })

  def union[U <: T](that: ContraMSet[U]): ContraMSet[U] =
    new ContraMSet[U]((y: U) => this.count(y) + that.count(y))
}
```
An empty instance is `new ContraMSet[T]((_: T) => 0)`. The constructor's [precondition](../../../../../precondition.md) is that `f` is pure and gives a nonnegative [integer](../../../../../integer-split.md) count, with finite [support of a multiset](../../../../../support-of-a-multiset.md) if only finite [multisets](../../../../../multiset.md) are intended. Nonnegativity and the support condition are preserved by each operation. [Integer overflow](../../../../../integer-overflow.md) must be excluded for this fixed-width count interface.

A [contravariant type parameter](../../../../../contravariant-type-parameter.md) makes `ContraMSet[T]` a consumer of values of type `T`. Thus a counter able to answer queries for every animal can also answer queries restricted to cats. It does not expose or enumerate stored `T` values. The [return type](../../../../../return-type.md) `ContraMSet[T]` is legal: its outer covariant result position and the class's contravariant argument position together place $T$ negatively.

For `union`, the argument itself is in a negative position, while its `ContraMSet` argument would reverse that sign. Using `ContraMSet[T]` directly as the parameter type would therefore put $T$ positively and fail the [variance-position rule](../../../../../variance-position-rule.md). Introduce $U<:T$: both operands can count every `U`, and their sum is a `ContraMSet[U]`. This is a restriction to a common query domain; operations do not promise to preserve counts outside the narrowed domain.[Type Parameters, Variance Annotations; bounds and sign changes](../../../../../scala-2-11-basic-declarations-and-definitions-specification.md)

Pointwise evaluation gives

$$
\boxed{f_{\mathrm{insert}(x)}(y)=f(y)+[y=x],\quad
f_{\mathrm{delete}(x)}(y)=\max(0,f(y)-[y=x]),\quad
f_{M\mathrm{\ union\ }K}(y)=f_M(y)+f_K(y).}
$$

No old [function](../../../../../function-split.md) is modified, so updates preserve [immutable object](../../../../../immutable-object.md). Constructing each wrapper takes constant work, but a later `count` may traverse a chain of previously created [programming closures](../../../../../closure-computer-programming.md); its [running time](../../../../../running-time.md) need not be constant in the history length. This functional representation trades enumeration and direct storage of occurrences for composable counting behavior.

## ↑ Ancestors (12)

1. [B](../b.md)
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
