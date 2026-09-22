<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take the abstract state to be a finite [sequence](../../../../../sequence.md) $s$ of [integers](../../../../../integer-split.md), initially empty. Let $s_0$ denote the entry state, $\epsilon$ the empty [sequence](../../../../../sequence.md), and $\mathbin{+\!+}$ concatenation. A [Scala](../../../../../scala.md) [trait](../../../../../trait.md) presents the interface; its comments give the mathematical [preconditions](../../../../../precondition.md) and [postconditions](../../../../../postcondition.md):
```
trait DoubleEndedQueue {
  // Pre: true. Post: result == s0.isEmpty and s == s0.
  def isEmpty: Boolean
  // Pre: true. Post: s == [x] ++ s0.
  def addLeft(x: Int): Unit
  // Pre: s0.nonEmpty. Post: result == s0.head, s == s0.tail.
  def getLeft(): Int
  // Pre: true. Post: s == s0 ++ [x].
  def addRight(x: Int): Unit
  // Pre: s0.nonEmpty. Post: result == s0.last, s == s0.init.
  def getRight(): Int
}
```
The [double-ended queue](../../../../../double-ended-queue.md) has no abstract capacity limit in this first specification. Both removals require nonemptiness; the query leaves the state unchanged, an instance of [command-query separation](../../../../../command-query-separation.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
