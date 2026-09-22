<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use a history [dynamic array](../../../../../dynamic-array.md) and a cursor between elements. If the cursor is behind the history's end, `next` replays history; otherwise it pulls a new element from the source. `prev` moves the cursor left and returns the element crossed, so `prev` followed by `next` returns the same element twice and restores the cursor.
```
def genBiIter[T](it: Iter[T]): BiIter[T] = new BiIter[T] {
  private val history = scala.collection.mutable.ArrayBuffer.empty[T]
  private var pos = 0

  def hasPrev: Boolean = pos > 0
  def hasNext: Boolean = pos < history.length || it.hasNext

  def next(): T = {
    if (pos < history.length) {
      val v = history(pos); pos += 1; v
    } else if (it.hasNext) {
      val v = it.next()
      history += v; pos += 1; v
    } else {
      throw new NoSuchElementException("BiIter.next")
    }
  }

  def prev(): T = {
    if (!hasPrev) throw new NoSuchElementException("BiIter.prev")
    pos -= 1
    history(pos)
  }
}
```
The [representation invariant](../../../../../representation-invariant.md) is $0\leq\mathrm{pos}\leq|\mathrm{history}|$, with history exactly the prefix already consumed from the original source. The logical unread [sequence](../../../../../sequence.md) is the history suffix starting at `pos`, followed by the source's remaining [sequence](../../../../../sequence.md). The logical backward history is the prefix before `pos`. Every operation preserves this model, including alternating backward and forward moves after source exhaustion.

$$
\boxed{\text{Memoize the consumed prefix; move a cursor through it before fetching new elements.}}
$$

This [bidirectional iterator](../../../../../bidirectional-iterator.md) uses $O(k)$ storage after consuming $k$ distinct source elements. Replay and backward moves take constant time; appending has [amortized time complexity](../../../../../amortized-time-complexity.md) $O(1)$ under the usual [dynamic array](../../../../../dynamic-array.md) model. The input [iterator](../../../../../iterator.md) must not be advanced separately.

## ↑ Ancestors (12)

1. [B](../b.md)
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
