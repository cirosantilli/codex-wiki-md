<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A simple current-value implementation works when $f$ is a [pure function](../../../../../pure-function.md), but sharing a mutable [closure](../../../../../closure-topology.md) between copies would violate the independence requirement used in part (d). Use a [memoized successor chain for stateful iterator copies](../../../../../memoized-successor-chain-for-stateful-iterator-copies.md): the generated [sequence](../../../../../sequence.md) has shared cells, and each [iterator](../../../../../iterator.md) has its own current-cell pointer.
```
object FunIter {
  final class Cell[T](val head: T, f: T => T) {
    lazy val tail: Cell[T] = new Cell[T](f(head), f)
  }
}

class FunIter[T](v: T, f: T => T) extends Iter[T] {
  private var cursor = new FunIter.Cell[T](v, f)

  def hasNext: Boolean = true

  def next(): T = {
    val x = cursor.head
    cursor = cursor.tail
    x
  }

  def copy(): Iter[T] = {
    val result = new FunIter[T](cursor.head, f)
    result.cursor = cursor
    result
  }
}
```
The [representation invariant](../../../../../representation-invariant.md) is that `cursor` points to the next cell to be returned, and each cell's lazy tail is computed at most once. The [abstraction function](../../../../../abstraction-function.md) is the infinite [sequence](../../../../../sequence.md) of heads starting at that cell. Advancing changes only this [iterator](../../../../../iterator.md)'s pointer. A copy starts at the same cell, so both observe the same remaining heads even when their calls are interleaved:

$$
\boxed{next\text{ returns }v,f(v),f(f(v)),\ldots;\qquad copy\text{ preserves an independent position}.}
$$

For a stateful $f$, the generator state must be privately owned by this shared chain; unrelated external calls to $f$ must not change it. As usual, the values and transition must allow successive results to be observed without externally mutating old results. No interface can independently clone the hidden state of an arbitrary externally mutated [closure](../../../../../closure-topology.md) from its [function type](../../../../../function-type.md) alone. The chain avoids needing such cloning: a lagging copy reuses the already generated future instead of invoking $f$ again.

Each new cell needs one transition and constant bookkeeping, but retained slower copies can keep a long generated prefix alive. This is an intentional space tradeoff that permits the stateful generator in part (d). No output is possible if computing a demanded transition itself fails or diverges.

## ↑ Ancestors (12)

1. [C](../c.md)
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
