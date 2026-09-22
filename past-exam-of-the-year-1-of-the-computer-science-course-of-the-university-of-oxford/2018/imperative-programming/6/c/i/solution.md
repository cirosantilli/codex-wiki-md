<h1 id="6/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

If [sequence](../../../../../../sequence.md) versions are immutable, replace `perform` by the following method; the insert, delete and move entry points can stay as written:
```
private def perform(forward: () => Unit,
                    backward: () => Unit): Change = {
  val before = songs
  forward()
  val after = songs
  new Change {
    def undo(): Unit = { songs = before }
    def redo(): Unit = { songs = after }
  }
}
```
The unused inverse argument can subsequently be removed from `perform` and its callers. Each history record now captures two complete versions. Undo and redo restore the respective roots without replaying an operation, an instance of the [Memento pattern](../../../../../../memento-pattern.md). The same chronological history discipline still applies.

**The supplied method signatures alone do not establish immutability or persistence.** If `insert` or `delete` changes a shared mutable [software object](../../../../../../software-object.md), merely storing its reference fails to freeze the earlier state. Then independent copies of the relevant state are needed, including any mutable song state intended to be undoable, or the implementation must provide immutable [persistent data structure](../../../../../../persistent-data-structure.md) versions. This is a representation requirement, not a reason to invent a particular unavailable copying API.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [6](../../../6.md)
4. [Imperative programming](../../../../imperative-programming-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
