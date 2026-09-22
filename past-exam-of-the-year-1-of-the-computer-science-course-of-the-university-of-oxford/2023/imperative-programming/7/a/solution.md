<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The **[Memento pattern](../../../../../memento-pattern.md)** supports saving and later restoring an object's state while preserving [encapsulation](../../../../../encapsulation-computer-programming.md). The originator creates a snapshot and knows how to restore it; the memento stores that snapshot; the caretaker retains mementos and decides when to request restoration, without depending on their representation. Undo history is a typical use.

Scala's nested [class in object-oriented programming](../../../../../class-programming.md) definitions, access qualifiers, immutable values and [path-dependent types](../../../../../path-dependent-type.md) help keep snapshots opaque and associated with their originator. For example:

```
final class Editor {
  private var text = ""
  final class Snapshot private[Editor] (
    private[Editor] val saved: String
  )
  def current: String = text
  def edit(next: String): Unit = { text = next }
  def save(): Snapshot = new Snapshot(text)
  def restore(s: Snapshot): Unit = { text = s.saved }
}

val editor = new Editor
editor.edit("first version")
val saved: editor.Snapshot = editor.save()
editor.edit("later version")
editor.restore(saved)
assert(editor.current == "first version")
```

The caretaker can retain `saved` but cannot inspect its private contents or construct an arbitrary snapshot. `editor.Snapshot` is a type tied to the stable `editor` value; a snapshot from a different `Editor` is not interchangeable without an explicit type escape. An immutable [string](../../../../../string.md) is safe to share in this example. If the originator held mutable [arrays](../../../../../array-data-structure.md) or mutable nodes, storing only references to them would not freeze their contents; the memento would need a [deep copy](../../../../../deep-copy.md) or a persistent immutable representation.[Qualified private and constructor access](../../../../../scala-2-13-classes-and-objects-specification.md)[Paths, stable identifiers and path-dependent types](../../../../../scala-2-13-types-specification.md)

## ↑ Ancestors (12)

1. [A](../a.md)
2. [7](../../7.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
