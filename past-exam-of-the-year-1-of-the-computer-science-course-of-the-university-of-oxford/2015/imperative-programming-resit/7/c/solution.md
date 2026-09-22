<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

If `f` is a [pure function](../../../../../pure-function.md) on immutable values, a simple implementation stores the next value and copies it into a fresh `FunIter`. Part (d)'s suggested mutable [programming closure](../../../../../closure-computer-programming.md), however, would be shared by such copies and violate independence. A [memoized iterator snapshot](../../../../../memoized-iterator-snapshot.md) avoids that contradiction: all cursors share already determined [sequence](../../../../../sequence.md) values, but each has its own position.
```
class FunIter[T](v: T, f: T => T) extends Iter[T] {
  private class Cell(val head: T) {
    lazy val tail: Cell = new Cell(f(head))
  }

  private class Cursor(private var cell: Cell) extends Iter[T] {
    def hasNext: Boolean = true

    def next(): T = {
      val answer = cell.head
      cell = cell.tail
      answer
    }

    def copy(): Iter[T] = new Cursor(cell)
  }

  private val cursor = new Cursor(new Cell(v))

  def hasNext: Boolean = true
  def next(): T = cursor.next()
  def copy(): Iter[T] = cursor.copy()
}
```
The first cell stores $v$; its lazily memoized successor stores $f(v)$; the next stores $f(f(v))$, and so on. A cell's successor is evaluated at most once. The [representation invariant](../../../../../representation-invariant.md) is that each cursor points to the cell holding its next result. `next` returns that result and advances only this cursor. `copy` shares the cell, whose future is memoized, rather than the mutable cursor. Advancing either copy therefore cannot skip entries in the other.

$$
\boxed{\operatorname{next}_j=f^{\,j}(v),\quad j=0,1,2,\ldots;\qquad\operatorname{hasNext}=\texttt{true}.}
$$

Assume each demanded application of `f` terminates and generated values are immutable for purposes of observation. A stateful generator should be privately owned by this family of cursors; arbitrary external changes to it cannot be made independent by the supplied interface. Unlike the pure-function implementation, memoization can retain a long prefix while one copy lags far behind another. The question imposes no constant-storage requirement.

## ↑ Ancestors (12)

1. [C](../c.md)
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
