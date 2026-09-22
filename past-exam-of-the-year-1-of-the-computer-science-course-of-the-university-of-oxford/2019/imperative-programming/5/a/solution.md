<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The abstract state is a finite [multiset](../../../../../multiset.md) $Q$ of ordered values, initially empty. Multiplicity matters: deleting the minimum removes one occurrence, not every equal occurrence. Assume a consistent [total order](../../../../../total-order.md) on `T`.
```
trait PriorityQueue[T] {
  // Pre: true. Post: Q' is the empty multiset.
  def clear(): Unit

  // Pre: true. Post: Q' = Q with one additional occurrence of x.
  def insert(x: T): Unit

  // Pre: Q is nonempty.
  // Post: result is a minimum of Q;
  //       Q' is Q with exactly one occurrence of result removed.
  def delMin(): T

  // Pre: true. Post: result iff Q is empty, and Q' = Q.
  def isEmpty(): Boolean
}
```
This [abstract data type](../../../../../abstract-data-type.md) places no fixed-capacity bound on insertion. **The only operation requiring a nonempty collection is `delMin`**. The representation must preserve duplicates even if it uses a [data structure](../../../../../data-structure-split.md) commonly associated with [sets](../../../../../set-split.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
