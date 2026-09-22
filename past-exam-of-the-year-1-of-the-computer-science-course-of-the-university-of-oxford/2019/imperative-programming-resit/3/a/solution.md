<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The abstract state is a finite [partial function](../../../../../partial-function.md) $B$ from [strings](../../../../../string.md) to [strings](../../../../../string.md), initially empty. Names and numbers below are non-null mathematical [strings](../../../../../string.md). `store` replaces an old binding if present; `delete` reports whether a binding existed.
```
trait Book {
  // Abstract state B: finite partial map String -> String; initially empty.

  // Pre: name != null && number != null.
  // Post: B' = B updated at name with number.
  def store(name: String, number: String): Unit

  // Pre: name != null && name is in dom(B).
  // Post: result = B(name), and B' = B.
  def recall(name: String): String

  // Pre: name != null.
  // Post: result iff name is in dom(B), and B' = B.
  def isInBook(name: String): Boolean

  // Pre: name != null.
  // Post: result iff name was in dom(B); B' = B with name removed.
  def delete(name: String): Boolean
}
```
These [preconditions](../../../../../precondition.md) and [postconditions](../../../../../postcondition.md) specify an [abstract data type](../../../../../abstract-data-type.md), independently of any [linked list](../../../../../linked-list.md). In particular, a failed deletion leaves the abstract state unchanged, and recalling a missing name is outside the operation's specified domain.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [Imperative programming resit](../../../imperative-programming-resit-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
