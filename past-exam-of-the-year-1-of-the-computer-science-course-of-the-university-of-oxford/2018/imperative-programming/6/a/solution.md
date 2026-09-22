<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use an inverse edit record with a common undo/redo interface. Positions are zero-based. For `move(i,j)`, **`j` is the song's final index after the move**, so it is also the insertion index in the shortened [sequence](../../../../../sequence.md). For an original length $m$, require $0\leq i,j<m$; insertion permits $0\leq i\leq m$ and deletion requires $0\leq i<m$. As allowed, the caller guarantees validity.
```
trait Change {
  def undo(): Unit
  def redo(): Unit
}

class SongSuite(initial: Sequence[Song]) {
  private var songs = initial
  def length: Int = songs.length
  def elementAt(i: Int): Song = songs.elementAt(i)

  private def rawInsert(i: Int, x: Song): Unit = {
    songs = songs.insert(i, x)
  }
  private def rawDelete(i: Int): Unit = {
    songs = songs.delete(i)
  }
  private def rawMove(i: Int, j: Int): Unit = {
    val x = songs.elementAt(i)
    songs = songs.delete(i)
    songs = songs.insert(j, x)
  }
  private def perform(forward: () => Unit,
                      backward: () => Unit): Change = {
    forward()
    new Change {
      def undo(): Unit = backward()
      def redo(): Unit = forward()
    }
  }
  def insert(i: Int, x: Song): Change =
    perform(() => rawInsert(i, x), () => rawDelete(i))

  def delete(i: Int): Change = {
    val x = songs.elementAt(i)
    perform(() => rawDelete(i), () => rawInsert(i, x))
  }
  def move(i: Int, j: Int): Change =
    perform(() => rawMove(i, j), () => rawMove(j, i))
}
```
`Song` denotes the application's song type, whose internal fields are irrelevant to these operations. `Sequence` denotes the supplied interface; each returned [sequence](../../../../../sequence.md) is assigned back, so the code does not discard the result of a functional implementation. `SongSuite` owns its current [sequence](../../../../../sequence.md); independent mutations through outside aliases are excluded. Atomic successful edits and an ordinary sequential history are assumed.

For [inverse command correctness](../../../../../inverse-command-correctness.md), inserting at $i$ is reversed by deleting at $i$; deleting at $i$ is reversed by reinserting the saved song there. After moving from $i$ to $j$, removing the moved song at $j$ recovers the original [sequence](../../../../../sequence.md) with that one entry missing, and reinserting it at $i$ restores the original. This also covers $i=j$. Store the actual deleted song reference, rather than identifying it by title, since duplicate songs may occur.

The edits have already executed when returned. A history manager can enforce the chronological protocol with two [stacks](../../../../../stack-data-structure.md):
```
class History {
  private var done: List[Change] = Nil
  private var undone: List[Change] = Nil
  def record(c: Change): Unit = {
    done = c :: done
    undone = Nil
  }
  def undo(): Unit = {
    require(done.nonEmpty)
    val c = done.head
    c.undo()
    done = done.tail
    undone = c :: undone
  }
  def redo(): Unit = {
    require(undone.nonEmpty)
    val c = undone.head
    c.redo()
    undone = undone.tail
    done = c :: done
  }
}
```
For example, `history.record(suite.move(i,j))` records an applied move. The history [invariant](../../../../../invariant-mathematics.md) says that the current playlist results from the applied prefix, the top of `done` is its last edit, and the top of `undone` is the first next edit available for redo. Each transfer preserves this [invariant](../../../../../invariant-mathematics.md). A fresh edit clears the redo branch. Calling an arbitrary old inverse after unrelated edits is outside this protocol and need not be correct.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
