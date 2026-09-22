<h1 id="7/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Cache only a requested current element. Merely constructing the [cursor](../../../../../../cursor.md), or asking whether it is nonempty, must not fetch a value from the [iterator](../../../../../../iterator.md):

```
def asCursor[T](it: Iter[T]): Cursor[T] = new Cursor[T] {
  private var cached: Option[T] = None

  def hasCurrent: Boolean = cached.nonEmpty || it.hasNext

  def current: T = {
    if (cached.isEmpty) {
      require(it.hasNext, "empty cursor")
      cached = Some(it.next())
    }
    cached.get
  }

  def next(): Unit = {
    if (cached.nonEmpty) cached = None
    else {
      require(it.hasNext, "empty cursor")
      it.next()
      ()
    }
  }
}
```

The [abstraction function](../../../../../../abstraction-function.md) for the adapter is `it.seq` when no value is cached and `[cachedValue] ++ it.seq` otherwise. Fetching `current` removes one underlying [iterator](../../../../../../iterator.md) value but saves it, so the [cursor](../../../../../../cursor.md)'s abstract [sequence](../../../../../../sequence.md) is unchanged; repeated reads return the same value. Advancing either discards that cache or consumes one uncached [iterator](../../../../../../iterator.md) value. No following element is prefetched.

A too-eager implementation could call `it.next()` at construction, or fetch a new element immediately after every advance, even when the client never requests it. That can trigger unnecessary work or nontermination on a difficult stream. This [lazy iterator-to-cursor adapter](../../../../../../lazy-iterator-to-cursor-adapter.md) avoids both behaviors and checks the underlying access [preconditions](../../../../../../precondition.md) itself. The wrapped [iterator](../../../../../../iterator.md) is assumed to be used exclusively through the adapter; independent external consumption would invalidate the shared-state abstraction.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [7](../../../7.md)
4. [Imperative programming (resit)](../../../../imperative-programming-resit-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
