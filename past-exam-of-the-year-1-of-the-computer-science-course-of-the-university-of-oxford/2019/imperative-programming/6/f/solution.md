<h1 id="6/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Use one cached optional result. Only a request for availability or the next result fills that cache:
```
class FilterIterator[T](test: T => Boolean, iter: Iterator[T])
    extends Iterator[T] {
  private var cached: Option[T] = None

  private def prepare(): Unit = {
    while (cached.isEmpty && iter.hasNext) {
      val x = iter.next()
      if (test(x)) cached = Some(x)
    }
  }

  def hasNext: Boolean = {
    prepare()
    cached.nonEmpty
  }

  def next(): T = {
    prepare()
    cached match {
      case Some(x) =>
        cached = None
        x
      case None => throw new NoSuchElementException("Filtered iterator exhausted")
    }
  }
}
```
This is a [demand-driven filtering iterator](../../../../../demand-driven-filtering-iterator.md). When the cache is empty, its abstract remaining [sequence](../../../../../sequence.md) is the filtered remaining input. When it holds `Some(x)`, the abstract [sequence](../../../../../sequence.md) is `x` followed by the filtered remaining input. The [loop invariant](../../../../../loop-invariant.md) for `prepare` says that all input elements consumed during the present search have failed `test`, except for the one cached passing value if one has been found. The first passing value stops the loop, so it cannot read past a result that the client has not yet consumed.

**Construction performs no underlying reads, and repeated `hasNext` calls reuse a cached result.** `next` also works without a preceding `hasNext`, clears only the result it returns, and does not prefetch its successor. `Some(x)`, rather than `Option(x)`, allows a passing null value to remain a genuine cached value. For finite remaining input, its length is a [loop variant](../../../../../loop-variant.md); for infinite input, availability can legitimately run forever if no further passing element exists. Deterministic terminating tests and exclusive ownership of the consuming input are assumed. One cache slot is $O(1)$ extra storage.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [6](../../6.md)
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
