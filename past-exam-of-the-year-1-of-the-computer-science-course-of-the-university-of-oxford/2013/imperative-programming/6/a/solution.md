<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [prefix-dropping iterator](../../../../../prefix-dropping-iterator.md) must preserve the first satisfying element. Reading it to test the [predicate](../../../../../predicate.md) physically consumes it from the source, so keep it in a one-element buffer. Once a match is found, return the entire suffix without testing subsequent elements again.
```
trait Iter[T] {
  def hasNext: Boolean
  def next(): T
  def copy(): Iter[T]
}

class DropUntil[T](p: T => Boolean, iter: Iter[T]) extends Iter[T] {
  private var seeking = true
  private var saved: Option[T] = None

  private def prepare(): Unit = {
    if (seeking) {
      while (saved.isEmpty && iter.hasNext) {
        val x = iter.next()
        if (p(x)) saved = Some(x)
      }
      seeking = false
    }
  }

  def hasNext: Boolean = {
    prepare()
    saved.nonEmpty || iter.hasNext
  }

  def next(): T = {
    prepare()
    saved match {
      case Some(x) => saved = None; x
      case None =>
        if (!iter.hasNext) throw new NoSuchElementException("next")
        iter.next()
    }
  }

  def copy(): Iter[T] = {
    val result = new DropUntil[T](p, iter.copy())
    result.seeking = seeking
    result.saved = saved
    result
  }
}
```
Assume the source [iterator](../../../../../iterator.md) is owned by the wrapper, its `copy` meets the stated independent-cursor contract, and $p$ is a [pure function](../../../../../pure-function.md). Before preparation, the logical remainder is the source remainder with its maximal initial failing prefix removed. After preparation, it is the buffered match followed by the source remainder, or simply the source remainder when the buffer is empty. This describes the [abstraction function](../../../../../abstraction-function.md) and proves that repeated `hasNext` calls neither lose the match nor skip more values.

Copying preserves the phase flag and optional buffered value and independently copies the source [iterator](../../../../../iterator.md). It does not rerun the [predicate](../../../../../predicate.md) on an already accepted match. A shallow copy of the wrapper alone would give [shared iterator consumption](../../../../../shared-iterator-consumption.md), violating the specification. Therefore

$$
\boxed{\text{DropUntil returns the suffix starting at the first match, with independent copies}.}
$$

When no element satisfies $p$, a finite source yields an empty [iterator](../../../../../iterator.md). Seeking can diverge on an infinite source with no match; this is inherent in determining whether its required suffix begins anywhere. An element object is not deep-copied by this cursor operation.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
