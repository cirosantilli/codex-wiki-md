<h1 id="7/a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

A single flag represents whether the only element remains:

```
def unitIter[T](t: T): Iter[T] = new Iter[T] {
  private var available = true
  def hasNext: Boolean = available
  def next(): T = {
    require(available, "empty iterator")
    available = false
    t
  }
}

def unitCursor[T](t: T): Cursor[T] = new Cursor[T] {
  private var available = true
  def hasCurrent: Boolean = available
  def current: T = {
    require(available, "empty cursor")
    t
  }
  def next(): Unit = {
    require(available, "empty cursor")
    available = false
  }
}
```

The abstract [sequence](../../../../../../sequence.md) is `[t]` while the flag is true and empty afterward. `current` leaves it unchanged; either advance consumes its sole element. **Renaming both methods to `unit` would leave identical parameter signatures differing only in result type**, which cannot define two such Scala overloads.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [A](../../a.md)
3. [7](../../../7.md)
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
