<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The doubling [mixin](../../../../../mixin.md) delegates with a transformed argument.
```
trait DoublePlugin extends Stack {
  override def push(x: Int): Unit = super.push(2 * x)
}
```
For `A`, the relevant [Scala trait linearization](../../../../../scala-trait-linearization.md) is `A, DoublePlugin, SumPlugin, Stack`. A push first doubles the argument, then `SumPlugin` sees and sums that doubled value. The physical values are $2,4,6$ and the total is $12$.

For `B`, the [Scala trait linearization](../../../../../scala-trait-linearization.md) is `B, SumPlugin, DoublePlugin, Stack`. `SumPlugin` sums the original argument, while its `super.push` doubles the stored value. The physical values are still $2,4,6$, but the counter is $1+2+3=6$. Hence the two lines printed are
```
12
6
```
Equivalently,

$$
\boxed{a.sum=12,\qquad b.sum=6.}
$$

This is [stackable trait modification](../../../../../stackable-trait-modification.md): the order determines which arguments an outer [mixin](../../../../../mixin.md) observes. In particular, the running-total specification from part (b) holds for `A` but does not survive the transforming inner [mixin](../../../../../mixin.md) in `B`. With the given implementation, popping from `B` would subtract the doubled stored value, demonstrating why mixing individually sensible [traits](../../../../../trait.md) can break a combined [representation invariant](../../../../../representation-invariant.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
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
