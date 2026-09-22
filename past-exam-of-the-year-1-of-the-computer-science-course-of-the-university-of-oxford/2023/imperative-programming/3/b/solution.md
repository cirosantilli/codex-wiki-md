<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Every operation requires $u\in U$. The queries have [postconditions](../../../../../postcondition.md) “return $I_0(u)$” and “return $O_0(u)$” respectively, leaving both [functions](../../../../../function-split.md) unchanged. An incoming increment additionally requires $I_0(u)<M$ and has

$$
I'(v)=\begin{cases}I_0(u)+1&v=u,\\I_0(v)&v\ne u,\end{cases}\qquad O'=O_0.
$$

The outgoing increment analogously requires $O_0(u)<M$, increments only $O(u)$, and preserves $I$. These frame conditions prevent an implementation from accidentally changing another user's count. Here a subscript zero denotes the old [program state](../../../../../program-state.md).

```
trait Payments {
  // All methods require 1 <= user && user <= 99999999.
  // Queries leave the abstract state unchanged.
  def incoming(user: Int): Int
  def outgoing(user: Int): Int

  // Require the corresponding old count < Int.MaxValue.
  // Increment only that user's named count by one.
  def recordIncoming(user: Int): Unit
  def recordOutgoing(user: Int): Unit
}
```

The [preconditions](../../../../../precondition.md) and [postconditions](../../../../../postcondition.md) are part of the [formal specification](../../../../../formal-specification.md); the trait's [type signatures](../../../../../type-signature.md) alone cannot express all of them. The implementation below uses checked `require` calls for the relevant invalid operations.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
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
