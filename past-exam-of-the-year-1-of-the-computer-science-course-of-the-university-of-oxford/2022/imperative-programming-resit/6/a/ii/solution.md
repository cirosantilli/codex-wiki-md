<h1 id="6/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A mutable character buffer supplies a cached length and constant-time indexed access:

```
class DocImp extends Doc {
  private val data = scala.collection.mutable.ArrayBuffer.empty[Char]

  def insert(pos: Int, ch: Char): Unit = {
    require(0 <= pos && pos <= data.length)
    require(data.length < Int.MaxValue)
    data.insert(pos, ch)
  }

  def delete(pos: Int): Char = {
    require(0 <= pos && pos < data.length)
    data.remove(pos)
  }

  def apply(pos: Int): Char = {
    require(0 <= pos && pos < data.length)
    data(pos)
  }

  def length: Int = data.length
}
```

The [representation invariant](../../../../../../representation-invariant.md) is that `data` is a well-formed private [dynamic array](../../../../../../dynamic-array.md) of at most `Int.MaxValue` characters. Its [abstraction function](../../../../../../abstraction-function.md) is the buffer's character [sequence](../../../../../../sequence.md). Initialization is empty; insertion and removal at the checked position implement exactly the required [sequence](../../../../../../sequence.md) edits, and the queries do not modify it.

**`length` and indexing are $O(1)$** because a [dynamic array](../../../../../../dynamic-array.md) stores its used length and supports address arithmetic for indexed access. An insertion or deletion at position $p$ in a document of length $L$ shifts $O(L-p)$ entries; insertion can additionally resize the backing storage, giving amortized $O(L-p+1)$ time and worst-case $O(L)$ for one operation. Deletion is $O(L-p)$ with an additional constant term.

Building a document by appending the characters of a length-$L$ string costs **$O(L)$ amortized time**, since geometric capacity growth copies a total of only $O(L)$ entries. Thus this implementation does not have the quadratic append behavior of repeated immutable-string concatenation. A known final length can also be reserved in advance. The bounds use the usual [amortized analysis](../../../../../../amortized-analysis.md) of a [dynamic array](../../../../../../dynamic-array.md).[Mutable [sequence](../../../../../../sequence.md) table: ArrayBuffer constant indexed access and amortized constant append](../../../../../../performance-characteristics-of-scala-2-13-collections.md)

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [6](../../../6.md)
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
