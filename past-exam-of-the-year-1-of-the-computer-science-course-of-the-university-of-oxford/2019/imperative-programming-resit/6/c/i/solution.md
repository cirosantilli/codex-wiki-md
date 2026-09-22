<h1 id="6/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Replace edit-specific inverse information by before/after snapshots implementing the [Memento pattern](../../../../../../memento-pattern.md). The same `Change` and `History` interfaces still work. A complete alternative suite is:
```
class SnapshotSlideSuite(initial: Sequence[Slide]) {
  private var slides = initial

  private def changeTo(after: Sequence[Slide]): Change = {
    val before = slides
    slides = after
    new Change {
      def undo(): Unit = { slides = before }
      def redo(): Unit = { slides = after }
    }
  }

  def insert(i: Int, x: Slide): Change =
    changeTo(slides.insert(i, x))

  def delete(i: Int): Change =
    changeTo(slides.delete(i))

  def move(from: Int, to: Int): Change = {
    val x = slides.elementAt(from)
    changeTo(slides.delete(from).insert(to, x))
  }
}
```
By-value evaluation computes `after` without changing `slides`, then `changeTo` captures the still-current `before` and installs the new value. The `val` bindings inside each call are stable snapshots, rather than later reads of a mutable variable. Under the same chronological history [preconditions](../../../../../../precondition.md), **undo and redo are constant-time reference assignments**. This is the [Memento pattern](../../../../../../memento-pattern.md) applied to an immutable [sequence](../../../../../../sequence.md). Retaining a reference to an in-place-mutated [sequence](../../../../../../sequence.md) would not save its old state. The snapshot covers slide order and membership; it does not promise to undo unrelated mutations inside a `Slide` object.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [6](../../../6.md)
4. [Imperative programming resit](../../../../imperative-programming-resit-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
