<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Represent an applied edit by a [command pattern](../../../../../command-pattern.md) object with `undo` and `redo`. Use zero-based positions. For `move(from,to)`, define `to` as the slide's index in the resulting [sequence](../../../../../sequence.md); it is in $[0,n)$ for a presentation of length $n$. Removing the slide first and then inserting at that index implements this convention in either direction.
```
trait Change {
  // Pre: this is the most recent applied change not yet undone.
  def undo(): Unit
  // Pre: this is the next change on the redo history.
  def redo(): Unit
}

class SlideSuite(initial: Sequence[Slide]) {
  private var slides = initial

  private def insertRaw(i: Int, x: Slide): Unit = {
    slides = slides.insert(i, x)
  }

  private def deleteRaw(i: Int): Unit = {
    slides = slides.delete(i)
  }

  private def moveRaw(from: Int, to: Int): Unit = {
    val x = slides.elementAt(from)
    slides = slides.delete(from).insert(to, x)
  }

  def insert(i: Int, x: Slide): Change = {
    insertRaw(i, x)
    new Change {
      def undo(): Unit = deleteRaw(i)
      def redo(): Unit = insertRaw(i, x)
    }
  }

  def delete(i: Int): Change = {
    val x = slides.elementAt(i)
    deleteRaw(i)
    new Change {
      def undo(): Unit = insertRaw(i, x)
      def redo(): Unit = deleteRaw(i)
    }
  }

  def move(from: Int, to: Int): Change = {
    moveRaw(from, to)
    new Change {
      def undo(): Unit = moveRaw(to, from)
      def redo(): Unit = moveRaw(from, to)
    }
  }
}
```
`Sequence` and `Slide` are the supplied external types. Valid insertion positions are $0\leq i\leq n$, deletion positions are $0\leq i<n$, and both move positions are valid indices of the original length. These are the permitted unchecked argument [preconditions](../../../../../precondition.md). The private raw operations perform exactly their named state transformation and do not create history entries. A move to the same index is a legitimate no-op.

The deleted slide must be saved because its index alone cannot reconstruct it. By contrast, insertion already receives the slide to retain. For a move, the inverse of moving the slide from `from` to its final index `to` is to remove it at `to` and reinsert it at `from`; all other slides retain their relative order. Thus each returned object satisfies **`undo` restores the state immediately before the edit, and `redo` restores the state immediately after it**, under the stated history protocol.

A controller can enforce the protocol with two [stacks](../../../../../stack-data-structure.md). This code records changes that have already been executed:
```
class History {
  private var done = List.empty[Change]
  private var undone = List.empty[Change]

  // Pre: c is a fresh, already-applied change of this history's suite.
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
For example, `history.record(suite.move(i,j))` executes and records one move. The [representation invariant](../../../../../representation-invariant.md) says that `done` contains applied changes in reverse application order, while `undone` contains undone changes in the next-redo order, all belonging to the same suite. A fresh edit clears the redo branch. Undo and redo transfer one command between the two heads, so they neither skip intervening edits nor generate new history records. Unrecorded external edits and out-of-order use of old command objects are excluded by this protocol.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [Imperative programming resit](../../../imperative-programming-resit-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
