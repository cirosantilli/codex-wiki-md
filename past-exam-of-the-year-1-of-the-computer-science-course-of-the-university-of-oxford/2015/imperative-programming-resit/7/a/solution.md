<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The first matching entry must be retained, and copying an already-started [prefix-dropping iterator](../../../../../prefix-dropping-iterator.md) must not restart the search. Use a private initial buffer together with the underlying [iterator snapshot](../../../../../iterator-snapshot.md):
```
class DropUntil[T] private (
    p: T => Boolean, iter: Iter[T],
    saved: Option[T], alreadyStarted: Boolean) extends Iter[T] {

  def this(p: T => Boolean, iter: Iter[T]) =
    this(p, iter, None, false)

  private var pending: Option[T] = saved
  private var started: Boolean = alreadyStarted

  private def prepare(): Unit = {
    if (!started) {
      var found = false
      while (!found && iter.hasNext) {
        val x = iter.next()
        if (p(x)) {
          pending = Some(x)
          found = true
        }
      }
      started = true
    }
  }

  def hasNext: Boolean = {
    prepare()
    pending.nonEmpty || iter.hasNext
  }

  def next(): T = {
    prepare()
    pending match {
      case Some(x) => pending = None; x
      case None =>
        if (!iter.hasNext) throw new NoSuchElementException("DropUntil.next")
        iter.next()
    }
  }

  def copy(): Iter[T] =
    new DropUntil[T](p, iter.copy(), pending, started)
}
```
Before preparation, the [iterator](../../../../../iterator.md) still represents the original remaining [sequence](../../../../../sequence.md). During the search, the [loop invariant](../../../../../loop-invariant.md) says that every discarded entry fails the [predicate](../../../../../predicate.md), and `pending` is either empty or contains the first satisfying entry just consumed. For a finite input, the number of unread entries is a [loop variant](../../../../../loop-variant.md). After preparation, the abstract remaining [sequence](../../../../../sequence.md) is `pending.toList` followed by the underlying [iterator](../../../../../iterator.md)'s remaining [sequence](../../../../../sequence.md). Repeated `hasNext` calls do not discard or test more entries after the first match.

The [iterator snapshot](../../../../../iterator-snapshot.md) copies both the cached entry and the started flag. In particular, copying after the matching entry has been returned continues with the remaining suffix, including later entries that fail `p`. Restarting `new DropUntil(p, iter.copy())` at that point would wrongly drop another prefix.

$$
\boxed{\operatorname{remaining}=\operatorname{dropWhile}(\neg p,\operatorname{input})\text{ initially; copies preserve the current suffix}.}
$$

As usual, assume a deterministic [predicate](../../../../../predicate.md) without shared mutable effects. On an infinite input having no match, the first demand cannot terminate: no finite inspection establishes absence. Independence here concerns cursor state; arbitrary mutation of shared element objects is outside the [iterator](../../../../../iterator.md) contract.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [7](../../7.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
