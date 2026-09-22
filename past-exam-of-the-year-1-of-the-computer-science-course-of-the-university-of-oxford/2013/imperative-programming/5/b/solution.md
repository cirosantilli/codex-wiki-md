<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Keep a running total in the [mixin](../../../../../mixin.md), and use only the inherited public operations. Updating after a successful superclass operation leaves the total unchanged if an empty `pop` fails its [precondition](../../../../../precondition.md).
```
trait SumPlugin extends Stack {
  private var total = 0

  override def push(x: Int): Unit = {
    super.push(x)
    total += x
  }

  override def pop(): Int = {
    val x = super.pop()
    total -= x
    x
  }

  def sum: Int = total
}
```
For this [trait](../../../../../trait.md) mixed directly into `Stack`, its [representation invariant](../../../../../representation-invariant.md) is $total=\sum s$, where $s$ is the abstract [stack](../../../../../stack-data-structure.md) [sequence](../../../../../sequence.md). A successful push adds exactly its argument and a successful pop removes exactly its returned value. Thus

$$
\boxed{sum=\text{the sum of the current stack entries},\qquad sum(\text{empty stack})=0.}
$$

The [mixin](../../../../../mixin.md) reads no private `Stack` fields. Its operations add constant [time complexity](../../../../../time-complexity.md). As in the paper's `Int` interface, an unbounded mathematical total requires excluding [integer overflow](../../../../../integer-overflow.md), or replacing the accumulator with `BigInt` if the interface is allowed to change. A later [mixin](../../../../../mixin.md) can transform a pushed value at a different point in the [Scala trait linearization](../../../../../scala-trait-linearization.md); the effect is analyzed in the next part.

## ↑ Ancestors (12)

1. [B](../b.md)
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
