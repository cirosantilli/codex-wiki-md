<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

These methods consume the receiver's remaining sequence; `exists` stops as soon as it finds a witness:

```
trait RichIter[T] extends Iter[T] {
  def foreach(f: T => Unit): Unit = {
    while (hasNext) f(next())
  }

  def exists(p: T => Boolean): Boolean = {
    while (hasNext) {
      if (p(next())) return true
    }
    false
  }

  def foldLeft[U](x: U)(f: (U,T) => U): U = {
    var result = x
    while (hasNext) result = f(result, next())
    result
  }
}
```

After $j$ consumed elements, `foreach` has invoked its callback on exactly that prefix, `exists` has found no witness in it unless it has already returned, and the [left fold](../../../../../left-fold.md) accumulator is the fold of that prefix in its original order. These [loop invariants](../../../../../loop-invariant.md) prove the finite-sequence results. On an infinite sequence, `exists` may still terminate when it reaches a witness; a full traversal or fold generally does not. To retain the original cursor, a caller can invoke the operation on a suitable copy.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
