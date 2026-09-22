<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Keep a buffered first match and a flag recording whether the initial prefix still needs to be skipped:

```
class DropUntil[T] private (
    p: T => Boolean,
    iter: Iter[T],
    private var cached: Option[T],
    private var seeking: Boolean) extends Iter[T] {

  def this(p: T => Boolean, iter: Iter[T]) =
    this(p, iter, None, true)

  private def prepare(): Unit = {
    if (seeking) {
      while (cached.isEmpty && iter.hasNext) {
        val x = iter.next()
        if (p(x)) cached = Some(x)
      }
      seeking = false
    }
  }

  def hasNext: Boolean = {
    prepare()
    cached.nonEmpty || iter.hasNext
  }

  def next(): T = {
    prepare()
    cached match {
      case Some(x) => cached = None; x
      case None =>
        if (!iter.hasNext) throw new NoSuchElementException("DropUntil.next")
        iter.next()
    }
  }

  def copy(): Iter[T] = {
    prepare()
    new DropUntil[T](p, iter.copy(), cached, false)
  }
}
```

While seeking, `prepare` drops exactly the rejected prefix and caches the first accepted value, including a possible null payload as `Some(null)`. Afterwards the abstract remainder is the cache, if any, followed by the underlying remainder; later values are returned even when they fail `p`. Repeated `hasNext` calls do not lose the cached value.

The [iterator snapshot](../../../../../iterator-snapshot.md) copies the underlying cursor and the cached value, then marks the initial search complete. It does not reconstruct a fresh two-argument `DropUntil`, which could incorrectly discard later values. Resolving the initial search before copying also avoids having two snapshots independently rerun a privately stateful predicate. The wrapper owns consumption of the supplied source cursor. If that source is infinite and never produces an accepted value, seeking cannot finish. This is a [prefix-dropping iterator](../../../../../prefix-dropping-iterator.md), rather than a repeatedly [demand-driven filtering iterator](../../../../../demand-driven-filtering-iterator.md).

## ↑ Ancestors (12)

1. [A](../a.md)
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
