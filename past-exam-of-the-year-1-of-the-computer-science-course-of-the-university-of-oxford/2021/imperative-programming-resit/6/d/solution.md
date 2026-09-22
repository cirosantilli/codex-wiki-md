<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Delay both initial skipping and every later skipped entry until a caller actually requests availability or an output:
```
class HalfIterator[T](iter: Iterator[T], odd: Boolean)
    extends Iterator[T] {
  private var needSkip = !odd

  def hasNext: Boolean = {
    if (needSkip && iter.hasNext) {
      iter.next()
      needSkip = false
    }
    iter.hasNext
  }

  def next(): T = {
    if (!hasNext)
      throw new java.util.NoSuchElementException("empty half iterator")
    val result = iter.next()
    needSkip = true
    result
  }
}
```
The state flag means that the next underlying entry, if present, must be skipped before the next selected entry can be exposed. It is initially false for odd positions and true for even positions. Returning a selected entry reinstates that obligation.

Construction does not call the underlying [iterator](../../../../../iterator.md) at all. A successful availability check may discard the one required intervening entry, but does not fetch the selected entry. It then clears the flag, so repeated availability checks cannot skip again. To decide whether a second entry exists through this interface, consuming the preceding discarded entry is necessary. After `next()` returns, it does not eagerly request the following skipped entry. This gives the intended laziness while retaining correct exhaustion behaviour, including an even-position [iterator](../../../../../iterator.md) over a singleton input.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [6](../../6.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
