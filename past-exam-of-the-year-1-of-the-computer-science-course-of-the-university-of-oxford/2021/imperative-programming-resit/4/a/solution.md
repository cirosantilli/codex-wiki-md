<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use a finite [sequence](../../../../../sequence.md) $q$ as abstract state, initially empty. One [Scala](../../../../../scala.md) interface is
```
trait DoubleEndedQueue {
  def isEmpty: Boolean
  def addLeft(x: Int): Unit
  def getLeft(): Int
  def addRight(x: Int): Unit
  def getRight(): Int
}
```
The emptiness query has no [precondition](../../../../../precondition.md); its result is $q_0=\langle\rangle$ and its [postcondition](../../../../../postcondition.md) is $q=q_0$. Adding on the left has no [precondition](../../../../../precondition.md) and gives $q=\langle x\rangle\mathbin{++}q_0$. Adding on the right gives $q=q_0\mathbin{++}\langle x\rangle$. Both return `Unit`.

Each removal requires a nonempty incoming [sequence](../../../../../sequence.md). `getLeft()` returns its first entry and leaves the remaining final [sequence](../../../../../sequence.md); `getRight()` returns its last entry and leaves the remaining initial [sequence](../../../../../sequence.md). These contracts remove exactly one occurrence, so duplicate values are permitted and do not collapse the [sequence](../../../../../sequence.md) into a [set](../../../../../set-split.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
