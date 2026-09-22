<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [demand-driven filtering iterator](../../../../../demand-driven-filtering-iterator.md) needs one cached accepted value. Otherwise `hasNext` would either lose an element or consume another accepted value every time it is queried.
```
def filterIter[T](p: T => Boolean, it: Iter[T]): Iter[T] =
  new Iter[T] {
    private var buffered: Option[T] = None
    private var finished = false
    private def fill(): Unit = {
      while (buffered.isEmpty && !finished) {
        if (!it.hasNext) finished = true
        else {
          val x = it.next()
          if (p(x)) buffered = Some(x)
        }
      }
    }
    def hasNext: Boolean = {
      fill()
      buffered.nonEmpty
    }
    def next(): T = {
      fill()
      require(buffered.nonEmpty)
      val answer = buffered.get
      buffered = None
      answer
    }
  }
```
The [representation invariant](../../../../../representation-invariant.md) says that `buffered` holds at most one accepted value. The represented [sequence](../../../../../sequence.md) is the buffered value, if present, followed by the subsequence of the underlying remainder satisfying the [predicate](../../../../../predicate.md). Filling moves the next accepted value into the cache and discards only rejected values, so this abstract [sequence](../../../../../sequence.md) is unchanged by `hasNext`. Clearing the cache in `next` removes its head. Thus

$$
\boxed{\alpha(\mathrm{filterIter}(p,it))=\mathrm{filter}(p,\alpha(it)).}
$$

`next` works even when the client has not first called `hasNext`; exhaustion violates its stated precondition. As with ordinary [iterator](../../../../../iterator.md) adapters, clients should give this wrapper exclusive consumption of `it`, and the [predicate](../../../../../predicate.md) should give a stable answer for each element. One call may scan several rejected elements, but across a complete traversal each source element is consumed once. Cache storage is constant.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
