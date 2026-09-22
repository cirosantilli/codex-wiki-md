<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use two finite [integer](../../../../../integer-split.md) [lists](../../../../../list-abstract-data-type.md) $A,B$, with the head of each [list](../../../../../list-abstract-data-type.md) representing its [stack](../../../../../stack-data-structure.md) top. Initially both are empty. A suitable abstract [object interface](../../../../../object-interface.md) is

```
trait DoubleStack {
  def pusha(x: Int): Unit
  def pushb(x: Int): Unit
  def popa: Int
  def popb: Int
  def isEmptya: Boolean
  def isEmptyb: Boolean
}
```

For the unbounded [abstract data type](../../../../../abstract-data-type.md), each push has no logical [precondition](../../../../../precondition.md). The [postcondition](../../../../../postcondition.md) of `pusha(x)` is $A'=x:A$ and $B'=B$; `pushb(x)` symmetrically gives $B'=x:B$ and $A'=A$. The [precondition](../../../../../precondition.md) of `popa` is $A\ne[]$, and its [postcondition](../../../../../postcondition.md) is return value $\operatorname{head}(A)$, new state $A'=\operatorname{tail}(A)$, and unchanged $B$. The specification for `popb` exchanges $A,B$. Each emptiness query leaves both [lists](../../../../../list-abstract-data-type.md) unchanged and returns exactly whether its corresponding [list](../../../../../list-abstract-data-type.md) is empty.

These frame conditions matter: an operation on one [stack](../../../../../stack-data-structure.md) must preserve the other, not merely produce the right return value.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
