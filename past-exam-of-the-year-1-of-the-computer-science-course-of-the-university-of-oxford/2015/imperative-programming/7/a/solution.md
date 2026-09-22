<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The source comment saying that `hasNext` checks whether the sequence is empty is read in the standard sense “whether another element exists”; the method must return true for a nonempty logical sequence. The example fixes the meaning: skip $n$ source elements and return the next one, repeatedly. Require $n\geq0$. A [lookahead iterator](../../../../../lookahead-iterator.md) must determine whether a complete group of $n+1$ elements exists, since a short final group contributes no result.
```
def skipIter[T](it: Iter[T], n: Int): Iter[T] = {
  require(n >= 0)
  new Iter[T] {
    private var prepared = false
    private var cached: Option[T] = None

    private def prepare(): Unit = {
      if (!prepared) {
        var skipped = 0
        while (skipped < n && it.hasNext) {
          it.next(); skipped += 1
        }
        cached =
          if (skipped == n && it.hasNext) Some(it.next())
          else None
        prepared = true
      }
    }

    def hasNext: Boolean = { prepare(); cached.nonEmpty }

    def next(): T = {
      prepare()
      cached match {
        case Some(v) =>
          cached = None; prepared = false; v
        case None => throw new NoSuchElementException("skipIter.next")
      }
    }
  }
}
```
The [iterator](../../../../../iterator.md) owns consumption of `it`; clients must not independently advance the wrapped source. A prepared `Some(v)` is exactly the next selected source element, and `None` means no complete group remains. Repeated `hasNext` calls use the cached decision, and `next` also works without a preceding `hasNext`. Using `Option[T]` avoids an invalid generic sentinel value, including when a valid element is `null`.

For source elements $a_1,\ldots,a_m$, the result is

$$
\boxed{a_{n+1},a_{2(n+1)},\ldots,a_{\lfloor m/(n+1)\rfloor(n+1)}.}
$$

The extra storage is $O(1)$ and each source element is consumed at most once. `hasNext` may physically consume and cache source elements: an arbitrary [iterator](../../../../../iterator.md) has no non-consuming length query.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [7](../../7.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
