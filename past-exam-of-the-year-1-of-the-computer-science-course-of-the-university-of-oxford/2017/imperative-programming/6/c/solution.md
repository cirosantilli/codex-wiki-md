<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use a shared memoized [lazy list](../../../../../lazy-list.md) with a separate mutable cursor in each iterator:

```
import scala.collection.immutable.Stream

class FunIter[T] private (
    private var rest: Stream[T]) extends Iter[T] {

  def this(v: T, f: T => T) = this(Stream.iterate(v)(f))

  def hasNext: Boolean = true

  def next(): T = {
    val result = rest.head
    rest = rest.tail
    result
  }

  def copy(): Iter[T] = new FunIter[T](rest)
}
```

For a total step function, the stream is infinite and its values are $v,f(v),f(f(v)),\ldots$. At every call, `rest` starts with the next unconsumed value. Copying that reference gives a new cursor at exactly the same position; later cursor assignments are independent.

The [memoized iterator snapshot](../../../../../memoized-iterator-snapshot.md) is useful for the next part: if `f` owns private mutable state, advancing either cursor realizes a previously unknown tail only once, and both copies can then read the same cached values. Merely constructing `new FunIter(current, f)` would share the mutable closure while generating two independent futures, which could diverge. Memoization instead makes the generated sequence shared and the consumption positions independent. The closure must not be mutated externally, and generic element payloads are shared rather than deep-copied. Retaining an old cursor can retain cached cells.[Opening memoization example and notes on retained heads](../../../../../scala-2-12-stream-api-documentation.md)

## ↑ Ancestors (12)

1. [C](../c.md)
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
