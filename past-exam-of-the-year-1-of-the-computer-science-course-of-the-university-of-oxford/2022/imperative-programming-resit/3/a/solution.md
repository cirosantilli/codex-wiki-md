<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The abstract [FIFO queue](../../../../../fifo-queue.md) state is a finite [sequence](../../../../../sequence.md) $q:[A]$, initially empty. Because the interface returns `Int` length, use the representable-size model $0\leq|q|\leq Int.MaxValue$. Its operations are:

```
trait Queue[A] {
  // State q: finite sequence of A; initially [].
  // Pre: length(q) < Int.MaxValue. Post: q = q0 ++ [x].
  def enqueue(x: A): Unit

  // Pre: q is nonempty. Post: return head(q0); q = tail(q0).
  def dequeue(): A

  // Post: q = [].
  def clear(): Unit

  // Post: q unchanged; return q.isEmpty.
  def isEmpty: Boolean

  // Post: q unchanged; return length(q).
  def length: Int
}
```

The unchanged-state clauses on the two queries are part of their [postconditions](../../../../../postcondition.md). `dequeue` removes exactly the oldest remaining element, while `clear` discards all entries regardless of the old state. The size bound can be omitted in an unbounded mathematical model, but it must be reconciled with fixed-width lengths in an implementation.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
